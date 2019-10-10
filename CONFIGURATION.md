### config.toml

There are various settings in the config.toml that affect how pages are rendered. See the exampleSites/config.toml for a sample and further information.

|Variable|Section|Effect|
|--------|--------|-------|
|copyright|Site|Copyright text placedin the footer (Optional). Contents of `author` used if copyright is missing|
|googleAnalytics|Site|If defined and non-blank, adds code to the header of all pages for Google Analytics|
|headerImage|Params|Sets the image used in the header of each page. (Optional) If the setting is missing, a colored band is used instead.|
|blogWelcome|Params|Text to place just above the blog post listing. (Optional).|
|postDateFormat|Params|Format for the date of the posting (Optional). Default format is "January 2, 2006". See [hugo docs](https://gohugo.io/functions/format/#go-s-layout-string) for format details.|
|showReadTime|Params|Controls the display of reading time in the post listing. If absent or false, the reading time will not be displayed.|
|socialIconSize|Params|Controls the size of the social media icons in the footer. Must be one of `small`, `medium`, or `large`. `large` is the default|
|footerClass|Params|Controls the CSS style class to use to style the footer (text color, background color, etc).|
|openGraphImage|Link to image to place in the "og:image" metatag|
|github,linkedin,etc|Social|If an userid is specified for the service, the icon and link are placed in the footer. See config.toml for the list of currently supported services.|

### Menus

The menus underneath the hero banner can be modified via entries in the
config.toml file. There are three different menus, brand, topleft, and
topright.

See the [hugo menu docs](https://gohugo.io/variables/menus/#readout) for more info on configuring menus items.

#### brand menu

This is to the far left. By default, it will contain a "Home" and "About"
entry. IF any entires are present in the config.tml file, this will get
overriden. As an example, here is how to specify the default entries:

```toml
[menu]
    [[menu.brand]]
        identifier = "home"
        name = "Home"
        url = "/"
        weight = -110
    
    [[menu.brand]]
        identifier = "about"
        name = "About"
        url = "/about/"
        weight = -100
```

### topleft menu

Displayed just to the right of the brand menu. On a mobile platform, this will
be hidden behind a "hamburger".

This menu is empty by default.

### topright menu

Displayed against the right hand side of the header. By default it contains a
link to the RSS feed page.

### partials

The following partials can be copied from the theme directory into your site's `layout/partial` directory in order to customize.

```
cp themes/hugo-theme-vellichore/layouts/partial/<partial> ./layouts/partial
```

#### social.html

This controls the layout of the social media icons in the footer. It is used in
all top level index types.

The list of services that are displayed can be controlled directly from `config.toml`

### Comment Services

The theme knows about two comment services - Disqus, and utteranc.es.

If the parameter "disqusSHortName" is defined in the config.toml, thn the theme
will inject code to render the Disqus comment widget.

If the parameter `utterances` is defined in the `params` section, then the thme
will inject code to display the utteranc.es comment widget.
