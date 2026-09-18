# What's new

BiVoice builds as they reach the [public beta](https://testflight.apple.com/join/KZUs8RRm).
TestFlight updates to the newest one on its own.

## 1.0 (7) — 18 September 2026

**Read Punctuation, set in BiVoice.** VoiceOver does not tell other speech engines its
punctuation setting: it sends exactly the same text whether punctuation is set to All or None.
Each profile now has its own Read Punctuation setting (None, Some or All), at the top of its
Speech Rules.

- Some reads symbols such as @, #, % and &. All also reads commas, full stops, question marks
  and the rest.
- Dots inside a web or email address, such as example.com, are no longer read as the end of a
  sentence.
- English voices read the Arabic comma as "comma".

**Speech rules now work with VoiceOver.** VoiceOver marks every sentence it sends with a
language, and BiVoice was treating that mark as your primary language, so the Primary Language
choice for numbers, punctuation and symbols made no difference. Your primary language is now
the one you chose in the profile. A number VoiceOver sends as a sentence of its own, such as a
battery percentage after its label, now follows the text around it.

**Lighter and smoother.** The app no longer pauses for half a second each time you return to it
while it reloads the voice list. The engine's work per phrase is down to a few milliseconds,
and voices no profile uses are released from memory.

## 1.0 (5) — 18 September 2026

**Speaking rate that matches VoiceOver.** VoiceOver's speaking rate, pitch and volume are now
passed to each voice unchanged, so the voice renders them exactly as it does for VoiceOver
itself. Previously the rate was converted, and at the highest speed BiVoice spoke about 22%
slower than Apple's own voice.

- The volume slider for each language is now exact.
- If BiVoice goes missing from VoiceOver's voice list after an update or a restart, opening the
  app registers it again. If it still does not appear, restart your iPhone and open BiVoice
  once more.

## 1.0 (3) — 18 September 2026

**The engine follows your settings.**

- Pitch. VoiceOver's pitch and the Pitch slider for each voice now change the voice. Previously
  neither had any effect.
- A punctuation mark is no longer read aloud unless you asked to hear it, and punctuation names
  are read by the voice the Punctuation rule picks.
- Symbols such as @, #, % and & follow the Symbols rule.
- Change Voice for Single Words. When it is off, one word in another language, such as
  "iPhone" in an Arabic sentence, is read by the voice of the sentence around it.
- Pause Between Languages adds its pause wherever the voice changes language, including inside
  a sentence.
- Text VoiceOver asks to be spelled is read letter by letter.

## 1.0 (2) — 17 September 2026

The first public beta.

- The whole interface was rewritten, and is translated into Arabic, Chinese (Simplified),
  English, French, German, Hindi, Indonesian, Italian, Japanese, Portuguese (Brazil), Russian,
  Spanish and Turkish.
- The app is now called BiVoice.
- Every feature is free for seven days. After that, BiVoice is a single purchase, kept for life.
