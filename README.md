# Framewise support

Framewise is a desktop app for macOS and Windows that writes stock-ready
titles, descriptions, keywords and locations for batches of video clips,
using your own Anthropic (Claude) or OpenAI API key.

This page is the place to get help, report a problem or suggest a feature.
The app's source code isn't public; this repository only hosts support and
the [privacy policy](PRIVACY.md).

## Get help

- **Report a bug:** [open a bug report](https://github.com/skootrz/framewise/issues/new?template=bug_report.yml)
- **Suggest a feature:** [open a feature request](https://github.com/skootrz/framewise/issues/new?template=feature_request.yml)
- **Email:** [scottj@live.com](mailto:scottj@live.com), if you'd rather not
  use GitHub or your question includes anything private

Before opening an issue, check the [existing issues](https://github.com/skootrz/framewise/issues?q=is%3Aissue)
in case someone has already reported it. Issues are public, so never paste an
API key, and only attach frames or clips you're happy for anyone to see.

## Frequently asked questions

### Do I need an account?

No. Framewise has no account and no subscription. You need an API key from
[Anthropic](https://console.anthropic.com/) or [OpenAI](https://platform.openai.com/api-keys).
Paste it on the welcome screen, or later under **API keys** in the sidebar.

### What does it cost to run?

The AI provider bills you directly for what you use, usually from under a
cent to a few cents per clip depending on the model and clip length. Framewise
shows an estimate before you start and tracks usage clip by clip. Frames are
downscaled before upload to keep costs low. Setting a monthly spending limit
in your provider's console is a good idea.

### Which models can I use?

Claude Haiku, Sonnet and Opus with an Anthropic key, or GPT-6 Luna, GPT-6 Sol
and GPT-4o with an OpenAI key. Haiku and Luna are the fastest and cheapest;
Opus and Sol give the most detailed results.

### Which video formats work?

MP4 and MOV in H.264, HEVC and ProRes, plus most other common formats. If a
clip won't load, please [report it](https://github.com/skootrz/framewise/issues/new?template=bug_report.yml)
with the camera model and the format details from your camera or editor.

### Where does the location come from?

If the clip has GPS data, Framewise turns it into a place name. It reads:

- the location tags phones and most cameras write
- GoPro GPS telemetry
- the telemetry in DJI drone and Osmo footage
- the `.SRT` files older DJI drones record next to each clip

Without GPS, the AI suggests a likely location from what it sees, and you can
correct it before exporting.

### Why isn't my DJI .SRT file used on the Mac App Store version?

The Mac App Store version can only open files you select. To use an `.SRT`
file, add it together with its clip (select both, or add the whole folder).

### The analysis failed with an API error

- **401 or "invalid key":** the key was mistyped, revoked, or belongs to the
  other provider. Use **Test** under **API keys**.
- **Insufficient credit or quota:** add credit or raise the limit in your
  provider's billing settings.
- **Rate limit or "overloaded":** wait a minute and retry the clip.

### Where is my data stored?

On your computer. API keys are kept in the macOS Keychain or Windows
Credential Manager. Your clips are never uploaded; only a few still frames go
to the AI provider you choose. The [privacy policy](PRIVACY.md) has the
details.

## Privacy

Framewise has no server, analytics, tracking or ads. Read the full
[privacy policy](PRIVACY.md).
