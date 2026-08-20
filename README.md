# Valentine-simple-web

A beautiful and interactive Valentine's Day webpage with language support (English/Chinese), plus a proposal page to ask someone to be your official girlfriend.

## Pages

- `index.html` — Will you be my Valentine?
- `proposal.html` — Will you be my official girlfriend? (photo collage background)

## Features

- 💕 Romantic and beautiful design with animated hearts
- 🌍 Multi-language support (English / ไทย / 中文 on the proposal page)
- 🎯 Interactive "Yes" and "No" buttons
- ✨ Celebration animation with confetti when "Yes" is clicked
- 🖼️ Polaroid photo collage background on the proposal page
- 🎨 Responsive design that works on all devices

## How to Use

Simply open `index.html` or `proposal.html` in your web browser, or serve it using a local web server:

```bash
python3 -m http.server 8000
```

Then visit:

- `http://localhost:8000` for the Valentine page
- `http://localhost:8000/proposal.html` for the girlfriend proposal page

You can personalize names with URL parameters:

```
proposal.html?name_from=Pawat&name_to=HerName
```

## Adding photos to the proposal page

1. Drop your pictures into the `photos/` folder.
2. Open `proposal.html` and update the `PHOTO_FILES` list near the top of the script with your filenames.

Until you add real photos, colorful placeholders fill the background collage.

## Languages

- English
- 中文 (Chinese)

Click the language buttons in the top-right corner to switch between languages.

## Special Features

- The "Yes" button grows larger each time "No" is clicked
- The "No" button moves around after multiple clicks (making it harder to click!)
- Beautiful confetti animation appears when "Yes" is finally clicked

Enjoy! 💖
