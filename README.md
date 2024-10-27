# Flintlock District, Spirit of Adventure Council, Scouting America, Boston MA

This is the repository that backs www.flintlockscouting.org - the informational site for adult Scouting America leaders who live in the Flintlock District of The Spirit of Adventure Council, Boston MA. This site is a work in progress where we are attempting to provide a Github Pages driven database of resources for Scouters to collect and share ideas, and publish them on the web.

## Contributing

This site is built using [Github Pages](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/about-github-pages-and-jekyll) and the [Just-the-Docs Theme](https://just-the-docs.com/). 

Contributors should familiarize themselves with [Github Markdown](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) and [Shopify Liquid templates](https://github.com/Shopify/liquid) as all pages/posts on this site will be a combination of those two technologies.

### Making Any Changes

All changes are triggered automatically via Committing the changes. You can use the Github Editor or you can use git commands via your favorite tool. 

Changes trigger **Github Actions** - see the Actions Tab in the Repository Viewer, and can take between 3 and 15 minutes to publish to the mainsite. You can track the progress of a change by looking at the most recent Action after a Commit. 

### Adding a New Page

To create a new "main page" on the site (one that appears in the left navigation) you will create a new markdown file in the `docs` folder. 

Each new file **must** be named with a `.md` extension and **must start** with a [Font-Matter](https://jekyllrb.com/docs/front-matter/) such as

```
---
layout: page
title: My Unique Page Name
nav_oder: 7
---

Ipsum Lorem Content of my unique page in Markdown and Liquid mixed
```
- **title** is the unique name that will appear in the left-hand-navigation, do not use a title that has already been used
- **nav_order** dictates the order in which this link will appear in the left-navigation

### Creating Blog Posts on the Main Page Feed

To create a new post on the "what's new" feed, you will create a new markdown file in the `_posts` folder. 

Each new file **must** be named `YYYY-MM-DD-mypost-title.md` and the post will not be visible on the site until the specificed date. 

The post **must start** with a [Font-Matter](https://jekyllrb.com/docs/front-matter/) such as

```
---
layout: post
title:  My Post Title
---

Ipsum Lorem Content of my new post in Markdown and Liquid mixed
```

If you want you can use the `_drafts` folder to preview your blog posts and then move your file to `_posts` when it is ready, but typically you would only do that if you are going to work on a post for a long period of time and is usually unnecessary for the kinds of posts we tend to make.

### Changing the Main Site Page

The main `Home` page is controlled by `index.md`  

### Creating new ideas in an existing Scouting Resource

Currently we support the following types of Scouting Resources:

  - activities
  - camping
  - games
  - recipes 
  - songs
  - skits

To add to one of those resources, you only need to create a new `.md` file in the corresponding resource directory (the one with a leading underscore in front of the resource type) and then follow match the formatting you see in other files in that directory. 

Resources get automatically indexed and are searchable as soon as you publish.

### Creating new types of Scouting Resources

To create a new type of resource would create a new `_myNewResource` folder, and a corresponding `myNewResource.md` file in the `docs` directory. Next you would edit the `_config.yaml` and in the 2 places where `collections:` are referenced create entries for your `myNewResource` so that the file gets indexed properly. 

The myNewResource.md **must start** with a [Font-Matter](https://jekyllrb.com/docs/front-matter/) and look like

```
---

layout: page
title: My New Resource
parent: Scouting Resources

---

Flintlock Favorite My New Resource

<ul>
{% for newResource in site.myNewResource %}
<li>
    <a href="{{ site.baseurl }}/{{ newResource.url }}">
        {{ newResource.name }}
    </a>
</li>
{% endfor %}
</ul>
```


## Getting Help

Feel free to reach out to any of the collaborators on this project to get help at any time for help. 





