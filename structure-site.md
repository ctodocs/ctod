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
The structure of your pages and the site should be consistent. Make sure the organization you use for pages works for your site too.  
## Navigation
* Navigation is on the left side of the screen (just the docs).
* Use YAML front matter to structure navigation 
* ```nav_order:``` designates the position in navigation.
* ```nav_exclude:``` hides page from navigation display.
## Multi-level Menu
* ```has_children: true``` allows subpages.
* ```parent:``` designates higher level page current page appears under.
* ```grandparent:``` designates top level page.
* Don’t go deeper than Grandparent > Parent > Child
## Table of Contents
* ```{:toc}``` to autogenerate with kramdown.
* ```{: .no_toc }``` and ```{: .no_toc .text-delta }``` to exclude table of contents.
* Use the same organization for navigation and documents where possible - link where not possible.cs
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



