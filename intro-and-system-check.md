---
title: Intro to Tools & System Check
layout: default
nav_order: 2
---

# Activity 1.1: First, Commit

1. Open your browser and log into [GitHub.com](https://github.com).

2. Navigate to or search for the **[futureDocs](https://github.com/ctodocs/futureDocs)** repository.

3. Fork this repository and go to your fork.

4. Go to your Fork’s repository settings, and then to GitHub Pages settings. Click on the "source branch" drop down and select ‘gh-pages’.

5. Here you'll also see your site link - click the URL to view your site (or reload if you've already got it open). You should see a website.

7. Open GitHub Desktop, and clone this repo (File > Clone). It should show up in your list of owned repositories, but if not, head back over to the front page of the repo and copy/paste the URL and use that. Once back in GitHub Desktop, be sure youre in the ```gh-pages``` branch.

8. The destination for this repo will be ```yourusername/Documents/Github/futureDocs``` by default, unless you've updated your destination preferences in GitHub Desktop.

9. Open a terminal window and navigate to your local repository
```
cd ~/Documents/GitHub/futureDocs
```

10. Now list the unhidden files in your current directory
```
ls
```
... You should see the following
```
404.html                LICENSE                 _site                   index.markdown          pagetwo.md
Gemfile                 README.md               about.markdown          package-lock.json
Gemfile.lock            _config.yml             assets                  package.json
```

15. Open the README.md file (if you're using VSCode Terminal, it should open in VSCode)
```
open README.md
```
16. This should open in VSCode. Select the markdown preview tool in the upper right corner of the window and edit your README.
```
# docs are awesome!
```

17. Save your changes. In GitHub Desktop, you should now see the change you made being tracked. Write a commit message and commit this change.

18. In your browser, on the landing page of your fork's repository on GitHub.com, you should now see your updated README.

**Congrats!** You just committed a change!

## Activity 1.2: System Check
Now that you've updated your README, let's check to make sure your fork's jekyll site is up and running.
```
bundle install
```
10. Then un the following to test your build
```
bundle exec jekyll serve
```

11. Navigate to [http://localhost:4000/](http://localhost:4000/) in your browser. You should see a site there.

12. To stop serving
```
Ctrl+c
``` 
