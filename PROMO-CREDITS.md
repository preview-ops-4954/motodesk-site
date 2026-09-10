# MotoDesk hybrid promo - source and credits manifest

Deliverable: motodesk-hybrid-promo.mp4 (59.9s, 1280x720, 30fps, h264 + AAC 48kHz, ~6.1MB, faststart, -16 LUFS)
Poster/thumbnail: motodesk-hybrid-poster.jpg (1280x720)

## Structure (timeline)
- 0.0-0.9   Card: "THE PHONE WON'T STOP." (original, brand-styled)
- 0.9-2.9   B-roll: motorcycle workshop, bikes waiting (Mixkit 41941)
- 2.9-3.8   Card: "THE TICKET'S STILL ON PAPER."
- 3.8-5.9   B-roll: hands working a motorcycle engine (Mixkit 41928)
- 5.9-6.8   Card: "THE PARTS ARE THREE TABS DEEP."
- 6.8-8.9   B-roll: row of motorcycles in a garage (Mixkit 41927)
- 8.9-9.9   Card: "ONE DESK FOR ALL OF IT."
- 9.9-22.6  Product UI: dashboard + work order board (demo.mp4 0:00-0:12.7, original narration)
- 22.6-33.0 Product UI: ticket detail (demo.mp4 0:21.3-0:31.7)
- 33.0-40.5 Product UI: parts counter / draft PO (demo.mp4 0:42.3-0:49.8)
- 40.5-47.4 Product UI: "Nothing goes live without you" boundaries (demo.mp4 1:05.3-1:12.2)
- 47.4-56.4 Product UI: pilot offer "Run it next to what you use now" (demo.mp4 1:13.3-1:22.3)
- 56.4-59.3 End card: MOTODESK wordmark, free 6-8 week parallel pilot, getmotodesk.com,
            "watch the full 88-second walkthrough on the homepage"
- 59.3-59.9 Fade out

Product UI is on screen ~46.5s of 59.9s (78%). The outreach-only line
("Now booking pilot shops in Austin and San Antonio. Reply to claim a spot.")
is deliberately excluded; the cut lands in the silence after "no lock-in."

## Sources and licenses
1. demo.mp4 - original MotoDesk product screen capture with narration (own asset,
   from preview-ops-4954/motodesk-site repo; demo data only, no real shop data).
   Narration audio is reused verbatim from this asset - no new voice generated.
2. Mixkit b-roll (video-only files, no audio tracks):
   - https://mixkit.co/free-stock-video/arriving-at-a-workshop-full-of-motorcycles-41941/
   - https://mixkit.co/free-stock-video/mechanic-repairing-a-motorcycle-engine-41928/
   - https://mixkit.co/free-stock-video/many-motorcycles-parked-in-a-row-in-a-garage-41927/
   License: Mixkit Stock Video Free License - free for commercial use, no attribution
   required. No identifiable faces (one helmeted rider seen from behind).
3. Title/end cards - original renders (PIL) in the MotoDesk workbench identity:
   paper #f4efdf, card #fffdf5, ink #111, accent #ef5b24, shadow #aaa28f.
4. Fonts: Barlow Condensed (Bold/SemiBold) and IBM Plex Mono - SIL Open Font
   License 1.1, via google/fonts GitHub repo.
5. Poster: original render in the same identity.

## Truthful-boundary notes
- All UI footage shows the demo dataset (tag baked into the UI).
- Boundaries section states payments are log-only, reminders are drafts, supplier
  ordering stays locked - matches current product state.
- No testimonials, no shop results claims, no third-party branding in b-roll.

## Rebuild
Working files (segments, cards as PNG, concat list) were produced with ffmpeg + PIL.
Cards can be re-rendered from the fonts and hex values above if text needs changes.
