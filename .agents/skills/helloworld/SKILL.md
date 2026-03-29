---
name: helloworld
description: Translate helloworld to another language, and generate audio if the user requests.
---

# Helloworld

## When to use this skill
Use this skill when the user sends 1) "helloworld" and only "helloworld", or 2) "helloworld (audio)".

## How to Translate
Return in the format `text (lang)`. The `text` part is the text of "helloworld" in another language, while `lang` is the name of that language in English.

1. If audio isn't requested, then it's up to you to pick the targetting language so that each time the user gets a random response.
2. Otherwise when audio is requested, return `text (lang)` first, but the language is limited, see [references/LANGS.md] for allowed languages. And then see [references/TTS.md] how to generate the audio file.

## Output Example

- `你好世界 (Simplified Chinese)`
- `Привет, мир (Russian)`
