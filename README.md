# Hugo PaperMod Theme Customizations

This repository contains a customized setup of the Hugo PaperMod theme. The following files have been modified or added to override the default theme behavior.

## `hugo.yaml`

The `hugo.yaml` file has been configured to set various site-wide parameters.

## `assets/`

The `assets/` directory contains custom CSS to override the theme's default styles.

-   **`assets/css/extended/theme-vars.css`**:
    -   Sets the `--main-width` to `900px`.

## `layouts/`

The `layouts/` directory contains custom layouts and shortcodes to override the theme's default templates.

-   **`layouts/_default/_markup/render-link.html`**:
    -   This file overrides the default link rendering to open external links and PDF files in a new tab.

-   **`layouts/partials/extend_footer.html`**:
    -   This file adds a custom footer to the site.

-   **`layouts/partials/extend_head.html`**:
    -   This file can be used to add custom HTML to the `<head>` section of the site, such as Google Analytics scripts.
