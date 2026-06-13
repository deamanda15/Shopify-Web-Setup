# Developing a Shopify Theme

This guide explains how to access the Shopify Code Editor to modify theme files directly, and provides an overview of the key folders within a standard Shopify theme structure (like the Dawn theme).

## Steps to Customize Theme Code:

### 1. Access the Shopify Code Editor
- In your Shopify Admin panel, navigate to **Sales channels** > **Online Store** > **Themes**.
- For your active theme (or any backup theme in your library), click the three-dots `...` action button next to the **Customize** button.
- Select **Edit code** from the dropdown menu. This will launch Shopify's web-based code editor interface.

![Accessing Edit Code option](assets/images/Screenshot%202025-03-08%20220204.png)

### 2. Understanding the Theme Directory Structure
Inside the code editor, your theme code is organized into several key folders:

#### A. Layout Folder
- Contains overall page shells (like `theme.liquid`). These files wrap all other pages and contain header scripts and base structure.

#### B. Templates Folder
- Contains JSON configurations that define which sections display on what page types (e.g. `index.json` for home page, `product.json` for product details).

#### C. Sections Folder
- Contains `.liquid` files that dictate the structure of reusable page segments (e.g., `announcement-bar.liquid`, `featured-collection.liquid`, `custom-liquid.liquid`).
- Developers add custom Liquid schema and HTML inside these files so store owners can customize them via the visual editor.

![Sections Directory](assets/images/Screenshot%202025-03-08%20220721.png)

#### D. Snippets Folder
- Contains smaller, reusable bits of Liquid/HTML (e.g. product cards or icon indicators) that can be included inside layout or section files using the `{% render 'snippet-name' %}` tag.

#### E. Assets Folder
- Contains stylesheets (`.css` files like `base.css` or component-specific styles like `section-main-product.css`) and Javascript files (`.js` files like `animations.js` or `cart.js`) that control frontend behavior.
- Developers upload icons and custom fonts here to render store assets dynamically.

![Assets Directory CSS Files](assets/images/Screenshot%202025-03-08%20220844.png)
![Assets Directory Base CSS](assets/images/Screenshot%202025-03-08%20220511.png)
