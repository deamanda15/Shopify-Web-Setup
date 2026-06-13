# Customizing Shopify Sections with HTML and Liquid

This guide explains how to back up your theme, manage media assets, add Custom Liquid/HTML blocks, and configure payment providers to support custom storefront designs.

## Steps for Custom HTML and Code Customizations:

### 1. Create a Theme Backup
- Before modifying theme code or adding custom HTML structures, it is critical to back up your theme.
- Go to **Online Store** > **Themes**.
- Click the three dots `...` next to your active theme (e.g., *Edited 17/01*) and click **Duplicate**. This creates a backup copy (e.g., *Copy of Edited 17/01*) in your Theme library.

![Theme Backup and Library](assets/images/custom%20section%20with%20HTML%20-%20pict%201.png)

### 2. Add Custom Liquid/HTML Section
- Open the Theme Customizer.
- Click **Add section** in the left sidebar, scroll down, and select **Custom Liquid**.

![Adding Custom Liquid Section](assets/images/custom%20section%20with%20HTML%20-%20pict%202.png)

### 3. Upload Media Assets to Shopify CDN
- To use custom images or videos in your HTML/Liquid sections, upload them to Shopify first:
  - Go to Shopify Admin > **Content** > **Files**.
  - Click **Upload files** and select your assets (e.g., product images, promotional videos).
  - Copy the generated URL link to use directly inside your custom code.

![Shopify Files CDN Manager](assets/images/custom%20section%20with%20HTML%20-%20pict%203.png)

### 4. Write Custom HTML and Styling
- Select the **Custom Liquid** section you added.
- In the right-hand settings panel under **Liquid code**, write your HTML and CSS:
  - Add `<style>` tags to define custom styles (e.g., adjusting the responsive layout of a video player).
  - Use HTML tags like `<video>` with the CDN link copied from the files manager.
  - Example code for autoplaying banner video:
    ```html
    <style>
    video {
      display: block;
      margin: 0 auto;
      width: 100%;
      height: 50%;
    }
    </style>

    <video controls autoplay loop playsinline muted>
      <source src="https://cdn.shopify.com/...your-video-url.mp4" type="video/mp4">
    </video>
    ```
- Use the **Custom CSS** text box at the bottom right to apply additional fine-grained CSS rules (e.g., `h2 { font-size: 32px; }`).

![Custom Liquid Block & Custom CSS](assets/images/custom%20section%20with%20HTML%20-%20pict%204.png)

### 5. Verify Store Payments Setup
- For checkout custom HTML or testing checkout functionality, make sure your payment provider is configured.
- Go to **Settings** > **Payments**.
- You can activate payment methods like **PayPal** or third-party gateways (e.g., **Midtrans** for card and local bank payments in Indonesia).
- Choose a **Payment capture method** (e.g., set to **Manually** or **Automatically at checkout**).

![Shopify Payments Settings](assets/images/custom%20section%20with%20HTML%20-%20pict%205.png)

---
**Next Topic:** [Setting Hard-Selling Pop-up](setting-hardselling-pop-up.md)

