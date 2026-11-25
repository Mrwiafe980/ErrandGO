# ErrandGo: app builder prompt

Copy this into your app builder or developer brief.

> **Build a colorful, professional, ultra-simple mobile app called "ErrandGo" for Ghana, available on Android first (Flutter or React Native), with iOS to follow.** The app lets people post shopping lists (groceries, pharmacy, household items, market goods) and pay verified couriers to buy and deliver them to their doorstep. The design must be so simple that even a 5-year-old can navigate it: big rounded buttons, large friendly icons and emojis, one main action per screen, minimal text, voice input, and an animated friendly mascot guiding the user.
>
> **Visual style:** Bright, joyful and premium. Palette: sunshine yellow (#FFC93C), Ghana green (#1E9E5A), warm red (#E63946), deep trust blue (#1D3557), with soft white cards, generous spacing, rounded corners (24px), playful micro-animations (bouncing cart, ticking checkmarks, confetti on delivery) and a clean modern typeface (e.g. Poppins or Nunito). Include light and dark mode and accessibility support (large text, high contrast, screen reader labels).
>
> **Customer app screens:**
> 1. Onboarding with 3 illustrated slides and phone-number OTP login (Ghana +233).
> 2. Home with one huge button "What do you need?" plus quick category tiles (Groceries, Pharmacy, Market, Household, Anything).
> 3. List builder: add items by typing, voice, or photo; each item has a picture icon, +/− quantity, a note field and a brand preference. Allow saving favourite lists for reuse.
> 4. Shop picker: Google Map of Ghana with pins for malls and supermarkets (Accra Mall, West Hills Mall, Kumasi City Mall, Melcom, Shoprite, Game, Palace, Makola Market, Kaneshie Market, Kejetia Market), searchable by name, plus an "Any shop near me" option.
> 5. Order summary: itemized estimated cost, delivery fee, service fee, total, and a clear spending cap the customer can set.
> 6. Payments: MTN MoMo, Vodafone/Telecel Cash, AirtelTigo Money, card (Paystack or Flutterwave integration), and cash on delivery.
> 7. Live order tracking: real-time courier location on Google Maps with ETA, route line, and a progress bar (Accepted → Shopping → On the way → Delivered).
> 8. Per-item status: every item shows ⏳ waiting, ✅ picked (with price), or ❌ unavailable, and sends a push notification each time an item is picked. For unavailable items the customer gets a one-tap "Substitute / Skip" choice.
> 9. Receipt transparency: courier uploads a receipt photo per shop; the customer sees the receipt, actual prices, and any refund or top-up automatically calculated.
> 10. Chat and masked call with the courier, a delivery confirmation PIN or QR code, ratings and reviews, and a full order history with re-order in one tap.
>
> **Courier app screens:** Online/offline toggle, incoming errand requests with earnings preview, accept or decline, shop-by-shop checklist with tick-off and price entry, receipt camera upload, turn-by-turn navigation via Google Maps, proof of delivery, an earnings wallet with MoMo withdrawal, and rating history. Include courier verification (Ghana Card, selfie, guarantor details).
>
> **Admin dashboard (web):** Courier approval, live map of all active couriers, order management, dispute and refund handling, dynamic pricing (distance-based delivery fees), promo codes, analytics, and payout management.
>
> **Maps and location:** Google Maps SDK, Places API and Directions API, with live courier tracking (location updates every 5 to 10 seconds via Firebase or WebSockets). Map defaults to Ghana with Accra, Kumasi, Takoradi, Tamale and Cape Coast as quick-select cities. Support Ghana Post GPS digital addresses, dropped pins, and landmark notes for delivery. Optimize for patchy networks with caching and a low-data mode.
>
> **Tech:** Flutter or React Native frontend; Node.js or Firebase backend; PostgreSQL or Firestore; Firebase Cloud Messaging for push notifications and SMS fallback; secure payments; GDPR-style privacy with Ghana Data Protection Act compliance; English plus Twi, Ga, Ewe and Hausa language options.
>
> **Quality bar:** Fast, polished and trustworthy, like a top-tier delivery app, but simpler and friendlier. Deliver clean, well-structured code, reusable UI components, and a clickable prototype first.

## Tips before you build

1. **Start with an MVP**: one city (Accra), 3 to 4 malls or markets, MoMo payments, live tracking and per-item updates. Add the rest after real users test it.
2. **Handle price risk**: use a spending cap plus pre-authorization so couriers aren't out of pocket if prices differ.
3. **Safety**: verify couriers carefully and use the delivery PIN, because trust is your biggest selling point.
4. **Build in stages**: ask your AI builder for the design/prototype first, then the customer app, then the courier app, then the admin panel.
