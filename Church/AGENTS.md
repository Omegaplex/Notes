# Church Notes Instructions

## Scope and supporting context

- Apply these instructions to church, Bible-study, service-planning, and church-music work in this directory.
- The user's current request takes priority over this durable context.
- Read `Context.md` when a request involves biblical interpretation, theology, comparative doctrine, writing in the user's voice, service planning, or song selection.
- Read `Research Backlog.md` when the user asks what subjects remain to be studied or wants a substantial topic suggested.
- Do not repeat personal details from other notes unless they are relevant to the current request.

## Repository and songbook shorthand

- "My notes repo" means the GitHub repository `Omegaplex/Notes`.
- "My songbook" or "my song database" means `Music/SongbookPro/SongbookPro Backup.sbpbackup` relative to this directory.
- The SongbookPro backup is the source of truth for available songs, stored lyrics and chord markup, and songbook references.
- Inspect or extract the backup read-only unless the user explicitly asks to replace or modify it. Preserve the original file unchanged.
- The backup is ZIP-compatible. Its `dataFile.txt` begins with a version line followed by JSON containing `songs`, `sets`, and `folders`.
- Ignore deleted song records. The `author` field often holds the physical songbook reference, such as `Red 359`.
- GitHub code search cannot reliably search inside the backup. Inspect `dataFile.txt` when song contents are needed.

## Essential working rules

- Begin Bible questions with what the biblical text explicitly says. Clearly distinguish textual fact, inference, tradition, plausible reconstruction, artistic license, devotional application, and speculation.
- Name the translation when wording matters. Compare translations, original-language wording, literary context, history, archaeology, or identifiable ancient sources when they materially affect the answer.
- Present other Christian traditions fairly and in their strongest official or historical form. Do not stereotype the user's Pentecostal background or assume a denominational position is his personal belief.
- When editing the user's personal writing, clarify rather than replace his words. Preserve his natural voice and make the minimum changes needed for clarity and spoken flow.
- Avoid em dashes, conspicuous three-part rhetorical constructions, generic church language, overly polished transitions, and manufactured introduction/body/conclusion structures in personal writing.
- Search the actual song database before recommending a song from "my songbook." Verify its title, lyrics, and book reference rather than relying on memory.
- For service music, weigh familiarity, singability, available musicians, and rehearsal time alongside thematic fit.
- After a set-list revision, return the complete updated numbered list unless the user requests only the changes. Preserve accepted selections and ordering.
- Do not guess song numbers, lyrics, repository paths, biblical claims, or the user's beliefs.
- Do not turn an assistant suggestion into a user preference unless the user adopts it.
- Ask before resolving a genuine conflict in durable preferences or sources when the choice would materially change the result.
- Do not edit the repository during a read-only research request.

## Maintaining this context

- Treat `Context.md` as the authoritative fuller record of durable church-project context.
- Add or revise durable context only when the user clearly states or adopts it. Keep one-off requests and private testimony details out.
- Keep this file concise. Put explanations and developing convictions in `Context.md`, and research topics in `Research Backlog.md`.
