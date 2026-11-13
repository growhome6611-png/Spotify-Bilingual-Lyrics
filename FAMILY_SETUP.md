# Spotify Bilingual Lyrics — Family Edition V14.0 (5 users)

## What this version includes

This is a private-family deployment guide and in-app onboarding panel built on V13.9. Existing music, Chinese lookup, Pinyin, translations and vocabulary functionality remain in place. This version does **not** add a backend, a five-seat licensing system, a shared family account, or server-side user isolation.

## Owner setup

1. Deploy the contents of this folder to your existing GitHub repository / Vercel project (HTTPS).
2. In Spotify Developer Dashboard, confirm the app's allowed-user list and add up to the current Development Mode limit, **including the owner**. Spotify rules can change; check the dashboard for current eligibility and limits.
3. Set the correct Redirect URI in Spotify Developer Dashboard. The app displays its expected Redirect URI in Settings.
4. Configure Google Cloud OAuth authorized JavaScript origins for the exact HTTPS domain. Enable Drive API if Drive sync is required. For a Google OAuth app in Testing, add relevant test users as required.
5. Never publish a Spotify Client Secret or unrestricted paid API key in the repository. Spotify OAuth here uses PKCE. Translation API keys entered into the current frontend are visible to the browser and should be tightly restricted by origin and API quota; a server-side proxy is needed for robust secret protection.
6. Send the exact Vercel URL to the family members.

## Each family member

1. Open the HTTPS link on their own phone, computer or separate browser profile.
2. Connect their **own** Spotify account. Spotify Web Playback may require Premium and supported device/browser.
3. Connect their **own** Google account to Drive if they want sync.
4. Keep vocabulary and translation data separate by not sharing the same browser profile. Browser localStorage is origin-scoped and is **not** currently partitioned by Spotify account.
5. Before switching accounts on the same browser profile, export vocabulary and verify Drive sync. Do not assume disconnecting Spotify automatically deletes or separates saved vocabulary.

## Important limitations

- Five Spotify users are not five independent application accounts. The app currently has no backend authentication or access-control list of its own. Anyone with the URL can open the public frontend, but Spotify API access remains subject to Spotify authorization.
- Google Drive is linked by the Google account selected in the OAuth flow. Verify the selected account before uploading.
- A user switching Spotify accounts in the same browser profile can still see local browser data from the prior user. Separate profiles/devices are recommended.
- No live Spotify, Google OAuth or real-device integration test was possible in this package. Test each family member's account after deployment.
- Do not distribute copyrighted lyrics, recordings or translations without checking applicable rights and platform terms.
