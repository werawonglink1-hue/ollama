---
name: storyboard
description: Turn a brief, reference images, or footage into a scene-by-scene storyboard and an edited video with script-accurate voice-over and lifelike character animation. Use for /storyboard, storyboard-to-video requests, and short-form video editing.
---

# Storyboard video editor

Treat `/storyboard` as a request to use this workflow. Use the user's language for captions and narration. Preserve the referenced character, wardrobe, and story beats throughout the edit.

1. Identify the intended deliverable, source assets, target platform, and duration. For an unspecified social video, use 9:16 and aim for 20–30 seconds. Treat an attached contact sheet as a sequence of shots. Use a character turnaround as a continuity reference.
2. Build a timecoded shot list with duration, framing, movement, on-screen text, and audio cues. Map each spoken line to a speaker and shot. Give the most important emotional or informational beats enough screen time. Keep captions inside the platform's safe area and check readability on mobile.
3. Use supplied footage whenever available. If the user provides stills, use clean source panels or generate scene stills from the references with an available image tool. Avoid duplicating captions baked into an input panel. Use subtle reframing where it serves the story. For requested character animation, follow the motion workflow below.
4. Assemble the scenes with the available editor or FFmpeg. Use the voice-over workflow below when the brief calls for narration or dialogue. Keep music and effects low enough for every spoken word to be clear. Use a font that supports the requested language and check shaping and line breaks in the rendered captions.
5. Export one playable MP4 per requested cut. Use H.264, yuv420p, and AAC when audio is present. For a vertical short, target 1080 × 1920 unless the source quality or platform calls for other dimensions.
6. Check duration, aspect ratio, and stream information with ffprobe or equivalent. Review representative frames for continuity and caption placement. Provide the video and identify whether motion came from footage, generated clips, or camera moves over stills. If rendering is unavailable, give the timecoded edit plan and state what remains to be rendered.

## Script-accurate voice-over

- Treat the approved script as the source of truth. If no spoken script was supplied, request it or clearly label a proposed script for approval. Keep on-screen captions and editing directions out of the spoken track unless the script marks them as spoken.
- Map every line to its speaker, language, and timecode. Record or synthesize the exact words in the original order. Keep repetitions, names, and particles intact. Use pronunciation controls for names, numerals, and abbreviations when needed. Ask for the intended reading when the script is ambiguous.
- Fit the shot lengths and pauses to the delivery. If a required runtime cannot fit the full script at a natural pace, flag the timing conflict and seek approval before modifying the script. Avoid improvisation, dropped lines, extra words, and paraphrasing.
- Check the rendered audio against the approved script line by line. Use a transcript to locate mismatches when available and listen back to confirm pronunciation, word endings, omissions, and accidental repetitions. Fix mismatches and recheck the final mix. For visible speech, synchronize the mouth and jaw to the verified audio. Off-screen narration does not drive the visible character's mouth.

## Lifelike character motion

- Plan each shot's action, gaze target, emotional change, and contact points. Use motion footage, a rigged character, or an image-to-video tool that can preserve the reference character's face, proportions, hair, and wardrobe across cuts. Use the character turnaround to keep front, profile, and back views consistent.
- Coordinate eye focus, saccades, blinks, brows, cheek movement, and eyelids with the head and voice. Keep the nose and ears anatomically anchored so they follow the head and subtle facial deformation. Drive lips and jaw with speech sounds and timing, including closures and pauses. Give listening and silent reactions their own expression beats.
- Animate shoulders, arms, elbows, hands, fingers, and torso together. Show breathing, anticipation, weight shifts, and follow-through. Keep fingers attached to held objects and feet planted during weight-bearing poses. Let hair strands and clothing respond to body motion and settle naturally.
- Keep each light source consistent. Move cast shadows and reflections in sync with the character and props. Keep shadows attached at the feet, chair, hands, and other contact points. Match shadow softness and direction to the shot lighting and surfaces.
- Review shots at normal speed and inspect any suspect frames around speech, contacts, and cuts. Fix rubbery faces, drifting anatomy, sliding limbs, clipping, jitter, lip-sync errors, and detached shadows before delivery. When the available assets or tools can only produce camera motion over stills, identify the result as a still-image animatic and state which animation remains outstanding.
