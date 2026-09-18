# BiVoice

A speech engine for VoiceOver on iPhone that gives every language its own voice, and changes
between them in the middle of a sentence.

If you read Arabic and English together, you know the problem: VoiceOver reads the whole line
with one voice, and the English words come out mangled. Turning on Detect Languages helps a
little, but it works sentence by sentence and misses short switches. BiVoice looks at the script
each part is written in and hands it to the voice you picked for that language, so "اشتريت
iPhone جديد" is read by your Arabic voice and your English voice together.

- [Try the public beta on TestFlight](https://testflight.apple.com/join/KZUs8RRm)
- [What's new](CHANGELOG.md)
- [Privacy Policy](PRIVACY.md)
- [Terms of Use](TERMS.md)
- [Support](SUPPORT.md)

## Public beta

BiVoice is in public beta. Open the link above on your iPhone, install TestFlight if you do not
have it, and accept the invitation. New builds arrive through TestFlight automatically.

Purchases in the beta go through Apple's test environment, so you are not charged. Please send
what you find, good or bad, to support.dev.a@gmail.com or through TestFlight's own feedback.

Requires an iPhone with iOS 17 or later.

## Setting it up

There is one step in Settings: Accessibility → VoiceOver → Speech → Voice, then choose your
profile under BiVoice. Everything else is set in the app, and every change is heard straight
away, without turning VoiceOver off and on.

You do not need to add a second language to VoiceOver's rotor, and Detect Languages can stay
off. BiVoice switches voices on its own.

## Profiles

A profile is a set of languages, each with its own voice. Each profile appears in VoiceOver as a
single voice. Make a second one with a different pair of voices, and move between them by adding
Voice to the VoiceOver rotor.

A profile is named after its languages until you give it a name of your own. Its primary
language decides where it is listed in VoiceOver's voice list, and which voice reads anything
that does not belong to another language.

## For each language

- **Voice.** Any voice iOS lets a speech engine use, with a preview button next to each one.
- **Speaking rate, pitch and volume.** These are relative to what VoiceOver asks for, so you can
  balance one voice against another. A quiet Arabic voice can be brought up to match a loud
  English one.

## Following VoiceOver

BiVoice passes VoiceOver's speaking rate, pitch and volume to each voice exactly as VoiceOver
sends them, so the voice renders them the same way it would for VoiceOver itself. At the highest
speaking rate, BiVoice speaks as fast as Apple's own voice.

VoiceOver does not tell other speech engines its punctuation setting. It sends the same text
whether punctuation is set to All or None. So BiVoice has its own setting for it, described
below.

## Speech rules

Each profile has its own rules:

- **Read Punctuation.** None, Some or All. Some reads symbols such as @, # and %. All also
  reads commas, full stops, question marks and the rest. Dots inside a web or email address are
  left for the voice to read naturally.
- **Numbers, Punctuation and Symbols.** Which voice reads them: the one reading the text before
  them, the one reading the text after them, or your primary language. This holds even when
  VoiceOver sends a number as a sentence of its own, such as a battery percentage after its
  label.
- **Arabic-Indic Digits Use the Arabic Voice.** ٣٤٥ is read in Arabic even inside English text.
- **Change Voice for Single Words.** When it is off, a single word from another language, such
  as a brand name in an Arabic sentence, stays with the voice of the sentence around it.
- **Read Punctuation Names in the Surrounding Language.** A punctuation name is said in the
  language of the voice reading it: "comma" from the English voice, "فاصلة" from the Arabic
  one.

And two for timing:

- **Pause Between Languages.** From 0 to 800 milliseconds, added wherever the voice changes
  language. A short pause makes the change easier to follow; zero is the fastest.
- **Trim Silence Between Segments.** Removes the silence voices leave at their edges, so a change
  of language does not sound like a gap.

The Preview section plays any text you type through the same rules VoiceOver uses.

## About the voices

BiVoice does not ship any voices. It uses what iOS already has on your iPhone.

There is a limit worth knowing before you install it. iOS runs third-party speech engines in a
restricted process that can only reach voices whose data is part of iOS itself. Voices you
downloaded separately (Enhanced, Premium), Siri voices, Eloquence, and voices belonging to other
apps are not available to any third-party engine, including this one. That still leaves a
voice for each of about 49 languages, plus the older English voices such as Albert, Fred and
Kathy.

The app lists every voice it can use, and next to each one it cannot, it says why.

## Light on your iPhone

BiVoice only decides which voice reads which part. The speaking itself is done by iOS, as it is
for Apple's voices. Its own share of the work is a few milliseconds per phrase, the first sound
starts about 20 milliseconds after VoiceOver asks, and voices that no profile uses any more are
released from memory.

## Languages

The app is available in Arabic, Chinese (Simplified), English, French, German, Hindi, Indonesian,
Italian, Japanese, Portuguese (Brazil), Russian, Spanish and Turkish.

## Privacy

BiVoice collects nothing. The text VoiceOver reads is processed in memory on your iPhone, is
never written to storage, and never leaves the device. The app makes no network connections.
The full [Privacy Policy](PRIVACY.md) says the same thing at more length.

## Price

Free to download, with every feature included for seven days. After that, BiVoice is a single
purchase, made once and kept for life, on every device signed in to your Apple Account. No
subscription. If the trial ends and you have not bought it, VoiceOver keeps speaking with the
system's voice.

BiVoice is an independent app. It is not affiliated with, endorsed by, or sponsored by Apple
Inc.

Developed by Abdulmajeed Almarzoqi.
