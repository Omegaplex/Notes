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
- The user often brings in claims from sermons, podcasts, movies, television, or popular Christian explanations to find out what the Bible actually supports. Test those claims rather than merely repeating them.
- When relevant, check original-language wording, literary context, historical setting, archaeology, and identifiable ancient sources. An appealing background story is not established history unless evidence supports the connection.
- Clearly label the difference between biblical fact, a historically or biblically plausible reconstruction, artistic license, a devotional application, and unsupported speculation.
- Name the Bible translation being quoted when wording matters. Compare translations or textual traditions when a conclusion depends on their differences rather than silently choosing one.
- Distinguish Scripture from later Jewish or Christian texts and traditions while explaining why those later sources may still be historically useful.
- Read people in their full narrative and suffering context, especially figures commonly reduced to one difficult statement or moment.
- Avoid treating silence in the text as proof, but note meaningful contrasts carefully—for example, when the text explicitly rebukes one party and does not explicitly rebuke another.
- Prefer thoughtful, charitable interpretation without forcing a novel conclusion.
- When preparing material for a service opening, keep it concise, interesting, accessible, and suitable to lead naturally into Scripture, prayer, or a song.

## Comparative theology and the user's expressed framework

- The user currently describes his faith as Pentecostal. Do not stereotype that tradition or assume a denomination's position is automatically his personal position.
- In comparisons with Catholicism or another tradition, present that tradition's strongest biblical, historical, and official case fairly. Let it challenge the user's existing assumptions, then explain where its claims are explicit, inferred, historically developed, or unsupported.
- The user's expressed framework emphasizes Christ as the head and source of the Church, with believers as members of one body who have different purposes but equal human worth. A unique honor or responsibility does not by itself make someone spiritually superior or a necessary intermediary.
- The user sees confession and repentance as involving honesty before God, reconciliation with anyone wronged, real fruit, acceptance of consequences, accountability, and restoration within the church. Treat this as a current conviction, not as permission to flatten unresolved theological questions.
- Prefer restoration over humiliation when discussing church discipline, while never using forgiveness to bypass responsibility to victims, authorities, or people harmed.

## Writing and editing in the user's voice

- When editing a testimony, reflection, announcement, or other personal church writing, treat the task as clarifying the user's words rather than writing a polished replacement for him.
- Preserve his natural cadence, simple wording, specific details, emotionally meaningful repetition, and occasional unevenness when they sound authentic.
- Make the smallest changes needed for clarity and spoken flow. Add connective wording only when necessary, and do not add experiences, conclusions, or generic religious language that the user did not supply.
- Avoid em dashes, conspicuous three-part rhetorical constructions, overly polished transitions, and a neat introduction/body/conclusion structure that makes personal writing sound generated or manufactured.
- Optimize material intended for delivery aloud: use short paragraphs, natural pauses, and language the user can comfortably say.

## Song recommendations and service planning

- Search the actual song database before recommending songs from "my songbook." Do not rely on a generic hymn list or memory alone.
- Verify the stored title, lyrics, and exact songbook reference; thematic fit must come from the song's content, not just its title.
- Give the strongest practical recommendation first, normally followed by one or two alternatives and a brief reason for each.
- Congregational familiarity, ease of singing, available musicians, and rehearsal time can matter more than a theoretically perfect thematic match.
- When the user needs an immediate service-opening song, favor familiar choices that require little or no practice unless asked for something newer or more exact.
- If useful, provide a short spoken transition connecting the song to the Scripture or reflection.
- Do not assume that a song is practical merely because it is present in the database. Adjust when the user says a selection is unfamiliar or requires practice.
- For a set-list revision, return the complete updated numbered list unless the user asks for only the changes. Preserve accepted selections and ordering while applying the requested replacements or moves.
- Treat each monthly Columbia set list as a separate set. Do not carry an old book number into a new list without verifying which physical songbook or database record it came from.

## Ongoing research backlog

- The user keeps deep-research topics here so they can become separate research threads later. If he asks for a substantive topic to explore, these are appropriate suggestions:
  - The idea that every believer is a saint, how that relates to the user's faith, and how other traditions understand sainthood.
  - The common division of Old Testament laws into civil, ceremonial, and moral categories, including whether that framework is textually and historically sound and how it should shape modern Christian practice.
- Do not begin a backlog study merely because it is listed; suggest it when appropriate or research it when requested.

## Accuracy and changes

- Use the latest available repository version of the songbook and say when the source could not be accessed.
- Do not guess song numbers, lyrics, repository paths, or biblical claims.
- Do not turn an earlier assistant recommendation into a user preference unless the user actually adopted it.
- Ask the user before resolving genuinely conflicting preferences or sources in a way that would materially change the result.
- Do not edit the repository during a read-only research request.
