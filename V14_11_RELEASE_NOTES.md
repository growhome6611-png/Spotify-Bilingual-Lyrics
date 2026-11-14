# V14.11 - Unified Drive lyrics format

- Both 'Save current lyrics' buttons now call the same `exportLyricsDrive()` function.
- Canonical file is `<track>__<language>__lyrics.json` under the selected `Spotify Bilingual Lyrics` Drive folder; JSON schema includes `version`, `type`, `trackKey`, `language`, `song`, `savedAt`, `lyrics[]` with `time`, `text`, `pinyin`, `translation`.
- Drive library browser reads the same JSON files and restores lyrics/Pinyin/translations into the lyric display without requiring an MP3.
- Existing older music library manifests under `Thu vien nhac` remain readable.
- Shared read-only folder can be browsed; uploads still restricted to personal folder.
- This release does not migrate older files or merge conflicts automatically.
- Static JS syntax and ZIP integrity checked; live OAuth/Drive tests still needed.
