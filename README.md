# Gemini-tts-ultimate
A free, unlimited Text-to-Speech tool powered by Google Gemini 2.5.
# 🌍 Gemini Ultimate TTS (Text-to-Speech)

![Gemini 2.5](https://img.shields.io/badge/Powered_by-Gemini_2.5_Flash-4285F4?style=for-the-badge&logo=google)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-Web_Browser-orange?style=for-the-badge)

**A free, unlimited, and privacy-focused Text-to-Speech tool that runs 100% in your browser.**

Turn books, articles, or scripts into lifelike audio using Google's latest `Gemini 2.5 Flash` model. No monthly subscriptions, no character limits, and no server-side tracking.

---

## 🌟 Special Features (Why use this?)

Most TTS tools charge by the character or require complex Python scripts. **Gemini Ultimate TTS** solves this:

* **🚀 Unlimited Text Processing:** Unlike the standard API which limits you to small chunks, this tool uses **"Smart Splitting"**. Paste a whole novel (100k+ characters), and it automatically breaks it down by sentence, processes it, and merges it back into one seamless audio file.
* **🛡️ Multi-Key "Round Robin" System:**
    * *The Problem:* The Free Tier has a speed limit (15 requests/minute).
    * *The Solution:* You can input **multiple API keys**. If Key #1 hits a limit, the app instantly switches to Key #2, then Key #3, ensuring uninterrupted generation for long projects.
* **🔄 Auto-Retry Logic:** If a network error occurs or the AI "hiccups," the system waits and retries the chunk up to 5 times. It doesn't crash; it persists.
* **🎨 4 Exclusive Themes:**
    * **Modern:** Clean, glassmorphism UI.
    * **Retro:** Old paper texture with typewriter fonts.
    * **Future:** Cyberpunk neon aesthetics.
    * **Terminal:** Hacker-style command line interface.
* **🔒 100% Private (Client-Side):** There is no backend server. Your API keys and your text **never** leave your computer (except to go directly to Google's API).

---

## 🛠️ How to Use

### Step 1: Get the Code
1.  Download the `index.html` file from this repository.
2.  Open it in any modern browser (Chrome, Edge, Firefox).

### Step 2: Get Your Free API Key
1.  Go to [Google AI Studio](https://aistudio.google.com/app/apikey).
2.  Click **"Create API Key"**.
3.  *Pro Tip:* Create 2 or 3 keys if you plan to generate hours of audio at once.

### Step 3: Generate Audio
1.  Paste your API Key(s) into the settings box (one per line).
2.  Select a **Voice** (e.g., *Charon* for deep narration, *Fenrir* for energetic reading).
3.  Paste your text into the main box.
4.  Click **Generate Audio**.
5.  Wait for the progress bar to hit 100%, then click **Download .WAV**.

---

## 💡 How is this Useful? (Use Cases)

### 📚 For Students & Learners
* **Audiobooks:** Convert PDF textbooks or long articles into audio to listen while commuting.
* **Language Learning:** Paste French, Japanese, or Tamil text to hear perfect native pronunciation. (Gemini supports 70+ languages).

### 🎬 For Content Creators
* **YouTube/TikTok Voiceovers:** Generate professional-grade voiceovers for faceless videos without paying for expensive tools like ElevenLabs.
* **Podcasts:** Use the "Multi-Speaker" simulation (by running the tool twice with different voices) to create podcast intros.

### ♿ Accessibility
* **Visual Aid:** A high-quality, free alternative to screen readers for reading long web content.
* **Dyslexia Support:** Listen to emails or documents to improve comprehension.

### 💻 For Developers
* **Test Bench:** A perfect playground to test the limits of the `gemini-2.5-flash-tts` model before building your own app.
* **Code Template:** Use this open-source code as a foundation for your own AI projects.

---

## ⚙️ Technical Details

* **Model:** Uses `gemini-2.5-flash-preview-tts` (Optimized for speed and high daily quotas).
* **Audio Format:** Outputs 24kHz WAV (Linear PCM).
* **Storage:** Uses browser `localStorage` to remember your API keys and theme preference.
* **Limits:** The tool bypasses the *Request Payload Limit* by chunking, and bypasses the *Rate Limit* by key rotation.

---

## ❓ FAQ

**Q: Is it really free?**
A: Yes. Google provides a generous "Free Tier" for the Gemini API (approx. 1,500 requests/day). This tool allows you to utilize that free tier fully.

**Q: Can I use this for commercial work?**
A: The code is MIT Licensed (free to use). However, check Google's [AI Terms of Service](https://ai.google.dev/terms) regarding the use of the specific *audio* output for commercial purposes.

**Q: My key stopped working!**
A: You likely hit the "RPM" (Requests Per Minute) limit. Just wait 60 seconds, or add a second API key to the list to distribute the load.

---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE). Feel free to fork, modify, and sell your own versions.

> **Disclaimer:** This is a community project and is not affiliated with Google. API keys are stored only on your local device.
