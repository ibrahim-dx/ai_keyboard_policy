[العربية](../ar/privacy.md) · [Terms of Use](terms.md)

# Privacy Policy

Last updated: 2026-11-18

This is the privacy policy of "AI Keyboard": an Arabic and English keyboard for Android with suggested words, voice dictation, AI rewriting and a clipboard for copied text. The app is a personal project installed directly on the phone. It has no servers and no accounts.

The app's interface is in Arabic. Button names are given here in English, with the Arabic label in brackets the first time each appears.

## In short

- What you type goes only to the app you are typing in. The keyboard does not store or log it, and the words it suggests come from a dictionary inside the app that does not learn from what you type.
- No ads, no analytics, no tracking, no accounts.
- Nothing leaves your phone unless you ask: text when you press the rewrite button `✦`, and the recording of a dictation when you end it, if your dictation goes through a provider. Both are sent to a provider you chose, and the recording is then deleted from your phone.
- The clipboard button shows what is on your phone's clipboard now. The keyboard keeps nothing of what you copy unless you ask it to remember earlier copies, and then on your phone only.
- Provider keys are stored encrypted, on your phone only.

## What the keyboard handles

**What you type.** Every keyboard sees what is typed with it, which is why Android shows a general warning when any keyboard is enabled. This keyboard passes the characters to the app you are typing in. It does not write them to any file or log, keeps no history of what was typed, and does not learn from it. The one exception is the emoji you last picked from the emoji panel, so that they come first next time, and you can switch that off on the "Emoji" (الإيموجي) page in the app.

**What it reads from the field.** To delete a character or a word, to put a space before dictated text, and to suggest a word, the keyboard reads a few characters before the cursor. When you press `✦` it reads the field's text and where the selection is, and it reads the field once more on "Undo" (تراجع) to make sure the text has not changed. The field is not read for any other purpose.

**What stays in memory for a moment.** During a rewrite the keyboard keeps the original text and the draft in memory, so that it can offer "Replace" (استبدال) and "Undo". During a dictation it keeps the text of what you dictated that time, so that it can be cleaned up if you end the dictation with `✦`. This is cleared when the rewrite panel is closed, at the next edit, or when you move to another field. It is never written to storage.

## Suggested words

- The dictionary is part of the app: two fixed lists, Arabic and English, and a short list of familiar phrases. It does not learn from what you type, your own words are not added to it, and what you pick from it is not kept.
- To suggest, the keyboard reads, after each character, the word you are typing and the two words before it, and looks them up in the dictionary. This happens in memory and on your phone only: nothing is sent and nothing is written to storage.
- The keyboard does not change what you typed by itself. A suggestion is written only when you press it.
- No suggestions appear, and the field is not read for them, in password fields and private fields, in number, address and e-mail fields, or in a field whose app asks for no suggestions.
- Suggestions need no consent, because they keep nothing and send nothing. You switch them off on the "Typing" (الكتابة) page in the app.

## When text or sound leaves your phone

### AI rewriting

- No text is sent without your press on `✦`: when you then choose a style or type an instruction, when you end a dictation with it, or when you use it to type a request in an empty field.
- **Rewriting text that is there.** The target text (the selection, or the whole field) is sent with the style's instruction.
- **Ending a dictation with the rewrite button.** Only the text of what you dictated that time is sent, so that misheard words are corrected and punctuation is added. The red button ends a dictation without sending its text for clean-up.
- **"Write for me" (اكتب لي) in an empty field.** The request you typed or dictated is sent, and nothing else.
- In every case the request goes straight from your phone to the provider, using your own key, and passes through no intermediate server. The result is shown as a draft, and is written into the field only when you press.
- Providers are tried in the order you set. If the first is busy or down, the same text is sent to the next one in your list. If the provider's model is not available to your key, the same text is sent to its other model, and then to the next provider. The name of the model that wrote the draft is shown on it.
- The name of the provider receiving the text is shown in the strip while it works, and then on the draft. Its privacy note is written on its badge in the settings.
- Once the text reaches a provider it is covered by that provider's policy, not by this one. Some free tiers may use text to improve their products; this is stated on each provider's badge in the settings.
- **Sensitive mode** (الوضع الحسّاس) limits sending to the providers you marked as "trusted" (موثوق).
- **Local server** (Ollama or LM Studio on your computer): the text stays inside your home network.

Providers listed in the app: Groq, Google Gemini, OpenRouter, Cloudflare Workers AI, Mistral, Anthropic Claude, OpenAI, and any compatible server you add yourself. Read each provider's policy before you enable it.

### Voice dictation

Dictation has two engines, and you choose between them on the "Voice input" (الإدخال الصوتي) page in the app. With either, the microphone opens only at your press, and closes as soon as the keyboard is hidden or the field changes.

**Through an AI provider.** This is the one used when you choose a provider for it, or whenever your list has an enabled provider that transcribes speech.

- When you press the microphone, the keyboard itself records your voice, into a temporary file inside the app's private storage. Nothing is sent while you speak.
- When you end the dictation, with the red button, with `✦`, or by pressing any key, the recording is sent straight from your phone to one provider, with your own key and through no intermediate server, and comes back as text that is typed into the field.
- **You choose who receives the recording**, on the "Voice input" page. If you choose one provider, the recording is sent to no other, even when that provider fails, and a dictation does not start while it is not ready. If you leave it on "Automatic" (تلقائي), the first provider in your list that transcribes speech receives it, and if that one is busy or down the same recording is sent to the next.
- Of the listed providers, these transcribe speech: Groq, Google Gemini, Mistral, OpenAI, and any compatible server you add yourself and name a model for. The name of the one receiving the recording is shown in the strip while it is transcribed. There, the sound is covered by that provider's policy, as text is, and its privacy note is written on its badge.
- The recording is deleted from your phone as soon as the text arrives. If it could not be sent, it stays so that it can be sent again with "Try again" (أعد المحاولة), and is then deleted at the next key you press, when another recording starts, when the field changes, or when the keyboard is hidden.
- A recording with no audible voice in it is not sent to anyone. The longest recording is five minutes.
- "Sensitive mode" applies to sound as it does to text.

**Through the Android system.** This is the one used if you choose it, or if you left the choice on "Automatic" and your list has no enabled provider that transcribes speech.

- Recording is done by the speech recognition service of the Android system on your phone (Google's on most devices), not by this app. The app asks for the service and receives only the resulting text. It stores no audio.
- The audio is covered by the policy of the recognition service installed on your phone, and may be processed on its servers.
- A dictation goes on until you press the stop button, and stops by itself after about ten seconds of silence.

### Testing a provider from the settings

When you test a provider from its page in the settings (testing the key, opening its model list and choosing a model from it, or the quality test), the app sends that provider a short request with a fixed sample text for each model it tries: its two models when the key is tested, and the model you press in the list. It also fetches its model list and what is left of its free allowance where the provider reports one. Nothing you typed is part of it.

### Nothing else

The app does not connect to the internet in any other case: no automatic updates, no crash reports, no usage statistics. What the keyboard reads of the phone's clipboard is never sent anywhere, and neither is what you type for the sake of suggested words.

## Clipboard

- **The phone's clipboard.** The clipboard button on the keyboard shows what your phone's clipboard holds now: the last text you copied in any app. The keyboard reads it when you copy while this is your selected keyboard, and each time it appears, to show it and to paste it with one press. It does not keep it: it is on the phone's clipboard, not in the keyboard. For two minutes the keyboard also offers, in its strip, to paste what you just copied with one press, and you can switch that offer off on the "Clipboard" (الحافظة) page in the app.
- **Remembering earlier copies.** Off by default. If you switch it on, on the "Clipboard" page, the keyboard keeps on your phone the texts that pass through its clipboard, so that you can paste them later: the last 20 of them (or 40), until you delete them or newer ones push them out, or for a lifetime you choose: a day, or an hour.
- **Pinned texts.** What you pin from the clipboard, or add in the app, stays until you delete it.
- **What the keyboard does not read.** Anything the app you copied from marked as sensitive (as password managers do on Android 13 and later), and anything you copy while typing in a password field or a private field: the keyboard shows that the clipboard holds a text without reading it, and if you press it, it asks the field to paste it from the phone's clipboard by itself. Images and files are not shown. Of a text longer than 5000 characters it reads only the beginning, to show it, and the field pastes it. None of these is ever kept, even when remembering is on.
- **A caution.** If you switch remembering on, a password copied by an app that does not mark it as sensitive may be remembered, and stays until you delete it unless you chose a lifetime. Delete it from there, choose a short lifetime, or leave remembering off if you copy passwords often.
- **It is not your phone's history.** Android keeps only the last thing copied, and gives keyboards no history of what came before. Samsung's clipboard history belongs to Samsung's keyboard, and no other keyboard can read it. So what the keyboard remembers is its own record, and it starts when you switch it on.
- **It stays on your phone.** What the keyboard reads of the clipboard, and what it remembers, is never sent anywhere, and is not part of "Export settings" (تصدير الإعدادات) or of any backup.
- **Control.** The keyboard does not read the phone's clipboard before you consent. Deleting the current text on the keyboard's clipboard panel deletes it from the phone's clipboard itself. You clear what the keyboard remembered with "Clear history" (مسح السجل) on the keyboard or in the app, and choose its lifetime and size, or switch it off, on the "Clipboard" page. Switching it off, or withdrawing your consent, deletes what it holds and keeps the pinned texts.
- The "Copy" (نسخ) button on the draft puts the result on the phone's clipboard, which is shared between your apps like any other copy. The "Paste the key and test it" (لصق المفتاح واختباره) button on a provider's page reads the clipboard once, when you press it, to take the key you copied.

## Sensitive fields

In password fields of every kind, and in fields whose app asks keyboards not to learn from them (such as private browsing), the rewrite button and the microphone are disabled and say why, and no words are suggested. In these fields the keyboard neither reads nor remembers what you copy, the emoji you type are not remembered, and if the keyboard offers to paste what you just copied it does so without showing the text. In password fields the key preview bubble is not shown either.

**Password manager suggestions.** On Android 11 and later, the keyboard's strip shows what the password manager you chose in your phone's settings suggests (Google Password Manager, Samsung Pass, or another): your saved sign-ins, or a strong new password. The keyboard tells the system only where they go, how large they are and in which colours. The suggestions are drawn by the system itself, in a surface the keyboard cannot read, so it does not know what they say, and a press on one fills the field through the system without what is filled passing through the keyboard. They may also appear in other fields your manager fills, such as a user name or an address. The keyboard keeps nothing of them and sends nothing, and what the manager suggests is covered by its own policy.

## What is stored on your phone

| What is stored | Where | Notes |
|---|---|---|
| Keyboard settings (language, theme, key roundness and height, letter size, side margin, vibration and key sound, digit style, whether suggested words are on, the dictation engine, emoji size and whether they are remembered, whether earlier copies are remembered, for how long and how many, and the paste offer) | App settings | Included in "Export settings" |
| The list of providers, their order, models (the dictation model among them) and addresses, the provider you chose for dictation, and your Cloudflare account ID if you entered one | App settings | Included in "Export settings" |
| Styles you created or edited (name and instruction), and the last style you used | App settings | Included in "Export settings" |
| Your consent to this policy and the terms of use (the version you accepted) | App settings | Included in "Export settings" |
| The emoji you used last, up to 32 | App settings | Kept only after you consent; switched off on the "Emoji" page; included in "Export settings" |
| The texts you pinned, and what the keyboard remembers of what you copied if you switched remembering on: the last 20 texts (or 40), until you delete them or for the lifetime you choose | A file of its own inside the app | Only after you consent; never part of any export |
| The recording of a dictation in progress, when dictation goes through a provider | A temporary file inside the app | Deleted as soon as it is transcribed; does not outlive the keyboard being hidden; never part of any export |
| Provider keys | Encrypted storage backed by the Android Keystore | Never shown in full, never part of any export |

"Export settings" copies the settings as text to the phone's clipboard, without the keys, and sends them nowhere.

No text you typed or dictated is stored, nor the texts you sent for rewriting, nor their results, and no recording remains once it has been transcribed.

The app is excluded from Android backup and from device-to-device transfer, so its settings, its keys and its clipboard history do not move to the cloud or to another phone.

## Permissions

| Permission | Why |
|---|---|
| Microphone | Voice dictation only: the keyboard's own recording, or the system's recognition service. The keyboard works without it. |
| Internet | Sending rewrite requests and dictation recordings when you ask for them. |
| Input method service | So that the system treats the app as a keyboard. |

Reading what you copy needs no permission: Android allows it for the keyboard you have selected.

## Deleting your data

- Delete a key: from the provider's page in the companion app.
- Clear what the keyboard remembered of your copies, or delete a pinned text: from the clipboard panel on the keyboard, or from the "Clipboard" page in the app. Clear the phone's clipboard itself: with a long press on the current text in the clipboard panel.
- Delete everything: clear the app's data from Android settings, or uninstall the app.
- What was already sent to a provider is covered by that provider's policy, and is deleted through them.

## Your consent

- The app asks for your consent once only: on the "Privacy and terms" (الخصوصية والشروط) page, which it shows the first time it is opened. This policy and the terms of use can be read there in full at any time.
- Before you consent, rewriting, dictation and the clipboard do not work. If you press one of their buttons on the keyboard, it opens that page for you, and nothing is sent, recorded or kept.
- Typing and suggested words need no consent, and send nothing.
- You can withdraw your consent on the same page. The copies the keyboard remembered and the recent emoji are then deleted, and the three features stop until you consent again.

## Changes to this policy

Any change in the app's behaviour that affects privacy is recorded in this file, and the date of each change is kept in the repository's history. If the version of the policy changes, the app asks again.
