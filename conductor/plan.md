# Implementation Plan: Surfboard Portfolio Site

## Objective
Create a minimalist, single-page Nuxt site to showcase a surfboard for sale, featuring its specifications, condition, included accessories, and a photo gallery.

## Key Files & Context
- `nuxt.config.ts` & `package.json`: Need updating to include `@nuxtjs/tailwindcss`.
- `app/app.vue`: Will be the main and only component for this single-page site.
- `public/`: Contains all the product images.

## Implementation Steps
1. **Setup Tailwind CSS:**
   - Install `@nuxtjs/tailwindcss` via npm.
   - Add `@nuxtjs/tailwindcss` to the `modules` array in `nuxt.config.ts`.
2. **Develop the Landing Page (`app/app.vue`):**
   - Create a clean, "sober" layout utilizing plenty of whitespace, simple typography (sans-serif), and a neutral color palette.
   - **Header Section:** Title ("Surfboard for Sale"), dimensions, and price.
   - **Details Section:** Specifications, included accessories, and condition report (translated to English).
   - **Gallery Section:** A responsive CSS grid to display the images from the `public` folder.
3. **Content Draft (English):**
   - **Dimensions:** 6'2" - 21" - 2 5/8" - 36L
   - **Fin Setup:** Thruster (3 fins)
   - **Accessories Included:** 3 Futures Honeycomb fins + Dakine leash.
   - **Condition:** Ridden for approximately 30 sessions. Purchased in 2023 and carefully stored since. Shows normal deck pressures and a compression mark on the top rail.
   - **Price:** Rp 5,000,000 (All included).

## Verification & Testing
- Run `npm run dev` to verify the site renders correctly.
- Ensure all images load properly from the `public` folder.
- Confirm the layout is responsive on mobile and desktop views using Tailwind's responsive classes.
