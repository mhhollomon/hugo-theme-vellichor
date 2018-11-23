# HUGO blog theme by @mhhollomon

A free blog theme for [HUGO](https://gohugo.io/), with tags, archives, last posts... Using [Bulma CSS framework](https://bulma.io/).

based on the the [jeffprod theme](https://github.com/Tazeg/hugo-blog-jeffprod)

# Install

Install HUGO (<https://gohugo.io/>) then :

```
hugo new site myblog
cd myblog
git clone https://github.com/mhhollomon/hugo-theme-vellichor.git themes/vellichor
```
In the file `config.toml` add the lines :
```
theme = "vellichor"

[permalinks]
    post = "/:year/:filename"

[taxonomies]
    tag = "tags"
    archive = "archives"
```

### Write blog posts

```
hugo new post/my-first-post.md
```
And edit this new file `content/post/my-first-post.md`. You can use [HUGO shortcodes](https://gohugo.io/content-management/shortcodes/) and [Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

### Render

```
hugo server
```
Then go to <http://localhost:1313>

### Create the web site

```
hugo
```

All files to publish are in `public/` directory.

## Configuration

There are various settings in the config.toml that affect how pages are rendered. See the exampleSites/config.toml for a sample and further information.

|Variable|Section|Effect|
|--------|--------|-------|
|GoogleAnalytics|Site|If defined and non-blank, adds code to the header of all pages for Google Analytics|
|HeaderImage|Params|Sets the image used in the header of each page. (Optional) If the setting is missing, a colored band is used instead.|
|BlogWelcome|Params|Text to place just above the blog post listing. (Optional).|
|PostDateFormat|Params|Format for the date of the posting (Optional). Default format is "January 2, 2006". See hugo dou=cs for format details.|
|showReadTime|Params|Controls the display of reading time in the post listing. If absent or false, the reading time will not be displayed.|

<!--
# Donate

<https://en.jeffprod.com/donate/>
-->

# Credits

Background image by https://pixabay.com
