# Setting CSS Sections and Layouts in Shopify

This guide explains how to configure theme sections, utilize custom CSS/Liquid blocks, manage color schemes, and assign templates in Shopify.

## Steps to Customize Sections and CSS:

### 1. Configure Color Schemes for Sections
- In the Shopify Theme Customizer, select any section (e.g., the **Header**).
- In the section settings panel on the right, you can change the **Color scheme** (e.g., choosing **Scheme 8**). 
- Clicking **Edit** under the selected scheme allows you to customize the background, text, and button colors globally for that scheme.

![Selecting Color Scheme](assets/images/setting%20css%20section%20-%20pict%201.png)
![Header Alignment Settings](assets/images/setting%20css%20section%20-%20pict%202.png)

### 2. Access Global Theme Settings
- Click the gear icon (**Theme settings**) in the left panel.
- This panel allows you to customize global styles such as **Logo**, **Colors**, **Typography**, **Layout**, **Animations**, **Buttons**, and **Dropdowns and pop-ups**.

![Global Theme Settings](assets/images/setting%20css%20section%20-%20pict%203.png)

### 3. Build Page Layouts with Sections
- In the left sidebar under the **Template** area, you can view the hierarchy of sections on your page (e.g., **Slideshow**, **Rich text**, **Featured collection**, **Image banner**).
- Rearrange these sections by dragging them, or toggle their visibility using the eye icon.

![Page Section Layout](assets/images/setting%20css%20section%20-%20pict%204.png)

### 4. Write Custom CSS via Custom Liquid Block
- If you need custom styling that the theme settings don't support, add a **Custom Liquid** section:
  - Click **Add section** and select **Custom Liquid**.
  - On the right panel, write a `<style>` block containing your custom CSS. For example, to adjust a video element's size and positioning:
    ```html
    <style>
    video {
      display: block;
      margin: 0 auto;
      width: 100%;
      height: 50%;
    }
    </style>
    ```

![Add Section & Custom CSS Liquid](assets/images/setting%20css%20section%20-%20pict%205.png)

### 5. Create and Configure Product Templates
- Navigate to the page dropdown at the top center of the customizer and select **Products** > **Create template** (e.g., creating a custom product template named `disclaimer-and-info`).
- Customize the product template:
  - Add specific product info sections, adjusting the desktop media width (e.g., Large), image zoom options, and section padding (e.g., Top: 36px, Bottom: 12px).
  - Add custom blocks like a **Rich text** disclaimer section or a features list block (e.g., **SS Feature #1**).

![Product Template Customizer](assets/images/setting%20css%20section%20-%20pict%206.png)
![Custom Product Disclaimer & Size Chart](assets/images/setting%20css%20section%20-%20pict%207.png)

### 6. Purchase or Import Pre-designed Sections
- If you want advanced sections without writing code, use the **Section Store** app from the Shopify App Store.
- The app offers various ready-to-use sections (e.g., Testimonials, Product Tabs, Scrolling logo clouds) that you can buy and add directly to your theme library.

![Shopify Section Store App](assets/images/setting%20css%20section%20-%20pict%208.png)

### 7. Assign the Custom Template to Products
- Go back to the main Shopify Admin dashboard.
- Go to **Products** and click on the product you want to modify.
- On the product details page, scroll down to the **Online Store** section on the right.
- In the **Theme template** dropdown, select your newly created custom template (e.g., `disclaimer-and-info`).
- Save the changes to apply the custom layout to that product.

![Select Product Page Template](assets/images/setting%20css%20section%20-%20pict%209.png)
![Product Page Template assigned](assets/images/setting%20css%20section%20-%20pict%2010.png)
![Assigning Template in Shopify Product Admin](assets/images/setting%20css%20section%20-%20pict%2011.png)

---
**Next Topic:** [Customizing Sections with HTML](custom-section-with-html.md)

