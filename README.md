# Jagatamba Barmeri Furniture Website

Responsive Hindi furniture catalogue for Jagatamba Barmeri Furniture.

## Firebase setup
1. In `index.html`, replace `PASTE_YOUR_FIREBASE_WEB_API_KEY` with the Web API key from Firebase Console → Project settings → Your apps → Config.
2. Replace `ADD_SHOP_WHATSAPP_NUMBER` with the shop WhatsApp number in international format (India: 91 followed by the number, no plus or spaces).
3. Products load from Firestore collection `products`. Required fields: `name`, `category`, `description`, `price`, `imageUrl`.

## Hosting
In Firebase Console → Hosting, use the GitHub deployment setup to connect this repository. Select branch `main` and the repository root. Firebase's setup will create the deployment workflow and required repository secret.

## Firestore safety
Keep public catalogue access read-only. Do not allow unauthenticated users to write or delete product documents. Configure Firestore Rules for your product collection before launch.
