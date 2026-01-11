# Secure Digital Product Delivery (WooCommerce)
This project documents the professional setup for selling PDFs and digital assets securely.

## 🛡️ Security Features Implemented:
* **X-Accel-Redirect/X-Sendfile:** Configured to prevent direct URL access to files.
* **Link Expiration:** Set to 24 hours to prevent unauthorized link sharing.
* **Download Limits:** Restricted to 3 attempts per purchase.

## ⚙️ Technical Workflow:
1. **Payment:** User completes checkout via M-Pesa/Stripe.
2. **Verification:** Order status changes to 'Completed' via API Webhook.
3. **Delivery:** System generates a unique, encrypted hash for the file download.
4. **Notification:** Automated email/WhatsApp sends the secure link to the customer.

## 🛠️ Tools Used:
* WordPress + WooCommerce
* .htaccess (for directory protection)
* Advanced Product Downloads logic
