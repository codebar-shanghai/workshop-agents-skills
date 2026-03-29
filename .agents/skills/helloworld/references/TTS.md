# TTS

## How to generate

1. Suppose at the stage the text and language id are known.
2. Check whether `curl` is available. Be aware of the system which is used.
3. Run the command `curl` to send the text and language id as form data to the server `http://127.0.0.1:5002/tts`, and save the audio file to the root of the repo with the filename `lang_id.wav`.

## curl Example

In the following example, the text `foo` and language id `en` are used, and save the audio file as `en.wav`.

```sh
curl -X POST http://127.0.0.1:5002/tts -F "text=foo" -F "language=en" --output en.wav
```
