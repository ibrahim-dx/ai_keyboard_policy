[العربية](../ar/privacy.md) · [Terms of Use](terms.md)

# Privacy Policy

Last updated: 2026-11-17

This is the privacy policy of "AI Keyboard": an Arabic and English keyboard for Android with voice dictation and AI rewriting. The app is a personal project installed directly on the phone. It has no servers and no accounts.

The app's interface is in Arabic. Button names are given here in English, with the Arabic label in brackets the first time each appears.

## In short

- What you type goes only to the app you are typing in. The keyboard does not store or log it.
- No ads, no analytics, no tracking, no accounts.
- Text leaves your phone only when you press the rewrite button `✦` and choose a style, and then it goes to the provider you chose.
- Provider keys are stored encrypted, on your phone only.

## What the keyboard handles

**What you type.** Every keyboard sees what is typed with it, which is why Android shows a general warning when any keyboard is enabled. This keyboard passes the characters to the app you are typing in. It does not write them to any file or log, keeps no history of what was typed, and does not learn from it.

**What it reads from the field.** To delete a character or a word, and to put a space before dictated text, the keyboard reads a few characters before the cursor. When you press `✦` it reads the field's text and where the selection is, and it reads the field once more on "Undo" (تراجع) to make sure the text has not changed. The field is not read for any other purpose.

**What stays in memory for a moment.** During a rewrite the keyboard keeps the original text and the draft in memory, so that it can offer "Replace" (استبدال) and "Undo". Both are cleared when the rewrite panel is closed, at the next edit, or when you move to another field. They are never written to storage.

## When text leaves your phone

### AI rewriting

- Nothing is sent until you press `✦` and then choose a style or type an instruction.
- The target text (the selection, or the whole field) is sent with the style's instruction, straight from your phone to the provider, using your own key. The request passes through no intermediate server.
- Providers are tried in the order you set. If the first is busy or down, the same text is sent to the next one in your list.
- The name of the provider receiving the text is shown in the strip while it works, and then on the draft. Its privacy note is written on its badge in the settings.
- Once the text reaches a provider it is covered by that provider's policy, not by this one. Some free tiers may use text to improve their products; this is stated on each provider's badge in the settings.
- **Sensitive mode** (الوضع الحسّاس) limits sending to the providers you marked as "trusted" (موثوق).
- **Local server** (Ollama or LM Studio on your computer): the text stays inside your home network.

Providers listed in the app: Groq, Google Gemini, OpenRouter, Cloudflare Workers AI, Mistral, Anthropic Claude, OpenAI, and any compatible server you add yourself. Read each provider's policy before you enable it.

### Voice dictation

- Recording is done by the speech recognition service of the Android system on your phone (Google's on most devices), not by this app. The app asks for the service and receives only the resulting text. It stores no audio.
- The audio is covered by the policy of the recognition service installed on your phone, and may be processed on its servers.
- Listening stops as soon as the keyboard is hidden or the field changes.

### Testing a provider from the settings

When you test a provider from its page in the settings (testing the key, loading its model list, or the quality test), the app sends that provider a short request with a fixed sample text, and fetches its model list and what is left of its free allowance where the provider reports one. Nothing you typed is part of it.

### Nothing else

The app does not connect to the internet in any other case: no automatic updates, no crash reports, no usage statistics.

## Sensitive fields

In password fields of every kind, and in fields whose app asks keyboards not to learn from them (such as private browsing), the rewrite button and the microphone are disabled and say why. In password fields the key preview bubble is not shown either.

## What is stored on your phone

| What is stored | Where | Notes |
|---|---|---|
| Keyboard settings (language, theme, vibration, key height, digit style) | App settings | Included in "Export settings" |
| The list of providers, their order, models and addresses, and your Cloudflare account ID if you entered one | App settings | Included in "Export settings" |
| Styles you created or edited (name and instruction), and the last style you used | App settings | Included in "Export settings" |
| Your consent to this policy and the terms of use (the date of the version you accepted) | App settings | Included in "Export settings" |
| Provider keys | Encrypted storage backed by the Android Keystore | Never shown in full, never part of any export |

"Export settings" (تصدير الإعدادات) copies the settings as text to the phone's clipboard, without the keys, and sends them nowhere.

Nothing you typed is stored, nor the texts you sent for rewriting, nor their results.

The app is excluded from Android backup and from device-to-device transfer, so its settings and keys do not move to the cloud or to another phone.

## Clipboard

The "Copy" (نسخ) button on the draft puts the result on the phone's clipboard, which is shared between your apps like any other copy. The keyboard does not read the clipboard. The "Paste and test" (لصق واختبار) button on a provider's page reads it once, when you press it, to take the key you copied.

## Permissions

| Permission | Why |
|---|---|
| Microphone | Voice dictation only. The keyboard works without it. |
| Internet | Sending rewrite requests when you ask for them. |
| Input method service | So that the system treats the app as a keyboard. |

## Deleting your data

- Delete a key: from the provider's page in the companion app.
- Delete everything: clear the app's data from Android settings, or uninstall the app.
- What was already sent to a provider is covered by that provider's policy, and is deleted through them.

## Your consent

- The keyboard asks for your consent once only: at the first press on the rewrite button or the microphone, before the field is read or anything is sent. One consent covers both.
- Typing needs no consent, and sends nothing.
- This policy and the terms of use can be read in full at any time under "Privacy and terms" (الخصوصية والشروط) in the app, and from the "Read the policy" (اقرأ السياسة) button when you are asked.
- You can withdraw your consent on the same page. The keyboard then asks again at the next use.

## Changes to this policy

Any change in the app's behaviour that affects privacy is recorded in this file, and the date of each change is kept in the repository's history. If the policy's date changes, the keyboard asks again at the next use.
