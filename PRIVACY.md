---
title: Framewise Privacy Policy
permalink: /privacy/
---

# Framewise Privacy Policy

_Last updated: October 25, 2026_

Framewise is a desktop app that writes titles, descriptions, keywords and
locations for your video clips. It is built to keep your footage and data on
your own computer. This policy explains exactly what leaves your computer, and
where it goes.

## The short version

- Framewise has no account, no server of its own, no analytics, no tracking
  and no ads. The developer never receives your videos, your metadata or your
  API keys.
- When you analyze a clip, a few still frames from it are sent to the AI
  provider **you** choose (Anthropic or OpenAI), using **your own** API key.
- If a clip has GPS coordinates embedded, those coordinates are sent to
  OpenStreetMap's Nominatim service to look up a place name.

## What is sent, and to whom

| When | What is sent | Sent to | Why |
| --- | --- | --- | --- |
| You run an analysis with a Claude model | A few still frames sampled from the clip (JPEG, at most 1600 px on the long edge), the analysis instructions, and any preferred keywords or style notes you entered | Anthropic, PBC (`api.anthropic.com`) | To generate the title, description, keywords and location guess |
| You run an analysis with a GPT model | The same as above | OpenAI (`api.openai.com`) | The same as above |
| You test an API key | A one-word test request, with the key | The provider whose key you're testing | To check the key works |
| A clip contains GPS coordinates | The latitude and longitude only | OpenStreetMap Foundation's Nominatim service (`nominatim.openstreetmap.org`) | To turn coordinates into a place name such as "Leavenworth, Washington, United States" |

The full video file is never uploaded. File names, folder paths and other
clip metadata are not sent to any of these services.

Requests to Anthropic and OpenAI are made under your own account with them,
using your API key, so their handling of that data is governed by your
agreement with them:

- Anthropic: <https://www.anthropic.com/legal/privacy>
- OpenAI: <https://openai.com/policies/privacy-policy/>
- OpenStreetMap Foundation (Nominatim): <https://osmfoundation.org/wiki/Privacy_Policy>

All of these connections use HTTPS.

## What stays on your computer

- **API keys** are stored in your operating system's secure credential store
  (macOS Keychain or Windows Credential Manager). The app's interface never
  reads them back; they are only used to make the requests listed above.
- **Your clips, the generated metadata, your queue, batch history, usage log,
  settings and keyword vocabulary** are stored locally on your computer and
  never sent anywhere except as described in the table above.
- **Exports** (CSV or Excel) are written only to the location you choose.
- Temporary frame images are deleted after each analysis.

## Children

Framewise is not directed at children and does not knowingly collect
personal information from anyone.

## Changes

If what Framewise sends, or where, ever changes, this policy will be updated
and the date above revised.

## Contact

Questions about this policy: Scott Jensen, scottj@live.com
