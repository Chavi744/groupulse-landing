# Veo / Gemini prompts — opening B-roll only

These generate the **0:00–0:06 establishing shot** of the demo: a therapist in a calm room
just after a group session, who picks up a phone to dictate. The app UI itself comes from a
screen recording of `demo.html` — **do not** ask the AI to render app screens or on-screen text
(it renders text, and especially Hebrew, unreliably).

## Generation settings
- **Model:** Veo 3 (via Gemini app or Google AI Studio / Vids).
- **Duration:** ~8s clips (generate each shot separately, trim in editing).
- **Aspect ratio:** 16:9 for landing page hero; 9:16 if the demo targets mobile/Reels.
- **Audio:** keep it ambient only — add the voiceover yourself later (AI speech ≠ your script).
- Generate 2–3 takes per prompt and pick the best; faces/hands vary between takes.

## Prompt principles baked in below
Subject → setting → action → camera move → lens/lighting → mood. Plus a "do not include" line
to avoid garbled text and busy UI.

---

### Prompt 1 — Establishing wide (the room empties)
```
A warm, softly lit group-therapy room in late evening. A circle of empty chairs, a few
cushions, a plant by the window, muted natural light fading outside. A calm therapist in
their 30s–40s, smart-casual, stands near the chairs after a session has ended, taking a
quiet breath. Slow cinematic dolly-in, shallow depth of field, 35mm lens, gentle golden
ambient lighting, hopeful and professional mood. Realistic, documentary feel.
No on-screen text, no captions, no logos, no app interface.
```

### Prompt 2 — Medium: picking up the phone
```
Medium shot of a calm therapist sitting on the edge of a chair in a quiet therapy room
after a group session, soft evening light. They exhale, then pick up a smartphone from a
small side table and hold it up, ready to speak a short note. Natural, unhurried movement.
Static camera on a tripod, shallow depth of field, warm cinematic color grade, 50mm lens.
Calm, focused, professional mood.
No readable screen content, no on-screen text, no captions, no logos.
```

### Prompt 3 — Close-up: thumb taps record (screen kept generic)
```
Close-up over the shoulder of a therapist's hand holding a smartphone in a softly lit room.
The thumb moves to tap a single round button near the bottom of the screen. The phone screen
is slightly out of focus and not legible. Shallow depth of field, soft bokeh background,
warm cinematic lighting, macro feel, gentle handheld motion.
Keep the phone screen blurred and generic — no readable UI, no text, no app graphics, no logos.
```
> Tip: keeping the screen blurred here lets you **composite the real `demo.html` UI** onto the
> phone in editing, or hard-cut from this close-up straight into the screen recording.

---

## Negative prompt (paste into a "negative"/"avoid" field if available)
```
on-screen text, captions, subtitles, watermarks, logos, app user interface, readable phone
screen, distorted hands, extra fingers, warped faces, glitchy text, clinical clutter
```

## Hebrew note (הערה)
ה-prompts כתובים באנגלית כי Veo מבין אותם טוב יותר. הם מתארים *תמונה* בלבד — אין בהם טקסט,
אז אין בעיית עברית/RTL. את הקריינות בעברית מוסיפים בעריכה (מתוך `DEMO_SCRIPT.md`).
