# Meryll's Humble Abode — Netlify website

A responsive, single-page property listing built with plain HTML and CSS. No build command or dependencies are required.

## Deploy to Netlify
1. Download and unzip this project.
2. Open Netlify and choose **Add new site → Deploy manually**.
3. Drag the unzipped project folder (the folder containing `index.html`) into the deploy area.

Alternatively, put these files in a Git repository and import that repository in Netlify. The publish directory is `.` and no build command is needed.

## Add the property photos
The page currently uses styled placeholders. Put your own image files in this folder and replace the matching placeholder `<div>` in `index.html` with an image, for example:

```html
<img src="/front-yard.jpg" alt="Front yard of the property" />
```

Then add this CSS rule to `styles.css`:

```css
.gallery-card img, .hero-image img {
  display: block;
  width: 100%;
  height: 100%;
  min-height: inherit;
  object-fit: cover;
  position: absolute;
  inset: 0;
}
```

Suggested photo filenames: `front-yard.jpg`, `living-room.jpg`, `kitchen.jpg`, `bedroom.jpg`, `backyard.jpg`. Use your own photos and accurate alt text.

## Before publishing
- The listing uses **₱550,000 PHP**, 3 bedrooms, 1 bathroom, living room, kitchen, and **1,200 sq ft** as provided. Confirm whether the area is floor area or lot area.
- The contact number is displayed exactly as supplied: `(230) 111-1997`. Verify the number and country code before publishing; the call button currently links to `tel:+2301111997`.
- Confirm property details and availability before accepting inquiries.
