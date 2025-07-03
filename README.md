# Hugo PaperMod Theme Customizations

This repository contains a customized setup of the Hugo PaperMod theme. The following files have been modified or added to override the default theme behavior.

## `hugo.yaml`

The `hugo.yaml` file has been configured to set various site-wide parameters.

-   **`homeInfoParams`**:
    -   Includes a welcoming title with a waving hand animation: `"Hi there <span class='wave'>👋🏻</span>"`.
-   **`cover`**:
    -   The `hiddenInList` option is set to `true` to hide the cover image on list pages and the homepage.

## `assets/`

The `assets/` directory contains custom CSS to override the theme's default styles.

-   **`assets/css/extended/theme-vars.css`**:
    -   Sets the main container width to `900px`.
    -   Defines a custom color palette for dark mode, overriding the default theme colors.
    -   Styles hyperlinks with a custom color and a hover effect.
    -   Adds a custom background style for highlighted text using `<mark>` tags.
    -   Sets a custom color for inline code snippets.
    -   Includes a `wave-animation` for the waving hand emoji in the site's title.

## `layouts/`

The `layouts/` directory contains custom layouts and shortcodes to override the theme's default templates.

-   **`layouts/_default/_markup/render-link.html`**:
    -   This file overrides the default link rendering to open external links and PDF files in a new tab.

-   **`layouts/partials/extend_footer.html`**:
    -   This file adds a custom footer to the site.

-   **`layouts/partials/extend_head.html`**:
    -   This file can be used to add custom HTML to the `<head>` section of the site, such as Google Analytics scripts.

-   **`layouts/shortcodes/gallery.html`**:
    -   This shortcode creates a responsive image gallery from a specified directory.
    -   To use it, create a folder (e.g., `gallery/`) inside the `content/` directory and add your images.
    -   In your Markdown file, use the shortcode `{{< gallery dir="gallery/" >}}` to display the images.
