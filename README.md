# MAISON — The Intelligent Wardrobe

A luxury-editorial wardrobe and outfit-styling web app (single page, no build step).

## How to run
Open `index.html` in any modern browser (Chrome, Edge, Safari, Firefox). An internet connection is only needed for the Google Fonts; everything else works offline.

## Features
- Overview, My Wardrobe (search, filters, sorting), Add New Piece, Outfit Studio, Style Calendar, Weather & Style, Color Studio, Saved Looks, Insights, Settings
- Outfit Studio: occasion (College, Party, Date Night, Casual, Work, Evening, Weekend, Travel, Festive), weather, style, colour and dress-code controls; Generate, Refresh, Save, Replace Item; compatibility score and explanation
- Add New Piece: upload a photo and the colour, category, name, dress code and warmth are filled in automatically (works in three levels: offline colour and shape analysis always runs first; with internet, an on-device image model (TensorFlow.js MobileNet, about 15 MB downloaded on first use) identifies the garment type; inside Claude, a Claude vision step gives the best result)
- Color Studio: colour harmonies, recommended pieces, and a personal "Suits you" score from your skin and hair tone
- Insights: category and colour distribution, most used pieces, favourite combinations (pure SVG/CSS charts)
- Light/dark appearance, toast notifications, responsive layout (desktop to mobile)

## Technology
HTML, CSS and vanilla JavaScript in one file. Data is stored in the browser (localStorage). No backend.

## Moving your photos into this copy
Browser storage is separate for every copy of the app. In the Claude-hosted app open **Settings → Save backup (.json)**, then in this copy open **Settings → Load a backup** and choose that file. All uploaded photos come across.

## Photos
The wardrobe ships pre-loaded with 49 uploaded pieces (tops, bottoms, coats, dresses, shoes, accessories); the same images are in `photos/`.

## Photos (export)
`photos/` is where the wardrobe photos go. In the app, open **Settings → Download wardrobe & photos (.zip)** to export every photo you uploaded plus `wardrobe.json`, then copy them into this folder before submitting.

## Notes
- Demo pieces are illustrations; real photographs appear once you upload your own.
- Browser storage is per browser, so a fresh browser starts with the demo wardrobe.
