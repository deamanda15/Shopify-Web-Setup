# How to Implement Meta Ads Manager

This guide explains how to set up Meta Ads (Facebook & Instagram Ads), integrate the Meta Pixel with Shopify, set up Conversions API, and manage advertising campaigns to drive traffic and sales.

## Steps to Implement Meta Ads:

### 1. Set Up Meta Business Suite and Ads Manager
- Go to [business.facebook.com](https://business.facebook.com) and create a **Meta Business Account**.
- Link your business's **Facebook Page** and **Instagram Business Account**.
- Under Business Settings, navigate to **Ad Accounts** and click **Add** > **Create a new ad account**. Configure your currency (e.g., IDR) and timezone.

### 2. Connect Meta Pixel & Conversions API to Shopify
To accurately track ads performance, set up data tracking:
- In your Shopify Admin, go to the **App Store** and install the official **Facebook & Instagram** sales channel.
- Open the Facebook channel, connect your Meta Business Account, and select the correct Page and Ad Account.
- Under **Data sharing settings**, choose **Maximum** tracking. This automatically sets up both:
  *   **Meta Pixel**: Browser-side tracking for events (PageView, ViewContent, AddToCart, InitiateCheckout, Purchase).
  *   **Conversions API**: Server-side tracking to capture events bypassed by browser ad-blockers or iOS tracking limitations.

### 3. Verify Your Domain and Configure Aggregated Event Measurement
- In Meta Business Settings, go to **Brand Safety** > **Domains**.
- Add your domain (`dafanyascarf.id`) and verify it using one of the methods (DNS TXT record in Exabytes cPanel Zone Editor or HTML Meta Tag).
- Go to **Events Manager**, select your Pixel, and configure **Aggregated Event Measurement** to prioritize your conversion events (with the `Purchase` event set as the highest priority).

### 4. Create and Structure Ad Campaigns
Open Meta Ads Manager and create campaigns using a structured funnel:
- **TOFU (Top of Funnel) - Cold Audience**: Focus on awareness or traffic. Use broad targeting, lookalike audiences, or interest-based targeting (e.g., fashion, hijab, accessories).
- **MOFU (Middle of Funnel) - Warm Audience**: Target users who engaged with your social media or viewed products but didn't add to cart.
- **BOFU (Bottom of Funnel) - Hot Audience**: Create **Dynamic Product Ads (DPA)** to retarget users who added items to their cart but abandoned checkout, offering incentives like free shipping or discounts.

### 5. Monitor and Optimize Key Metrics
Regularly check your Ads Manager reporting dashboard:
- **ROAS (Return on Ad Spend)**: The primary metric for profitability.
- **CTR (Click-Through Rate - Link Clicks)**: Aim for >1.5% as an indicator of strong ad creatives.
- **CPC (Cost Per Click)**: Monitor bidding and traffic costs.
- **Frequency**: Ensure ads are not shown too many times to the same person to avoid ad fatigue.

---
**Next Topic:** [Create and Use Google My Business](create-and-use-google-my-business.md)

