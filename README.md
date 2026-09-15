# PDFWALA

A distinct, single-page PDF utility website inspired by the category structure of online PDF suites, but with original branding/UI.

## Files
- `index.html` — complete single-file HTML entry point
- `style.css` — standalone styling
- `app.js` — tool catalog, UPI modal, demo payment state, and browser-side tools
- `upi-qr.jpg` — the UPI QR image supplied for this project

## Run
Open `index.html` in a modern browser. An internet connection is needed for the CDN libraries/fonts in this demo.

## Currently functional in the browser
- JPG/PNG images → PDF
- Merge PDF files
- ₹2 UPI payment modal using the supplied QR / UPI deep link
- Tool search, categories, responsive layout, drag/drop UI

## Important production note
The "I have paid ₹2" button is only a demo unlock. Never trust a browser-only flag to confirm payment.

For real instant payment verification, use a server-side payment provider/API or your bank/UPI-compatible merchant integration:
1. Create a payment/order on the server for exactly ₹2.
2. Show the provider's UPI/QR/intent flow.
3. Verify the transaction/order signature/status on the server.
4. Only after verified payment, issue a short-lived processing token.
5. Process the uploaded file server-side and delete temporary files according to your retention policy.

Office conversions, OCR, PDF-to-JPG, repair, AI summarization/translation, signatures, etc. require additional browser libraries or backend services. The UI cards are already included so the backend can be connected without redesigning the site.

## Branding
The website is called PDFWALA and uses an original visual design. It is not a copy of iLovePDF's code, logo, text, or visual assets.
