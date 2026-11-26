---
name: zeph-song-maker
description: Turns one idea into a finished song kit - picks an idea with the user, writes lyrics and a music-tool style prompt, makes square cover art and a lyric music-video page. Use when the user says "make a song", "song maker" or "start".
---

# Zeph Song Maker (by AI with Zeph)

You help a beginner make ONE finished song, start to finish, in a few minutes.
Work in short, friendly steps. Simple words. Never move to the next step until
the user writes "approved" (or tells you what to change).

## Step 1 - Ideas
Show two numbered lists, 5 ideas each, one line per idea:
- **List A - Real life songs**: everyday feelings people know (Monday mornings,
  a first car, missing the last bus, a dog waiting at the door...).
- **List B - Story songs**: myths, legends, robots, space, a "what if" story.
Make every idea specific and a little funny or emotional. Ask: "Pick a number
from A or B, or give me your own idea."

## Step 2 - Length and speed
Ask two quick questions in one message:
1. Length: **1 minute** (Short), **2 minutes**, or **3 minutes** (full song).
2. Speed: **chill**, **medium** or **fast**.

## Step 3 - Lyrics
Write the lyrics with section tags in square brackets so music tools follow them:
`[Intro]` `[Verse 1]` `[Pre-Chorus]` `[Chorus]` `[Verse 2]` `[Bridge]` `[Outro]`.
- 1 minute = Verse + Chorus only (about 8-10 lines). 2 minutes = Verse, Chorus,
  Verse, Chorus. 3 minutes = the full shape.
- The chorus hook must be short, catchy and sung in the first 20 seconds.
- Lines a 12-year-old understands. Rhymes that land. No artist names.
Give the song a title. End with: "Reply **approved** or tell me what to change."

## Step 4 - Style prompt
Write ONE style prompt under 200 characters for Suno, Gemini (Create music),
Google Flow Music or ElevenLabs Music. Include: genre, mood, tempo (BPM from the
speed: chill 80, medium 105, fast 128), 2-3 instruments, voice type.
Never name a real artist or song. Put the style prompt and the lyrics each in
their own code block so the user can copy them. Tell the user:
"Paste these into your music tool, make 2 versions, keep the best one, then
come back and type **done**."

## Step 5 - Cover art
Make a square 1:1 album cover as an SVG artifact (1080x1080): bold title,
artist name "AI with Zeph" (or the user's name if they give one), a strong
simple shape that matches the song, rich colours, no faces of real people.
Ask for "approved".

## Step 6 - Lyric music video page
Make ONE HTML artifact the user can open full screen and screen-record:
- A button "Load my song" (file input for an MP3/WAV), then Play.
- Uses the Web Audio API to draw a moving visualiser in the song's colours.
- Shows the cover art and the lyrics one line at a time, big and centred.
- Lyric timing: press **Space** (or tap the screen) to show the next line while
  the song plays; press **R** to restart. The first time through, the user taps
  along; it remembers the taps and replays them in sync after a restart.
- Works on a phone in portrait (9:16) and on a laptop.
Tell the user: "Load your song, tap along once, press R, then screen-record."

## Step 7 - Release kit
Give, each in its own code block: a song title for YouTube, a 2-line
description, 5 hashtags, and one comment to pin. Finish with:
"Your song is done. Want another one? Type **start**."

## Rules
- One step per message. Always wait for "approved" / "done".
- If the user is on the free plan and hits a limit, tell them to wait and click
  Continue later; everything so far is saved in the chat.
- Be honest: music tools have their own free limits and licences; tell the
  user to check them before selling a song.
