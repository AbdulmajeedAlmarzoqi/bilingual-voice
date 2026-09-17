# Bilingual Voice

A speech engine for VoiceOver on iOS that uses a different voice for each language in the same
sentence.

If you read Arabic and English together, you know the problem: VoiceOver reads the whole line
with one voice, and the English words come out mangled. Turning on "Detect Languages" helps a
little, but it works sentence by sentence and misses short switches. Bilingual Voice looks at
the script each part is written in and hands it to the voice you picked for that language, even
in the middle of a word group.

- [Privacy Policy](PRIVACY.md)
- [Terms of Use](TERMS.md)
- [Support](SUPPORT.md)

## How it works

You select the engine once, in Settings → Accessibility → VoiceOver → Speech → Voice. Everything
after that is set in the app: which voice reads which language, and what to do with numbers,
punctuation and symbols. Changes take effect immediately, without restarting VoiceOver.

You can build more than one profile — say Maged with Samantha, and another with Tarik and
Victoria — and switch between them from the rotor.

## About the voices

Bilingual Voice does not ship any voices. It uses what iOS already has on your device.

There is a limit worth knowing before you install it. iOS runs third-party speech engines in a
restricted process that can only reach voices whose data is part of iOS itself. Voices you
downloaded separately (Enhanced, Premium), Siri voices, and voices belonging to other apps are
not visible to any third-party engine, including this one. That is roughly 68 voices on a
current device: one per language for about 49 languages, plus the older English voices such as
Albert, Fred and Kathy.

The app lists every voice it can use, and next to the ones it cannot it says why.

## Price

Free to download, with a one-week trial. After that a single purchase unlocks it for good. No
subscription. If the trial runs out and you have not bought it, VoiceOver keeps working and
falls back to the system's default voice.

Developed by Abdulmajeed Almarzoqi.
