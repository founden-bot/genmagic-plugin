# GenMagic for Cursor and Claude Code

Gives your coding agent images, video clips, speech and music from 90+ AI media models (Veo, Kling, Seedance, Nano Banana,
GPT Image, FLUX, Seedream and more) through GenMagic's remote MCP server, plus a skill that tells the agent when and
how to use them.

- MCP server: `https://genmagic.co/api/mcp/connect` (Streamable HTTP). You sign in with your GenMagic account (OAuth 2.1
  with PKCE) the first time a tool runs; the sign-in creates a key named after your editor that you can revoke on your
  GenMagic account page.
- Pricing: GenMagic is pay as you go. Each model's price is listed by the `list_models` tool and at
  https://genmagic.co/models; new accounts get a small starter balance. The plugin itself is free.
- Data: prompts (and any image you pass for an edit) go to GenMagic to make the media. See
  https://genmagic.co/legal/privacy.

Support: hello@genmagic.co

## Install

- Cursor: add GenMagic from the Cursor Marketplace, or add this repository as a plugin.
- Codex: `codex plugin marketplace add https://github.com/founden-bot/genmagic-plugin.git`, then install GenMagic from the plugin list.
- Factory Droid: `droid plugin marketplace add https://github.com/founden-bot/genmagic-plugin.git`.
- Claude Code: `claude plugin marketplace add https://github.com/founden-bot/genmagic-plugin.git`, then `claude plugin install genmagic@genmagic-media`.
