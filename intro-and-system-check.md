---
title: System Check
layout: default
nav_order: 2
---

# Activity 1.1: Fork & Commit

1. Open your browser and log into [GitHub.com](https://github.com).
 
2. Navigate to or search for the **[futureDocs](https://github.com/ctodocs/futureDocs)** repository.
 
3. Fork this repository and go to your fork, if your browser doesn’t automatically switch you to it.
 
4. Go to your Fork’s repository settings, and then to GitHub Pages settings. Click on the drop down menu below "Source" and select ‘gh-pages’.
 
5. Here you should see your site link as well - Ctrl+click the URL to view your site in a new tab (or reload if you've already got it open).
 
6. Open GitHub Desktop, and clone this repo to your local system:
  * File > Clone: Your list of owned repositories should appear, but if not, head back over to the front page of the repo in the browser and copy/paste the URL then use that. Once back in GitHub Desktop and you've cloned the repo, be sure you’re in the ```gh-pages``` branch.
 
7. Note: The local destination for this repo will be in your Documents folder, within a GitHub folder (```yourusername/Documents/Github/futureDocs```) by default, unless you've updated your destination preferences in GitHub Desktop.
 
8. Open your project in VSCode. Your repository will be visible in the explorer, and you should see the following files:
 
```
.
├── _site
├── assets
├── Gemfile.lock
├── Gemfile
├── LICENSE.txt
├── 404.html
├── package-lock.json
├── package.json
├── _config.yml
├── about.markdown
├── adminDocs
├── docTemplates.md
    └── contributionPolicy.md
├── about.markdown
├── index.markdown
└── README.md
```

9. Select the README.md file in your explorer and go ahead and edit your README.
```
# Hello Docs!
```
 
10. Save your changes. In GitHub Desktop, you should now see the change you made being tracked. Write a commit message and commit this change.
 
11. Push this change to the remote version with the ```Push``` button in the upper right corner of GH Desktop.
 
12. In your browser, on the landing page of your fork's repository on GitHub.com, you should now see your updated README.
 
**Congrats!** You just committed a change!
 
# Activity 1.2: System Check
Now that you've updated your README, let's check to make sure your fork's jekyll site is up and running.
1. In your VSCode terminal, your working directory should already be the repository, because VSCode is smart. From here, run:
```
bundle install
```

2. Running the following will build your site locally
```
bundle exec jekyll serve
```
 
3. Navigate to [http://localhost:4000/](http://localhost:4000/) in your browser. You should see a site there.
 
4. To stop serving
```
Ctrl+c
```