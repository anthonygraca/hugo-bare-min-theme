The **Bare Min** theme is heavily inspired from [the better
mother-loving website](http://bettermotherfuckingwebsite.com/).

It was designed to:

-   Get rid of all visual clutter (CSS, JS, etc.)
-   Allow easily seeing debug information ([`debugprint.html`
    partial](https://github.com/kaushalmodi/hugo-bare-min-theme/blob/master/layouts/partials/debugprint.html))
    while developing Hugo sites, where focus stays on content
    development.

[![Bare Min Theme
Screenshot](https://raw.githubusercontent.com/kaushalmodi/hugo-bare-min-theme/master/images/screenshot.png)](https://ox-hugo.scripter.co/test/posts/keyword-collection/)

This theme is being used by:

1.  The [test site](https://ox-hugo.scripter.co/test/) for
    [`ox-hugo`](https://ox-hugo.scripter.co/).
2.  Unofficial [Hugo Sandbox](https://hugo-sandbox.netlify.com/) site
    that is used to create test cases for `hugo` bugs, new feature
    requests, and testing `hugo` features in general.

## Configuration options

These theme provides few customization hooks.

```toml
# In the site's config.toml

[Params]
  description = "Description of the site."
  intro = """
Text here is added to the header of each page.

This can contain <b>HTML</b> and/or **Markdown**
and can be multiple lines.
"""
  footer = """
Text here is added to the footer of each page.

This can contain <b>HTML</b> and/or **Markdown**
and can be multiple lines.
"""
  [Params.source]
    url = "https://your/site/repo/url" # Mandatory, used in bare_min single.html, baseof.html
    md_dir = "content" # Used to create links from pages to the page Markdown sources
    org_dir = "content-org" # Optional, but use if using ox-hugo!
```

See the `Params` section in the [`ox-hugo` test site
`config.toml`](https://github.com/kaushalmodi/ox-hugo/blob/master/test/site/config.toml)
to get an example.