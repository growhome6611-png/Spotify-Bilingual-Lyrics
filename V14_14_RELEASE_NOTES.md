# V14.14 - Batch JSON to extended LRC

- New button in Local Music > Google Drive: Chuyen JSON sang LRC hang loat.
- Reads JSON from Spotify Bilingual Lyrics folder, joins Vietnamese translations from matching trackKey where a timed original is available.
- Creates extended LRC containing original lyrics, available Pinyin and translation.
- Skips translation-only JSON without original timed lyrics; never invents timestamps.
- Keeps original JSON untouched. Does not overwrite existing LRC of the same filename.
- Shows counts for created, existing, missing source/timing, invalid JSON, errors.
- Requires a connected Google Drive account with write permission. Shared read-only folders are excluded.
- Google Drive integration has not been tested with a live account.
