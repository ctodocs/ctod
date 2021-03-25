---
title: Writing Markdown
layout: default
nav_order: 4
---
<details closed markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

# Let's Write Some Docs

So far this workshop has covered a set of technologies to build and serve documentation and a toolset for how to write good documentation.
Now we will cover how to combine those two skills, by writing good documentation using Markdown.
There are two activities.
The first is to [update `index.markdown`](#activity-1).
The second is to [create your own page](#activity-2).


## What is Markdown?
Markdown is a markup language like XML and HTML, but it is focused on text documents.
It also tries to balance human-readability and machine-readability by offering a constrained set of formatting features that require minimal taggin.
For example:
* Paragraphs
* Headings
* Bulleted and Numbered Lists
* Code Sections
* Links

This workshop covers each of these features.

Markdown is used in Jekyll, but it is also useful for writing READMEs, contributing to Wikis, and in many other text environments in technology.

Markdown is a text format.
Common file extensions include `.md` and `.markdown`.
To write a Markdown file we need a text editor, a program built to manipulate text formats.
Examples include Visual Studio Code, SublimeText, Notepad++, Atom, Notepad.
We do not mean a word processor like Microsoft Word or Google Docs.
While you can write Markdown text in these programs it is harder to export them as text files.
Plus, text editors have a wide variety of useful features and extensions.

## Visual Studio Code, A Markdown Editor

Visual Studio Code is an example of a text editor with many useful features that makes it easier to work on a project like a Jekyll site.

When you open Visual Studio you see at least two interface sections:
* a sidebard on the left side of the window
* a tabbed panel that occupies most of the window

### Sidebar

Clicking on any of the icons in the sidebard will expand the panel to show its features.

* Explorer, browse the file and folders in a project
* Search, search across all the files opened in explorer
* Git, debug, extensions: further features to incorporate depending on 

Clicking an icon again will hide the panel.

For this workshop, we will only use the Explorer panel.
1. Open the Explorer panel
2. Click on `Open Folder`
3. Open the 'futureDocs' folder you downloaded for this workshop

Now the Explorer panel should have a tree view of the files in that folder, including icons to indicate each file type.

### Editor Area

When you click on a file from the Explorer view, it opens in the Editor area. 
This area has its own features. 
For example:
* click once on a file in Explorer to preview it in Editor.
* click once on another file to replace that preview
* double-click on a file to open the file as its own tab

On the right side of the panel, there is a miniaturized version of the currently open file that you can use as a scroll bar.

At the top of the panel:
* tabs let you switch between multiple open documents
* a document with unsaved changes has a circle on its tab
* buttons in the top right let you open additional panels or a Preview panel.


#### Preview Panels

The Editor can be split into multiple panels, so that you can view and edit files side by side.
One of the built-in features that makes this incredibly useful is a markdown preview editor.
This feature renders the markdown document you are currently editing so that you can see how it would generally appear on your site.

To preview a markdown document:
1. Double-click on the `index.markdown` file from the Explorer
2. In the top bar of the Editor, click the split box with the magnifying class
3. Scroll up and down in the left panel. You should see the right panel scroll as well.

### Terminal

One final feature of Visual Studio Code that we will use in this workshop is the built-in terminal. This allows you to perform any terminal tasks without having to leave the text editor.

To open the terminal:
1. Open the Terminal menu in the menu bar at the top
2. Click `New Terminal`

This terminal uses the same shell and configuration as your system's default terminal. You can run commands like `ls -al` and `brew list` just like in a dedicated terminal program.

The working directory for the terminal is your project folder. For us, when we run `bundle exec jekyll serve`, that means the bundle program will build the jekyll site we're currently editing.

# Markdown
We will use the `index.markdown` page to explore the syntax of Markdown.

## Jekyll Frontmatter
At the top of `index.markdown`, you should see a section surrounded by dash marks with several `key: value` pairs.

```
---
title: Front Page
layout: default
nav_order: 1
---
```
This is the Jekyll frontmatter, metadata that will be used to render your site correctly.
For now, we will leave this as-is.
The Markdown text that we are interested in begins below the second set of dashes.\

## Headings
Headings help writers and editor structure the information and readers find the information they are looking for.
The visual effect of headers is a different font size and color, but it's better to use a header instead of altering the font because headers can be interpreted by assistive technology like screen readers.

Do not skip levels when using headings, for example putting a level 4 heading directly after a level 6 heading.
This creates confusion for the reader trying to understand the structure of the document.

### How to

To use a heading:
1. begin the line with the number `#` symbols to match your heading level
2. include at least one space
3. write the text of your heading

* `# Heading Title` is a level 1 heading
* `## Heading Title` is a level 2 heading
* `###### Heading Title` is a level 6 heading

If you don't start the line `#`, the `#` is interpreted as a pound sign.
If you don't put a space after the `#`, the line is interpreted as a comment

## Paragraphs
Paragraphs are used to break up sections of text into smaller units.
Readers tend to skim more as paragraph length increases.
Ideally, your documentation should keep paragraphs and paragraph-length to a minimum.

### How to
To create a new paragraph:
1. Press enter to move to a new line at the end of a sentence.
2. Press enter again to move a new line, leaving a blank line.
3. Write your next sentence

Markdown considers every line of text not separated by a blank line to be part of a paragraph.
Use this to your advantage by writing each sentence on a new line.
While that may be confusing to you as a writer, it highlights when sentences are getting too long for reader comfort.


## Bulletted and Numbered Lists
Lists are a core part of documentation.
They can be used to break down a complex task, create a checklist, or document the order of steps.

### How to
To create a bulletted list:
1. Start a new line with `* ` followed by your text. You can also use `- ` or `+ `, but the rendered symbol will be the same.
2. For another bullet, start the next new line with `* `
3. For a sub-bullet, start the next new line with two spaces and then `* `.

To create a numbered list:
1. Start a new line with `1. ` followed by your text. 
2. For another bullet, start the next new line with the next number in the sequence `2. `. Markdown will still make a list with any number though.
3. For a sub-bullet, start the next new line with two spaces and then `1. `.

## Code Sections
Code sections make it clear when text should interpreted as code.
Common examples include using the command line, adding lines to scripts, or other typing tasks.
Markdown includes methods to denote short and long pieces of code.

### How to
To insert a short piece of code:
1. Begin the code section in the text with a backtick mark, `` ` ``.
2. Write the code phrase.
3. Finish the section with a second backtick mark, `` ` ``.

To insert a multi-line piece of code:
1. Start a new line with 3 backtick marks, `` ``` ``.
2. On a new line begin writing lines of code.
3. On a new line, finish the code block with 3 backtick marks, `` ``` ``.

## Links
Links are critical for creating connections between documents and other sites.

### How to
To turn a phrase into a hyperlink:
1. Surround the phrase you want to turn into a hyperlink with square brackets, `[link text]`.
2. Immediately after the closing square bracket, add a left parenthesis, the link target, and a right parentheses, `(http://example.com/page)`.

* To link to a page outside of your documentation site, use a full url, `http://example.com`.
* To link to a page within your site, use the relative path from the root of your website, `/index.markdown`

# Activity
Take a draft document you created in the previous step and turn it into a Markdown document.

* Add at least one level-1 header.
* Separate your sentences onto new lines.
* Add at least one bulletted or numbered list.
* Add a link to an external website.
* Add a link to another page on your website.

# Let's Write Some Docs

So far this workshop has covered a set of technologies to build and serve documentation and a toolset for how to write good documentation.
Now we will cover how to combine those two skills, by writing good documentation using Markdown.


## What is Markdown?
Markdown is a markup language like XML and HTML, but it is focused on text documents.
It also tries to balance human-readability and machine-readability by offering a constrained set of formatting features that require minimal taggin.
For example:
* Paragraphs
* Headings
* Bulleted and Numbered Lists
* Code Sections
* Links

This workshop covers each of these features.

Markdown is used in Jekyll, but it is also useful for writing READMEs, contributing to Wikis, and in many other text environments in technology.

Markdown is a text format.
Common file extensions include `.md` and `.markdown`.
To write a Markdown file we need a text editor, a program built to manipulate text formats.
Examples include Visual Studio Code, SublimeText, Notepad++, Atom, Notepad.
We do not mean a word processor like Microsoft Word or Google Docs.
While you can write Markdown text in these programs it is harder to export them as text files.
Plus, text editors have a wide variety of useful features and extensions.

## Visual Studio Code, A Markdown Editor

Visual Studio Code is an example of a text editor with many useful features that makes it easier to work on a project like a Jekyll site.

When you open Visual Studio you see at least two interface sections:
* a sidebard on the left side of the window
* a tabbed panel that occupies most of the window

### Sidebar

Clicking on any of the icons in the sidebard will expand the panel to show its features.

* Explorer, browse the file and folders in a project
* Search, search across all the files opened in explorer
* Git, debug, extensions: further features to incorporate depending on 

Clicking an icon again will hide the panel.

For this workshop, we will only use the Explorer panel.
1. Open the Explorer panel
2. Click on `Open Folder`
3. Open the 'futureDocs' folder you downloaded for this workshop

Now the Explorer panel should have a tree view of the files in that folder, including icons to indicate each file type.

### Editor Area

When you click on a file from the Explorer view, it opens in the Editor area. 
This area has its own features. 
For example:
* click once on a file in Explorer to preview it in Editor.
* click once on another file to replace that preview
* double-click on a file to open the file as its own tab

On the right side of the panel, there is a miniaturized version of the currently open file that you can use as a scroll bar.

At the top of the panel:
* tabs let you switch between multiple open documents
* a document with unsaved changes has a circle on its tab
* buttons in the top right let you open additional panels or a Preview panel.


#### Preview Panels

The Editor can be split into multiple panels, so that you can view and edit files side by side.
One of the built-in features that makes this incredibly useful is a markdown preview editor.
This feature renders the markdown document you are currently editing so that you can see how it would generally appear on your site.

To preview a markdown document:
1. Double-click on the `index.markdown` file from the Explorer
2. In the top bar of the Editor, click the split box with the magnifying class
3. Scroll up and down in the left panel. You should see the right panel scroll as well.

### Terminal

One final feature of Visual Studio Code that we will use in this workshop is the built-in terminal. This allows you to perform any terminal tasks without having to leave the text editor.

To open the terminal:
1. Open the Terminal menu in the menu bar at the top
2. Click `New Terminal`

This terminal uses the same shell and configuration as your system's default terminal. You can run commands like `ls -al` and `brew list` just like in a dedicated terminal program.

The working directory for the terminal is your project folder. For us, when we run `bundle exec jekyll serve`, that means the bundle program will build the jekyll site we're currently editing.

# Markdown
We will use the `index.markdown` page to explore the syntax of Markdown.

## Jekyll Frontmatter
At the top of `index.markdown`, you should see a section surrounded by dash marks with several `key: value` pairs.

```
---
title: Front Page
layout: default
nav_order: 1
---
```
This is the Jekyll frontmatter, metadata that will be used to render your site correctly.
For now, we will leave this as-is.
The Markdown text that we are interested in begins below the second set of dashes.\

## Headings
Headings help writers and editor structure the information and readers find the information they are looking for.
The visual effect of headers is a different font size and color, but it's better to use a header instead of altering the font because headers can be interpreted by assistive technology like screen readers.

Do not skip levels when using headings, for example putting a level 4 heading directly after a level 6 heading.
This creates confusion for the reader trying to understand the structure of the document.

### How to

To use a heading:
1. begin the line with the number `#` symbols to match your heading level
2. include at least one space
3. write the text of your heading

* `# Heading Title` is a level 1 heading
* `## Heading Title` is a level 2 heading
* `###### Heading Title` is a level 6 heading

If you don't start the line `#`, the `#` is interpreted as a pound sign.
If you don't put a space after the `#`, the line is interpreted as a comment

## Paragraphs
Paragraphs are used to break up sections of text into smaller units.
Readers tend to skim more as paragraph length increases.
Ideally, your documentation should keep paragraphs and paragraph-length to a minimum.

### How to
To create a new paragraph:
1. Press enter to move to a new line at the end of a sentence.
2. Press enter again to move a new line, leaving a blank line.
3. Write your next sentence

Markdown considers every line of text not separated by a blank line to be part of a paragraph.
Use this to your advantage by writing each sentence on a new line.
While that may be confusing to you as a writer, it highlights when sentences are getting too long for reader comfort.


## Bulletted and Numbered Lists
Lists are a core part of documentation.
They can be used to break down a complex task, create a checklist, or document the order of steps.

### How to
To create a bulletted list:
1. Start a new line with `* ` followed by your text. You can also use `- ` or `+ `, but the rendered symbol will be the same.
2. For another bullet, start the next new line with `* `
3. For a sub-bullet, start the next new line with two spaces and then `* `.

To create a numbered list:
1. Start a new line with `1. ` followed by your text. 
2. For another bullet, start the next new line with the next number in the sequence `2. `. Markdown will still make a list with any number though.
3. For a sub-bullet, start the next new line with two spaces and then `1. `.

## Code Sections
Code sections make it clear when text should interpreted as code.
Common examples include using the command line, adding lines to scripts, or other typing tasks.
Markdown includes methods to denote short and long pieces of code.

### How to
To insert a short piece of code:
1. Begin the code section in the text with a backtick mark, `` ` ``.
2. Write the code phrase.
3. Finish the section with a second backtick mark, `` ` ``.

To insert a multi-line piece of code:
1. Start a new line with 3 backtick marks, ```` ``` ````.
2. On a new line begin writing lines of code.
3. On a new line, finish the code block with 3 backtick marks, ```` ``` ````.

## Links
Links are critical for creating connections between documents and other sites.

### How to
To turn a phrase into a hyperlink:
1. Surround the phrase you want to turn into a hyperlink with square brackets, `[link text]`.
2. Immediately after the closing square bracket, add a left parenthesis, the link target, and a right parentheses, `(http://example.com/page)`.

To link to a page outside of your documentation site, use a full url, `http://example.com`.
To link to a page within your site, use the relative path from the root of your website, `/index.markdown`

# Activity 1
Updating your front page
1. Update `index.markdown` to describe what you are documenting.
  1. Add one level-2 header.
  2. Add a paragraph under each header.
  3. Add one link to an external website.
2. Save your changes to `index.markdown`.
3. Run the local site from the terminal in VS Code, `bundle exec jekyll serve`.
4. View your local instance of the website to make sure it looks correct.
5. Commit and push your changes to your Github repository.
6. View your live site.

# Activity 2
Adding a page of documentation
1. Create a new document in VS Code.
2. Copy the draft document you created previously into the new document and add markdown tags as needed.
3. Copy Jekyll frontmatter to the top of the document and paste it at the top of the new document. Adjust the title.
4. Save the document in the root folder of your project.
5. View your local instance of the website to make sure it looks correct.
6. Commit and push your changes to your Github repository.
7. View your live site.

# Advanced Markdown
This is an introduction to Markdown.
It should get you the basic toolset to write your base set of your documentation.
As you refine your documentation, you might need additional features.

## Adding images
Images are very useful, but take additional time to create and not always accessible.
It's good practice to write and publish your documentation first, and then add images in a later step.

### How to
To add an image in Jekyll markdown:
1. Start a new line with a exclamation point, `!`.
2. Write the alt text for the image surrounded in square brackets, `[description of the content of the image]`.
3. Write the location of the image surrounded by parentheses, `(\assets\images\screenshot.png)`.

Common Jekyll practice is to store images in an `\assets\images` folder.

## Programming in Jekyll
Jekyll supports some scripting tasks, like getting variable values, assigning css classes, running if-then statements, and executing plug-ins.
These pieces of executable code are wrapped in curly braces, `{}`.
For example:
* Double curly braces `{{ }}` are used for variables, for example, `{{ site.url }}` is the url for your site.
* A curly brace followed by a colon `{: }` is used for CSS class. For example, `{: .toc }` creates a document element with a .toc class.
* A curly brace with percent signs {% raw %}`{% %}`{% endraw %} is used for executable statements. For example, `{% highlight ruby %} ... {% endhighlight %}` is a plugin that adds ruby syntax highlighting to a code block. 

These features are good for extending the functionality of your documentation, but they should be explored after completing your text.

## Using HTML
Jekyll will also render any valid HTML in a markdown document.

### How to
If you wanted to write a link with HTML
1. In your text, begin the link with `<a href='http://example.com'>`
2. Write the text to be linked.
3. Follow the text with a closing tag `</a>`.
