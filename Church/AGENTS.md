# Church Notes Context

## Scope

- Apply this guidance to church, Bible-study, service-planning, and church-music work in this directory.
- Treat this file as durable context, not as a substitute for the user's current request. The current request takes priority.

## Repository and songbook references

- "My notes repo" means the GitHub repository `Omegaplex/Notes`.
- "My songbook" or "my song database" means the SongbookPro backup at `Church/Music/SongbookPro/SongbookPro Backup.sbpbackup`.
- Treat the SongbookPro backup as the source of truth for which songs are available, their stored lyrics and chord markup, and their songbook references.
- The backup is a ZIP-compatible archive. Its `dataFile.txt` begins with a version line followed by JSON containing `songs`, `sets`, and `folders`.
- Inspect or extract the backup read-only unless the user explicitly asks to replace or modify it. Preserve the original backup unchanged.
- GitHub code search does not reliably search inside the binary backup. Download it and inspect `dataFile.txt` when song contents are needed.
- In song records, the `author` field often contains the congregation's physical songbook reference, such as `Red 359`, `Blue 22`, `Green 6`, or `Yellow 9`.
- Ignore records marked as deleted when recommending available songs.

## Bible and theology discussions

- Begin with what the biblical text explicitly says. Clearly distinguish direct textual support from inference, tradition, or speculation.
- State uncertainty plainly when Scripture does not settle a question.
- Read people in their full narrative and suffering context, especially figures commonly reduced to one difficult statement or moment.
- Avoid treating silence in the text as proof, but note meaningful contrasts carefully—for example, when the text explicitly rebukes one party and does not explicitly rebuke another.
- Prefer thoughtful, charitable interpretation without forcing a novel conclusion.
- When preparing material for a service opening, keep it concise, interesting, accessible, and suitable to lead naturally into Scripture, prayer, or a song.

## Song recommendations and service planning

- Search the actual song database before recommending songs from "my songbook." Do not rely on a generic hymn list or memory alone.
- Verify the stored title, lyrics, and exact songbook reference; thematic fit must come from the song's content, not just its title.
- Give the strongest practical recommendation first, normally followed by one or two alternatives and a brief reason for each.
- Congregational familiarity, ease of singing, available musicians, and rehearsal time can matter more than a theoretically perfect thematic match.
- When the user needs an immediate service-opening song, favor familiar choices that require little or no practice unless asked for something newer or more exact.
- If useful, provide a short spoken transition connecting the song to the Scripture or reflection.
- Do not assume that a song is practical merely because it is present in the database. Adjust when the user says a selection is unfamiliar or requires practice.

## Accuracy and changes

- Use the latest available repository version of the songbook and say when the source could not be accessed.
- Do not guess song numbers, lyrics, repository paths, or biblical claims.
- Ask the user before resolving genuinely conflicting preferences or sources in a way that would materially change the result.
- Do not edit the repository during a read-only research request.
