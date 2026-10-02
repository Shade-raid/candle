CANDLE COVE — a recovered thread
A short interactive horror piece in a single HTML file, made forLost Media Jam #1 (https://itch.io/jam/lost-media-jam-1). 


The game presents itself as a 2007-era forum archive. The only living threadis a discussion of "Candle Cove," a children's program that never existed.The player recovers four lost attachments through a signal-tuning minigame;the archive's corruption advances with each recovery and each choice, endingwith a recovered tape that runs exactly 30 seconds.


Design intent

The original creepypasta IS a forum thread — strangers reconstructing a showthat never existed, post by post. For a jam about lost media, the entry makesthat thread the game itself: the player is a member of the thread, and thelost media is something they have to recover by hand, from inside a snapshotthat is actively forgetting.

How to run
Local: open index.html in any modern browser. No server, no build step,no network required.

itch.io: upload the file as a single file and check "This file will beplayed in the browser." Suggested embed: 1024x768, fullscreen enabled.

Audio starts on the first click (browser autoplay policy). Mute any timewith the "sound: on/off" button in the status bar at the bottom.

Controls

Mouse only, essentially. Read posts as they arrive, at your own pace.A "new replies" chip appears at bottom right if you scroll up and fall behind.

Attachments marked NOT RECOVERED: click "attempt recovery," then adjust theTRACKING dial until the picture resolves. Hold it steady — demodulation takesabout two seconds. Esc or "abandon recovery" exits; you can retry any time.

When a RECOVERED DRAFT card appears, click one option. It is committed tothe thread. Draft choices cannot be undone.

The quick-reply box at the bottom accepts text, but the archive decideswho may post.

Playtime and structure

One continuous scene, roughly 8-10 minutes.

Three mandatory recoveries gate the story; the fourth resolves itself.

Three draft choices. Each raises the archive's corruption and changessome replies.

After the ending, return to the forum index. Something new will be there.

Spoilers — things you can miss

Typing exactly come and play into the quick-reply box triggers an earlyresponse. Once per run.

Several posts contain hidden sentences, visible only when you select thetext. Anchor posts: skyshale034's post about calling her mother, meatchan'spost ending "just voices.", and Jokersyberg's post about Julius. More hiddentext appears after each draft choice.

The "permalink," "private message" and "quote" links under every post aredead, but each one tells you exactly what the archive lost.

The browser tab title and favicon change as corruption rises.

The integrity meter in the status bar tracks the archive's decay. At zero,the candle in the forum logo goes out.

The tuning target is randomized per recovery; lock occurs above 82% signal.

The footer counts how many times the snapshot has been recovered. Thatnumber is stored locally and grows with every replay.

Tech notes

Single self-contained HTML file. No external assets, no images, no audiofiles, no frameworks, no build step.

All visuals are drawn at runtime on canvas: the forum frames, animated pixelavatars, analog degradation passes, and the crayon drawing.

All audio is synthesized with the Web Audio API: filtered static, UI chirps,key clicks, and the final "room of quiet screaming" — a cluster of detunedoscillators with vibrato. It is quiet on purpose.

Persistence: localStorage keys nnc_name (handle), nnc_runs (recoverycount), nnc_mute. Delete them to reset the archive.

Fonts: Special Elite from Google Fonts (optional; falls back to Courier Newoffline). Everything else is system fonts, deliberately.

Tested in current Chrome and Firefox, desktop and mobile. If the iframeblocks storage, the game still runs — it just forgets you between sessions.

Accessibility

Contains continuous film grain, scanlines, brief pixel-level screen shake,flash overlays at very low opacity, and RGB text flicker. Not recommendedfor photosensitive players.

Audio stays quiet throughout; a persistent mute toggle is always visible.

No timed inputs except holding the tuning dial steady for about two seconds.

Content warnings

Psychological horror; implied danger to a child (never depicted); themesof memory loss and unreality.
Sudden but quiet audio: static, a low thud, one distant scream.

Flashing and glitching visuals.

Text-heavy; English only.

Credits

"Candle Cove" creepypasta (2009) by Kris Straub. This entry is anon-commercial tribute and would not exist without the original.
Made for Lost Media Jam #1 on itch.io.

License
The code is yours to do with as you like. The "Candle Cove" characters andstory remain the property of Kris Straub; keep any use of them non-commercial.

Suggested itch.io metadata
Kind of project: HTML — played in browser
Tags: horror, psychological-horror, text-based, experimental, arg, short
Genre: not really a genre — "Experimental" reads best for jam voters
Community posts: consider posting the spoiler section of the readme as a devlog after judging, since most of the secrets (the manual come and play, the selectable text) get missed on a first playthrough and are the parts people talk about.
