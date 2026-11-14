# V14.9 - Google Drive Shared Lyrics Library

- Added shared folder URL entry in Settings > Google Drive Sync.
- Owner: the existing Spotify Bilingual Lyrics folder remains the single destination for individual and bulk translation uploads and downloads. Copy its Drive link and grant viewers access in Google Drive.
- Recipient: connect a Google account, paste the shared folder link, and use 'Tai ban con thieu' (download missing) to import translation records not yet on the device. Shared mode is read-only to avoid unintended overwrites.
- Incremental comparison remains in place; existing local records are never overwritten by a shared folder import.
- Return to the personal library with one click.
- Google OAuth now requests drive.file plus drive.readonly. The extra sensitive scope can require OAuth consent-screen configuration, test-user access, and Google verification for public distribution. Existing sessions must disconnect/reconnect to grant it.
- Spotify playback, local music, Pinyin, dictionary, exercises remain in the source.

Limitations: Shared-folder access depends on the Google account's actual sharing permission and Google API OAuth consent. A pasted URL alone does not grant access. The shared library imports translations; it does not automatically publish MP3 recordings or complete lyric-source files. Conflicting local translations are preserved, not overwritten. Sharing copyrighted lyrics and translations with others requires the appropriate rights.

QA: JavaScript syntax and ZIP archive integrity checked. Google Drive live authorization and cross-account behavior not tested in this environment.
