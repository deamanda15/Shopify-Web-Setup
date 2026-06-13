# How to Link a Domain: Exabytes to Shopify

This guide explains how I implemented the domain `dafanyascarf.id` from Exabytes to Shopify. I chose Exabytes because the pricing for domain registration and hosting is affordable, and it's easy to transfer the domain to various websites based on the company's needs. I purchased both the hosting and domain package at Exabytes.

## Steps to Link the Domain:

### 1. Login to Exabytes and Access cPanel
- First, log in to your Exabytes account, select **Layanan** in the top menu, and click on **Layanan Saya**.

![Login Exabytes](assets/images/how%20to%20linked-pict%201.png)

### 2. Access cPanel via Quick Shortcuts
- Under the **Detail Produk** page, you will see your active cPanel Hosting service. Scroll down to the **Quick Shortcuts** section and click on **Akun Email** (or any other shortcut) to be automatically logged into your **cPanel** dashboard.

![Quick Shortcuts cPanel](assets/images/how%20to%20linked-pict%202.png)

### 3. Scroll Down and Click on Zone Editor
- Once inside the cPanel dashboard, scroll down to the **Domains** section and click on **Zone Editor**.

![Zone Editor cPanel](assets/images/how%20to%20linked-pict%203.png)

### 4. Redirect Domain to Shopify (Configure DNS Records)
- Inside the Zone Editor, click **Manage** next to your domain (`dafanyascarf.id`).
- Add or edit the following records to direct your domain to Shopify:
  - **A Record**: Point the host name `@` (or `dafanyascarf.id.`) to Shopify's IP address: `23.227.38.65`.
  - **CNAME Record**: Point the host name `www` to `shops.myshopify.com`.

![cPanel DNS Records](assets/images/how%20to%20linked-pict%204.png)

### 5. Verify Domain in Shopify
- Go to your Shopify Admin page.
- Navigate to **Settings** > **Domains**.
- Click **Connect existing domain**, enter your domain name (`dafanyascarf.id`), and click **Verify connection**.

---
**Next Topic:** [How to Subscribe to Shopify](how-to-subscribe-shopify.md)


