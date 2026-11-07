---
name: genmagic-media
description: Use when the project needs a real image, icon, logo, illustration, short video clip, voiceover or music track (a hero image, an app icon, a product shot, a demo clip, a sound): generate it with the GenMagic MCP tools instead of leaving a placeholder.
---

# Making media for the project with GenMagic

The GenMagic MCP server (connected by this plugin; you sign in with your GenMagic account the first time a tool runs)
gives these tools:

- `list_models`: the models you can pick, with ids and prices. Free, no sign-in needed.
- `generate_image`: an image from a prompt, or an edit of a given image; `type: "logo"` for a clean brand mark.
- `generate_speech`: text read aloud, word for word, in a chosen voice.
- `generate_music`: an original track from a description.
- `create_video` then `get_video`: a clip is a job. `create_video` returns an id at once and charges nothing;
  `get_video` returns the clip when it is ready and charges once, on completion.
- `generate_text`: text, code, an SVG graphic or a web page from any text model.

How to use them well:

1. Every generation is paid from the person's GenMagic balance. Before a costly call (video, or several images), say
   which model you will use and its price from `list_models`, and prefer the default model unless the person asked for
   a specific one.
2. Save what you generate into the project (for example `public/images/`) with a descriptive file name, and write
   real alt text for images.
3. For a logo or icon, use `generate_image` with `type: "logo"`, then check it reads at small sizes.
4. For video, poll `get_video` every 15 to 30 seconds; clips usually take one to five minutes.
