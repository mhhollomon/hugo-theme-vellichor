# Vellichor HUGO blog theme

A free customizable blog theme for [HUGO](https://gohugo.io/) using [Bulma CSS framework](https://bulma.io/).

- Reactive
- Display Recent posts
- Display tags
- Display archives
- Custom top navigation
- Custom footer information
- Custom styling

Based on the the [jeffprod theme](https://github.com/Tazeg/hugo-blog-jeffprod)


# Installation

Follow the themes guide on the Hugo website. Briefly, within your Hugo site directory:

```
$ git submodule add https://github.com/mhhollomon/hugo-theme-vellichor themes/hugo-theme-vellichor
```

This will add the theme under the themes directory. Then copy the example `config.toml` to see all the configration options.

```
$ cp themes/hugo-them-vellichor/exampleSite/config.toml .
```

See below for configuration options.

### Write blog posts

```
hugo new post/my-first-post.md
```

And edit this new file `content/post/my-first-post.md`. You can use [Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) and [HUGO shortcodes](https://gohugo.io/content-management/shortcodes/) 


# Configuration

THe vellichor theme has quite a few ways to customize it. Just as a sample you can:

- change the image in the header.
- Control which social media links are displayed.
- Customize the links at the top.

Please see the following two places for more information.
- exampleSite/config.toml has descriptions and examples of most of the
  settings.
- The [Configuration How-to](CONFIGURATION.md) has more detailed information on other ways to customize the theme.


# License

Licensed under the MIT license.

# Credits

- Background image from [pixabay](https://pixabay.com).
- [Original jeffprod theme](https://github.com/Tazeg/hugo-blog-jeffprod).
- [Font Awsome](https://fontawesome.com/) icons.
