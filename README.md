# Gossitech presentation website

A responsive ecommerce presentation for Gossitech. Product details, prices, availability and stock are illustrative; confirm exact models, current stock, prices and delivery costs with the store.

## Run locally

Open `index.html` in a browser. No package installation, backend, build step or environment variables are required. To serve it locally, run `python -m http.server 8000` from this folder, then visit `http://localhost:8000`.

## Pages

Home, shop/catalogue, product details, wishlist, cart, quote checkout and confirmation, About, Contact, account concept, and store dashboard (`#admin`).

## WhatsApp quote requests

When the customer submits the quote form, the site prepares a WhatsApp message addressed to **+255 618 340 137** and opens WhatsApp with the order details filled in. The customer must review and press **Send** in WhatsApp. The site cannot silently send a message. For automatic server-side sending, the live store would need a backend connected to the WhatsApp Business Platform/API.

The quote request is also saved in localStorage for this browser and displayed on the dashboard. Contact and newsletter forms are not connected to a server. Payment credentials are never requested, and payment is not collected.

## Assets and deployment

The catalogue uses 15 locally stored Unsplash stock photos and three custom illustrations for the desktop, USB-C hub, and cooling pad. Photos are representative images, not confirmed Gossitech inventory or exact model photos. Sources are listed in `assets/IMAGE_SOURCES.md`; see the [Unsplash License](https://unsplash.com/license).

Publish this folder as a static website on Vercel, GitHub Pages, or another static host. No environment variables are needed. This frontend does not include production order storage, account security, payment processing, or automated WhatsApp API integration.
