# Mohammad Mustafa Khan — Portfolio

Static HTML/CSS/JS portfolio generated from the supplied CV and LinkedIn profile PDF.

## Files
- `index.html` — website
- `styles.css` — responsive styling
- `script.js` — mobile navigation

## AWS S3 static hosting
1. Create an S3 bucket with a globally unique name.
2. Upload `index.html`, `styles.css`, and `script.js` to the bucket root.
3. For simple public website hosting, enable Static website hosting and set `index.html` as the index document.
4. Configure the required bucket policy/public access according to your AWS account's security settings.
5. Open the S3 website endpoint.

For production, a better AWS architecture is S3 + CloudFront + HTTPS (ACM certificate) rather than exposing the S3 website endpoint directly.

## Notes
- No external JavaScript libraries are required.
- The LinkedIn button points to the public profile URL supplied in the source document.
- Contact details are displayed because they were present in the supplied CV/profile documents.
