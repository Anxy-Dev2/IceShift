# IceShift — Hockey Development Lab

## Run locally
1. Extract the ZIP.
2. Open the folder containing `index.html`.
3. Click the File Explorer address bar, type `cmd`, press Enter.
4. Run `py -m http.server 8095`
5. Open `http://localhost:8095` in a browser.

Keep the terminal open while using the app.

## Features
- Redesigned dark navy / ice-blue development dashboard
- Weekly ODR training checklist
- Training, game and practice logs
- Skill ratings and a 7-day training chart
- Film room with YouTube embeds, jersey number, timestamps, notes and reference clip tagging
- Optional short local video upload, if browser storage permits
- JSON export and offline PWA caching

## Important film-analysis limitation
This is a local-first web app, not a video-understanding AI model. It can embed public YouTube videos and store your notes/short clips, but it cannot independently identify your jersey number, track your shifts, or infer hockey tactics from footage. For actual AI analysis, provide a short clip or screenshots to a video-capable assistant, ask for feedback on your jersey number and position, and paste the observations into the saved review. A production automated-analysis version would require a video analysis model/backend and appropriate API credentials.

## Storage and privacy
No account or server backend is used. Data is stored in this browser's local storage. Uploaded video is stored as browser data when possible and can fill browser storage quickly. Keep clips short, export JSON backups, and do not clear browser data if you want to keep your records. YouTube links require internet access. The service worker works on localhost or an HTTPS host, not by opening the HTML file directly.

## Install on phone
Publish the folder to an HTTPS static host (for example GitHub Pages), open the HTTPS URL on the phone, then use the browser's install/add-to-home-screen option. The local data on your PC does not automatically sync to your phone.
