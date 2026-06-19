# Aureveil Studios Project Update

Last updated: 19 June 2026

## Positioning

Aureveil Studios is a premium digital wedding invitation brand. The product should be positioned as a mobile-first interactive wedding microsite, not as a cheap downloadable card.

Core offer:

> A mobile-first interactive wedding invitation with cinematic opening, music, countdown, map, RSVP, and WhatsApp sharing.

## Architecture

```text
Shopify = storefront, checkout, payment, product options, order collection
External card system = hosted interactive invitation experience
```

Shopify should handle commerce and order collection. The card system should handle the guest-facing invitation link, RSVP, music, animation, countdown, maps, guest personalization, and shareable final URL.

## Recommended Stack

- Shopify for storefront and checkout
- Next.js / React for interactive cards
- Vercel, Netlify, or Cloudflare Pages for hosting
- Supabase or Firebase for RSVP and card data
- Cloudinary or Supabase Storage for uploaded media

## Product Packages

| Package | Price Range | Includes | Revisions |
|---|---:|---|---:|
| Basic | RM49-RM89 | 1-page interactive card, names, date, venue, map, WhatsApp share | 1 |
| Standard | RM99-RM199 | Basic + music, countdown, RSVP, photo section | 2 |
| Premium | RM249-RM499 | Standard + guest-name personalization, multi-language, custom colors, RSVP export | 3 |

Strongest starting offer:

> RM149 interactive wedding card with music, countdown, map, RSVP, and WhatsApp sharing.

## First Templates

1. Minimal Luxury
2. Malay Elegant
3. Chinese Banquet
4. Floral Pastel
5. Dark Cinematic

Dark Cinematic should lead as the brand signature. Minimal Luxury should remain the safer conversion option.

## Core Interaction Requirements

- Tap-to-open opening screen
- Soft animation after tap
- Music starts only after user interaction
- Horizontal swipe navigation
- Couple names and wedding date
- Countdown
- Invitation message
- Event details
- Google Maps button
- RSVP section
- Gallery/photo reveal
- WhatsApp share button
- Optional gift/bank transfer section

## Data Model Direction

Cards should be generated from structured data, not hardcoded content.

```json
{
  "template": "minimal-luxury",
  "brideName": "Alya",
  "groomName": "Adam",
  "date": "2026-08-22",
  "time": "7:30 PM",
  "venueName": "The Majestic Hotel Kuala Lumpur",
  "venueAddress": "Kuala Lumpur",
  "mapLink": "https://maps.google.com/...",
  "music": "soft-piano.mp3",
  "language": "en",
  "themeColor": "champagne",
  "rsvpEnabled": true,
  "whatsappNumber": "60123456789",
  "gallery": ["photo1.jpg", "photo2.jpg"]
}
```

## Manual Fulfillment Workflow

1. Check payment
2. Check submitted details
3. Message customer if information is incomplete
4. Duplicate chosen template
5. Insert customer data
6. Upload photos
7. Configure RSVP
8. Generate preview link
9. Send preview
10. Collect revision
11. Finalize
12. Send final link
13. Mark completed

## Near-Term Priorities

1. Finalize package names, prices, features, revision rules, and delivery promises.
2. Build one polished interactive demo first.
3. Create Shopify product page draft.
4. Build customer personalization form.
5. Create manual order tracker.
6. Test one full order manually from purchase to delivery.
7. Record short demo videos for social proof.
8. Soft launch with beta pricing.

## Working Principle

Do not build a full editor yet. Start with a limited self-serve ordering flow and semi-manual fulfillment. Validate demand, pricing, fulfillment complexity, and template appeal before investing in full automation.
