# Page Statistics and Registration Tracking

This website is a static HTML site. A static site cannot store visitor statistics by itself unless it is connected to an analytics service.

The website has been prepared for Google Analytics 4.

## What is already added
The `index.html` file includes tracking code for:

1. Page visits / page views
2. Registration button clicks
3. Direct Google Form link clicks
4. When a visitor scrolls to the registration section

## What you still need to do
1. Create a Google Analytics 4 property.
2. Copy the Measurement ID, for example `G-ABC1234567`.
3. Open `index.html`.
4. Find this line:

```js
window.AYONIC_GA_MEASUREMENT_ID = "G-XXXXXXXXXX";
```

5. Replace `G-XXXXXXXXXX` with your real Measurement ID.
6. Upload the website again.

## Important limitation
The Google Form is embedded inside the page using an iframe. Because it belongs to Google, the website cannot directly detect when someone clicks the Submit button inside the embedded form.

Completed registrations should be counted from:
- Google Forms responses
- The connected Google Sheets response file

The website can track people who visit the registration section and those who click the backup registration link.
