### config.toml

There are various settings in the config.toml that affect how pages are rendered. See the exampleSites/config.toml for a sample and further information.

|Variable|Section|Effect|
|--------|--------|-------|
|copyright|Site|Copyright text placedin the footer (Optional). Contents of `author` used if copyright is missing|
|GoogleAnalytics|Site|If defined and non-blank, adds code to the header of all pages for Google Analytics|
|HeaderImage|Params|Sets the image used in the header of each page. (Optional) If the setting is missing, a colored band is used instead.|
|BlogWelcome|Params|Text to place just above the blog post listing. (Optional).|
|PostDateFormat|Params|Format for the date of the posting (Optional). Default format is "January 2, 2006". See hugo dou=cs for format details.|
|showReadTime|Params|Controls the display of reading time in the post listing. If absent or false, the reading time will not be displayed.|
|socialIconSize|Params|Controls the size of the social media icons in the footer. Must be one of `small`, `medium`, or `large`. `large` is the default|
|footerClass|Params|Controls the CSS style class to use to style the footer (text color, background color, etc).|
|github,twitter|Social|If an userid is specified for the service, the icon and link are placed in the footer. See config.toml for the list of currently supported services.|

### partials

The following partials can be copied from the theme directory into your site's `layout/partial` directory in order to customize.

```
cp themes/hugo-theme-vellichore/layouts/partial/<partial> ./layouts/partial
```

#### social.html

This controls the layout of the social media icons in the footer. It is used in all top level index types.

The list of services that are displayed can be controlled directly from `config.toml`

#### top-menu.html

This contains the list links that are shown in the top navigation bar.
