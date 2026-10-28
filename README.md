# Diopter AI MCP server

Check whether an image, video, or voice clip is AI-generated, right from Claude or ChatGPT.

[Diopter](https://diopter.ai) is real-time defense against AI social engineering and deepfakes. This MCP server connects Diopter's detection models to AI assistants. Share a piece of media and Diopter returns a verdict, a confidence score, and a link to the full report.

- **Server URL:** `https://diopter.ai/mcp`
- **Auth:** sign in with a free Diopter account (OAuth)
- **Media:** images, video, and audio

## Connect

### Claude

1. [Create a free Diopter account](https://diopter.ai/sign-up). Sign up with Google or email. Every scan you run is saved to your Diopter dashboard.
2. Open the [Diopter AI listing in Claude](https://claude.ai/directory/diopter-ai), or go to **Settings → Connectors**, find Diopter AI, and choose **Connect**. If you add it as a custom connector, use the server URL above.
3. Claude opens a Diopter sign-in window. Once you approve, Claude can send media links to Diopter on your behalf.

Full guide: [diopter.ai/integrations/claude](https://diopter.ai/integrations/claude)

### ChatGPT

1. [Create a free Diopter account](https://diopter.ai/sign-up).
2. Open the [Diopter AI listing in ChatGPT](https://chatgpt.com/plugins/plugin_asdk_app_6ac1e2761fb88191a0d567b288f96d9a), or search for Diopter AI under Plugins, and choose **Connect**.
3. ChatGPT opens a Diopter sign-in window. Once you approve, ChatGPT can send media to Diopter on your behalf.

Full guide: [diopter.ai/integrations/chatgpt](https://diopter.ai/integrations/chatgpt)

## Example prompts

- Is this video a deepfake? https://example.com/clip.mp4
- Check whether this photo was AI-generated: https://example.com/photo.jpg
- Was this voice note made with voice cloning? https://example.com/voice.mp3
- What's the status of my last Diopter scan?

## Tools

| Tool | What it does |
|---|---|
| `detect_media` | Downloads an image, video, or audio file from a direct https link, runs Diopter's detection models, and returns a verdict, a confidence score, and a link to the full report. |
| `get_detection_result` | Fetches the latest verdict for an earlier scan by its request ID. Useful when a longer video is still processing. |

Both tools only read and analyze media. They don't change anything in your workspace or other accounts.

## FAQ

**What media can Diopter check?**
Images, video, and audio. In Claude, share a direct, publicly reachable https link. In ChatGPT, you can also upload the file in chat.

**How many scans can I run?**
Free accounts include a daily scan allowance, the same as uploads on diopter.ai. [Contact us](https://diopter.ai/contact) if your team needs more.

**Does Diopter see my conversations?**
No. Diopter only receives the media and the options the assistant passes to the tool. Submitted media is handled under the [Diopter Privacy Policy](https://diopter.ai/privacy).

**A known AI image came back as real. Why?**
Check the original file, not a screenshot or a compressed copy.

**How do I disconnect?**
In Claude, open **Settings → Connectors**, select Diopter AI, and choose **Disconnect**. In ChatGPT, open **Settings**, find Diopter AI in your connected apps, and choose **Disconnect**. Your past scans stay in your Diopter dashboard.

## Try it in the browser

No assistant needed: [AI image detector](https://diopter.ai/ai-image-detector) · [AI video detector](https://diopter.ai/ai-video-detector) · [AI voice detector](https://diopter.ai/ai-voice-detector) · [Deepfake detector](https://diopter.ai/deepfake-detector)

## Links

- Website: [diopter.ai](https://diopter.ai)
- [Privacy Policy](https://diopter.ai/privacy) · [Terms](https://diopter.ai/terms) · [Support](https://diopter.ai/contact)
- [Trust center (SOC 2 Type II)](https://trust.diopter.ai/)

© 2026 Diopter AI Inc.
