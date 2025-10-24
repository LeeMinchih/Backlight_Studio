Backlight Studio — Cloudflare Pages (pages.dev) build v4

What changed:
- Hero section now uses a full-width, muted, looping background video.
- The page looks for a file at /hero.mp4. Please upload your own MP4 (10–15s recommended, H.264/AAC).

How to update on Cloudflare Pages:
A) Replace only index.html (risky: other assets won't update)
   - In your Pages project → Deployments → Upload assets → upload just the new index.html.
   - WARNING: Each deployment is a full snapshot. If you upload only index.html,
     this new deployment will contain ONLY that file unless your dashboard supports merging.
     To be safe, prefer option B.

B) Upload a full package (recommended)
   - Upload this ZIP so all files stay in sync.
   - After deploy, go to "Settings → Assets" (or project root) and upload hero.mp4 to the root.

Add your hero video:
- Name your clip "hero.mp4" (H.264 baseline or main, 1920x1080 or 1280x720, < 10–20 MB).
- In the Pages dashboard, use "Upload assets" and drag hero.mp4 into the root along with index.html (or include it in your ZIP before uploading).
- The <video> tag includes poster=/og-cover.jpg for a graceful first frame.

