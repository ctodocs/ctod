---
title: Structuring the Site
layout: default
nav_order: 5


---

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

# Structuring the Site
Now that you have more than one page this section will address structuring your Github Pages site. At the end of this section you will complete an [activity](#activity).  

Be consistent when you structure your pages and the site. Make sure the organization you use for pages works for your site too. You can create repository folders that mirror top level navigation to keep your repository manageable.   
## Navigation
* Navigation is on the left side of the screen (just the docs).
* Use YAML front matter to structure navigation.  
```
---
title: Structuring the Site
layout: default
nav_order: 5
---
```  
* ```nav_order:``` designates the position in navigation.
* ```nav_exclude: true``` hides page from navigation display.

## Multi-level Menu
* ```has_children: true``` allows subpages.
* ```parent:``` designates higher level page current page appears under.
* ```grandparent:``` designates top level page.
* Don’t go deeper than Grandparent > Parent > Child

## Table of Contents
* ```{:toc}``` to autogenerate with kramdown.
* ```{: .no_toc }``` and ```{: .no_toc .text-delta }``` to exclude table of contents.
* Use the same organization for navigation and documents where possible - link where not possible.
  * ```[Example](#example)``` Link to different sections of longer documents.
<div class="code-example" markdown="1">
**Good Example**

## Beginning the transfer
The transfer software will depend on the type of device. See the associated documentation for the correct device.  
* Legacy Removeable Media - [FTK Imager](link)
* CD and DVD Media - [optical.sh](link)
* External and Internal Hard Drives - [FT.sh](link)
</div>
* See [just-the-docs](https://pmarsceill.github.io/just-the-docs/docs/navigation-structure/){:target="_blank"} for more examples.
* Use ```details``` and ```summary``` elements to create an expandable TOC.

<div class="code-example" markdown="1">
```markdown
<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>
```

# Activity
* Change the ```nav_order:``` number on the front matter of a page.  
* View changes on your local site.  
* Create an expandable TOC on a page.  
* Experiment with navigation and front matter options.  

