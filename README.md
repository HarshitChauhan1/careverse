# CareVerse — GitHub-only MVP

A browser-based student prototype inspired by the CareVerse synopsis.

## Features in this MVP
- Responsive patient dashboard
- Rule-based symptom-to-specialty guidance with safety notices
- Local demo appointment booking, token numbers, cancellation
- Browser geolocation permission and external map search
- Demo health-wallet records with JSON export/delete
- Medicine reminder list (no background notifications)
- Admin analytics from browser-local data
- Local JSON export and demo-data reset

## Run using GitHub only
1. Open GitHub and create a new **public** repository named `careverse`.
2. On the repository page, choose **Add file → Upload files**.
3. Upload `index.html` and `README.md` from this folder, then commit.
4. Open **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select branch `main`, folder `/(root)`, and click **Save**.
7. Wait for the published URL to appear in Settings → Pages.

You can also use GitHub Codespaces: open the repo → Code → Codespaces → Create codespace. The static app can be previewed with the Codespaces port-forwarding preview, or use GitHub Pages for the shareable URL.

## Important limitations
This is a front-end MVP, not a production healthcare system.
- Uses browser `localStorage`; data is only in that browser/profile and does not sync between users/devices.
- No server, database, real login, access control, encryption, or cloud backup.
- Symptom guidance uses simple keyword rules; it is not a trained AI model or medical diagnosis.
- Doctor profiles, fees, ratings and appointments are demo data, not real providers or bookings.
- Emergency search opens a third-party map. It does not check hospital bed/ICU availability, route ambulances, or alert hospitals.
- Reminder entries do not trigger background push/SMS notifications.
- No real video consultation, payment, insurance processing, or hospital integration.
- Do not enter real patient data or sensitive health information.

## Suggested next development milestones
1. Build a backend API and real authentication.
2. Add a database and server-side validation.
3. Replace keyword rules with a properly evaluated, safety-reviewed model.
4. Integrate verified provider and hospital availability sources.
5. Add security/privacy review before handling real health data.
