# VoiceBank Free

Free, fully in browser voice banking. Record your voice, clone it on your device, type to talk. No account, no server, no upload, $0.

Built for people facing voice loss, including esophageal cancer and brain cancer, and anyone who wants to bank their voice before surgery or before speech declines.

## How it works

1. Record. Read 6 prompted sentences into your microphone. Each clip is stored in your browser with its exact transcript.
2. Build your voice. The app clones your voice on device from a 3 second reference using Qwen3-TTS 0.6B Base.
3. Type to talk. Type anything and hear it in your voice. Quick phrases, speed and pitch controls, 10 languages.

## Privacy

Everything stays on your device. Recordings live in the browser only. Nothing is uploaded anywhere. You can export a backup or erase everything from the app.

## Engine

Qwen3-TTS 0.6B Base, Apache 2.0, running in the browser through ONNX Runtime Web on WebGPU. Fallbacks: Qwen3-TTS 1.7B CustomVoice, then Chatterbox through voxshot, then the system voice. A WebGPU browser such as Chrome, Edge, or Brave is recommended for cloning. Other browsers fall back to the system voice.

## Run it

Open `index.html` in a browser, or enable GitHub Pages on this repo. The first load fetches the model weights from Hugging Face and caches them in the browser.

## Status

Prototype. The interface and type to talk flow are verified. Microphone recording and live model inference need a test on a real device with a microphone and WebGPU.
