# :mega: Hunter's Bot Guide

@» Staff ღ 
Hello team! The Hunter's bot helps manage reservations and table status. Here's a quick guide:

### Commands (Requires staff role)
- `/table-status [date:<dd-mm-yyyy>]` — Show table status
- `/accept-restaurant username:<name>` — Accept and assign table
- `/decline-restaurant username:<name>` — Decline reservation
- `/accept-hotel` / `/decline-hotel` — Hotel reservations
- `/assign-table` — Assign waiter (modal)
- `/new-reservation` — Walk-in booking
- `/cleanup-reservations` — Admin: clear old entries

**Note:** Use dd-mm-yyyy format. Bot runs on UTC.

## Web Interface

### Staff Pages
- **Cashier** (`/restaurant-cashier.html`): Orders, receipts, inventory
- **Inventory** (`/inventory.html`): Stock management
- **Admin** (`/admin.html`): Staff login

### Technical
```javascript
const config = {
  projectId: "hunter-s-2e810",
  apiKey: "AIzaSyAK-baJsRLyBp8EFmtWFqOmjTxjALTRl6Q"
};
```

### Features
- Firestore inventory tracking
- Discord webhooks for receipts/alerts
- Ingredient-level stock management
- Low-stock alerts (<=20 units)
- Secure staff pages