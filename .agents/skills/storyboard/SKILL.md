---
name: storyboard
description: Turn a brief, reference images, or footage into a scene-by-scene storyboard and an edited video. Use for /storyboard, storyboard-to-video requests, and short-form video editing.
---

# Storyboard video editor

Treat `/storyboard` as a request to use this workflow. Use the user's language for captions and narration. Preserve the referenced character, wardrobe, and story beats throughout the edit.

1. Identify the intended deliverable, source assets, target platform, and duration. For an unspecified social video, use 9:16 and aim for 20–30 seconds. Treat an attached contact sheet as a sequence of shots. Use a character turnaround as a continuity reference.
2. Build a timecoded shot list with duration, framing, movement, on-screen text, and audio cues. Give the most important emotional or informational beats enough screen time. Keep captions inside the platform's safe area and check readability on mobile.
3. Use supplied footage whenever available. If the user provides stills, use clean source panels or generate scene stills from the references with an available image tool. Avoid duplicating captions baked into an input panel. Use subtle reframing where it serves the story. If a motion-generation tool is available and the brief calls for moving characters, check continuity between separately generated shots.
4. Assemble the scenes with the available editor or FFmpeg. Keep music, dialogue, and effects audible at appropriate levels. Use a font that supports the requested language and check shaping and line breaks in the rendered captions.
5. Export one playable MP4 per requested cut. Use H.264, yuv420p, and AAC when audio is present. For a vertical short, target 1080 × 1920 unless the source quality or platform calls for other dimensions.
6. Check duration, aspect ratio, and stream information with ffprobe or equivalent. Review representative frames for continuity and caption placement. Provide the video and identify whether motion came from footage, generated clips, or camera moves over stills. If rendering is unavailable, give the timecoded edit plan and state what remains to be rendered.
