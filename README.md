# Neuron Lexicon v2.0.0 🧠

&lt;img width="500" height="500" alt="neuron-preview" src="https://github.com/user-attachments/assets/629edfb7-238a-49f0-bd88-8329299ef111" /&gt;

[![Version](https://img.shields.io/badge/version-2.0.0-purple.svg)](#) [![Platform](https://img.shields.io/badge/platform-Android-lightgrey.svg)](#) [![Expo](https://img.shields.io/badge/built%20with-Expo%20SDK%2054-000020.svg)](https://expo.dev)

**Neuron** is an intelligent, AI-powered dictionary and vocabulary curator. Built for logophiles and casual learners alike, Neuron transcends traditional dictionaries by utilizing generative AI to discover, define, contextualize, and visualize words you can't quite remember, and even transcribes your voice directly to search.

Built with ❤️ by **Chiza Labs**.

---

## ✨ Key Features

* **Generative AI Discovery:** Can't remember a word? Just describe it (e.g., *"the smell of rain"* or *"the fear of tight spaces"*), and Neuron's AI will find the exact word for you.
* **Voice-to-Text Search:** Native, frictionless audio transcription. Tap the mic, speak your thought, and let the AI instantly transcribe and search it.
* **Deep Context & Etymology:** Go beyond basic definitions. Neuron generates dynamic example sentences, nuanced usage insights, and fascinating etymologies for every word.
* **Multimedia Carousel:** Every word comes alive with a horizontal gallery of AI-curated visuals. Swipe through up to 3 images per definition and download your favorites directly to your device gallery.
* **Your Personal Library:** Save newly discovered words directly to your device via an ultra-fast local SQLite database. Access your curated lexicon entirely offline.
* **Smart Enrichment:** Words automatically gain deeper definitions and images as you browse. Online or offline - your experience never breaks.
* **Fluid UI/UX:** A bold, energetic interface built on a Deep Indigo and Gold palette. Smart animations, network-aware states, and dynamic layouts.

---

## 🎨 Visual Identity

| Token | Hex | Role |
|-------|-----|------|
| Deep Indigo | `#4B0082` | Primary backgrounds, commanding titles |
| Bright Purple | `#9640FF` | Buttons, active states, icon accents |
| Gold | `#E3A501` | Section labels, highlights, borders |
| Mustard | `#FFDB58` | Subtle card tints, warning states |
| Light Orange | `#FFB44D` | Recording pulse, microphone glow |

---

## 📥 Download & Installation

### Android (.apk)
1. Navigate to the [Releases](../../releases) tab on this repository.
2. Download the latest `Neuron-v2.0.0.apk` file to your Android device.
3. Open the file to install (you may need to allow "Install from Unknown Sources" in your settings).

&gt; **Minimum Requirements:** Android 8.0 (API 26), ~80MB storage

### iOS
*Not available for direct APK distribution. iOS requires an Apple Developer Account ($99/year) and App Store submission. Contact Chiza Labs for TestFlight beta access.*

---

## 🏗️ Architecture

| Layer | Technology |
|-------|-----------|
| Frontend | React Native + Expo SDK 54 (New Architecture enabled) |
| Local Database | expo-sqlite with WAL mode, zero-downtime migrations |
| AI Engine | Groq SDK - llama-3.3-70b-versatile |
| Image Pipeline | Unsplash API → Cloudinary CDN |
| Audio | expo-av (Voice-to-Text transcription) |
| Distribution | Direct APK via [chizalabs.vercel.app](https://chizalabs.vercel.app/apps/neuron) |

---

## 🔒 Privacy

Neuron is built with privacy and efficiency at its core:

* **All saved words** are stored **locally** on your device via SQLite. No cloud sync. No tracking.
* **AI requests** are routed securely through Chiza Labs' serverless backend on Vercel.
* **Images** are fetched from Unsplash and cached via Cloudinary — no personal data leaves your device.
* **Zero third-party analytics** in the app. We respect your focus.

---

## Changelog
**v2.0.0** (2026-06-05)

  - Complete visual overhaul - Deep Indigo & Gold palette
  - Horizontal image carousel with native download support
  - Richer AI schema: nuance, origin, and multimedia per word
  - Smart lazy enrichment for local database words
  - Working bookmark persistence with SQLite
  - Network detection and offline-first architecture
  - Hardened backend with rate-limit resilience

**v1.2.0**

  - Basic AI search and voice transcription
  - Local SQLite word storage
  - Splash screen and update checking

**v1.0.0**

  - Initial release

© 2026 **Chiza Labs**. All rights reserved.
