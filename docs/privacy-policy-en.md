---
permalink: /privacy-policy-en/
---

# ThaiJam Privacy Policy (iOS)

**Last updated: 17 August 2026**

[繁體中文版](/privacy-policy/)

> This page applies to the **iOS version**. The Android version has a
> [separate policy](/privacy-policy-android/) because it does not use iCloud or Apple Music.

## In one sentence

ThaiJam does **not** sell your data or use it for advertising or cross-app tracking. Most data
starts on your device. Depending on the features you choose, the app may connect to ThaiJam's
Cloudflare services, your private iCloud database, LRCLIB, Apple Music, Spotify, Shazam,
OpenAI, or Microsoft Azure Speech as described below.

## Data we collect and store

On first launch, ThaiJam creates a random **anonymous ThaiJam account identifier and session**.
This lets server-backed features work without asking for your name or email. Most on-device
features do not require Apple or Google sign-in. You must link Apple or Google before buying
AI Credits or using the same ThaiJam account reliably on another device. Spotify uses its own
authorization page.

ThaiJam has no advertising SDK and no third-party analytics package. It does not record which
screens you open or how long you spend on them. AI service usage records are described under
“AI usage records.”

| Data | Where it is stored | Purpose |
| --- | --- | --- |
| Study results, review schedule and streak activity | On-device database; ThaiJam servers if cross-device sync is enabled | Schedule reviews and continue on another device |
| Pronunciation score and assessment time, excluding the recording | On-device database; ThaiJam servers if cross-device sync is enabled | Practice history and sync |
| Cards, decks, hidden state and deck membership you create or import | On-device database; ThaiJam servers if cross-device sync is enabled | Your study content and sync |
| Song details and lyrics you add | On-device database; ThaiJam servers if cross-device sync is enabled | Song study and sync |
| AI word notes and purchased song-analysis results | On-device database; ThaiJam servers if cross-device sync is enabled | Preserve results you spent credits on |
| Renames and colors applied to official decks | On-device database; ThaiJam servers if cross-device sync is enabled | Preserve your customizations |
| Study Coin balance and ledger | ThaiJam servers | Prevent duplicate grants and keep the balance consistent |
| Owned themes, icons and content packs; remaining hint tickets and streak shields | ThaiJam servers | Preserve ownership and prevent duplicate rewards |
| Imported audio and artwork | App documents folder; your private CloudKit database if iCloud audio backup is enabled | Singing practice and media restoration |
| Spotify authorization token | Device Keychain | Search Spotify and control playback; it is not uploaded or synced |
| Spotify Client ID | Device preferences; iCloud KVS if iCloud audio backup is enabled | Connect the Spotify developer app selected by you; no Client Secret is stored |
| Daily review limit and card color setting | Device preferences; ThaiJam servers if cross-device sync is enabled | Keep reward-affecting and purchased settings consistent |
| Other display preferences | Device preferences only | Keep device-specific choices, such as text size, local |
| Random content-installation identifier | Device preferences; sent only to the content service when used | Downloads and error handling |

### Audio and artwork are not stored on ThaiJam's servers

Imported audio and artwork are never uploaded to ThaiJam's servers. If you enable iCloud audio
backup, they are stored as media assets in **your own private CloudKit database**. Song title,
artist, lyrics and translation may sync because they are editable study data; the media files do not.

### Two separate controls

- **Cross-device sync:** stores selected study data on ThaiJam's servers. An anonymous account
  can use this on the current installation; linking Apple or Google lets other iOS or Android
  devices access the same account.
- **iCloud audio backup:** stores imported audio and artwork in your private iCloud database.

If you turn off cross-device sync, later changes remain only on the device. Removing the app
removes local data. Data already stored on ThaiJam's servers can be exported or deleted from
Account settings.

### Anonymous account

The anonymous identifier contains no name, email address, or provider account. It is persistent
and is associated with server-backed data. If you later sign in with Apple or Google, ThaiJam
attempts to link that provider to the same user ID so your existing data is preserved. If the
provider already belongs to another ThaiJam account, the app asks before switching and does not
merge the two server accounts automatically.

## Identifiers used on iOS

| Identifier | Purpose | Retention |
| --- | --- | --- |
| Anonymous ThaiJam user ID | Server-backed features without registration | Until account deletion |
| Random installation ID | Content downloads and request limits | Cleared when the app is removed |
| Provider-specific Apple or Google user ID, if linked | Find the same ThaiJam account on another device | Until account deletion |
| App Attest device-key information | Confirm that protected requests come from an authentic ThaiJam app | Until account deletion |

For the one-time welcome grant, Apple DeviceCheck stores device bits for ThaiJam. ThaiJam does not
receive a reusable hardware identifier from DeviceCheck. None of these identifiers is used for
advertising or tracking across apps.

## AI usage records

ThaiJam does not use Firebase Analytics, Crashlytics, or another third-party analytics SDK, and it
does not record your navigation through the app. However, each AI request creates a service record
linked to your ThaiJam account containing:

- the AI feature and model used;
- input and output token counts and cost;
- success or failure and the time of the request.

These records support credit reconciliation, refunds after failed requests, cost control, service
reliability and abuse prevention. They do **not** contain the text you submitted. Aggregated request
counts and costs may be used for service analytics. This corresponds to the Product Interaction
disclosure in the app's App Store privacy information.

## Outbound network connections

The app may connect to the network in these cases:

1. **Cross-device sync.** If enabled, study records, user content, song details, lyrics, purchased
   AI results and Study Coin data are sent to ThaiJam's Cloudflare services and linked to your
   ThaiJam account.
2. **iCloud audio backup.** If enabled, imported audio and artwork are stored in your private
   CloudKit database. ThaiJam cannot read that private database and keeps no server copy.
3. **Content updates.** The app downloads public learning content from ThaiJam's content service.
   The request includes a random installation identifier for downloads and error handling. Cards,
   study history, songs and lyrics are not sent to the content-update service.
4. **Lyric search.** The song title and artist you enter are sent to
   [LRCLIB](https://lrclib.net). No ThaiJam identifier is attached.
5. **Apple Music.** If authorized, MusicKit searches Apple's catalog, fetches basic track details
   and plays music. [Apple's privacy policy](https://www.apple.com/legal/privacy/) applies.
6. **Spotify.** Search text is sent to Spotify's Web API. The authorization token stays in the
   device Keychain. When iCloud audio backup is enabled, your Client ID is stored in iCloud KVS;
   Spotify authorization itself must be granted separately on each device. A selected track ID is
   included in song data and reaches ThaiJam's servers only when cross-device sync is enabled.
   App Remote lets Spotify play audio while ThaiJam reads the current track and playback position
   to align local lyrics. [Spotify's privacy policy](https://www.spotify.com/legal/privacy-policy/) applies.
7. **Shazam.** After you choose Identify song and allow microphone access, ShazamKit matches an
   audio signature. ThaiJam does not keep or upload the raw recording. Apple's terms apply.
8. **Pronunciation assessment.** After you record and submit up to 10 seconds of speech, the audio
   and Thai reference text are sent through ThaiJam's Cloudflare Workers to Microsoft Azure Speech.
   The recording is buffered temporarily and deleted after submission or when you leave the screen.
   Neither ThaiJam nor the assessment service writes the recording or recognized text to a database.
   The returned score and recognized text remain locally; if cross-device sync is enabled, only the
   score and timestamp sync to ThaiJam. [Microsoft's privacy statement](https://privacy.microsoft.com/privacystatement) applies.
9. **AI text features.** These are described in the next section.

Read-aloud, Apple Translation, word segmentation and tracing scores run on the device.

## AI text features

Text leaves the device only when you choose song analysis, dictionary lookup, an AI explanation or
extra examples.

| Feature | Text sent |
| --- | --- |
| Song analysis | Lyrics you provide, after repeated choruses and section labels are removed |
| Dictionary lookup | The Thai term you enter |
| AI explanation | The Thai text on that card |
| Extra examples | The built-in pattern formula, explanation and existing examples |

The text first reaches ThaiJam's Cloudflare Workers and is then forwarded to the
[OpenAI API](https://openai.com/policies/privacy-policy). ThaiJam authenticates your request with
your account session for credits, rate limiting and abuse prevention. The content forwarded to
OpenAI contains no Apple or Google identifier, email address or other direct identifier.

These AI text features do not send your study history, decks, imported audio or artwork.
Pronunciation audio goes to Azure Speech, not OpenAI.

### AI result cache

AI-generated results may be cached for seven days under a hash of the submitted content. Another
user can receive the same result only by submitting identical content. Original lyrics are not
stored in this cache, cached results carry no account or email identifier, and there is no interface
for browsing or searching cached results.

AI translations and explanations can be wrong. You can edit saved cards and report a problem from
the relevant result in the app.

## ThaiJam account, sign-in and purchases

The anonymous account stores a random user ID, credit balance and history, Study Coin data and
server-backed feature records. If you link Apple or Google, ThaiJam also stores the provider-specific
user ID and an email address you choose to share. It does not receive your Apple or Google password,
real name or payment details. App Store payments are handled by Apple; ThaiJam receives a transaction
identifier needed to credit the purchase and handle refunds.

Google sign-in is handled by Firebase Authentication. Google therefore learns that the selected
Google account signed in to ThaiJam, and Firebase holds its authentication record. ThaiJam uses only
Firebase Authentication—not Firebase Analytics or Crashlytics. Sign in with Apple uses Apple's
native iOS flow and does not pass through Firebase. [Google's privacy policy](https://policies.google.com/privacy) applies.

### Export your data

Profile → Account settings → Export my data downloads a machine-readable JSON file containing study
data held by ThaiJam, Study Coin data, the AI credit ledger and purchase records. It excludes imported
media, original Apple or Google identifiers, and deleted items. Contact support if you need a broader
access request covering internal account fields.

### Delete your account

Profile → Account settings → Delete account works for anonymous and signed-in accounts and does not
require contacting support.

Deletion closes the active ThaiJam account and removes any Apple or Google sign-in link, email,
App Attest device-key information, feedback, remaining AI Credits, and the server copy of cards,
study progress, songs, lyrics, AI results and Study Coin data.

Purchase, credit-spending and related service records are retained in **pseudonymized form for five
years**, then deleted automatically. They retain no link to a sign-in account and are kept for tax
recordkeeping and delayed App Store refund reconciliation.

Local data on the device is not deleted. Imported audio and artwork in your private iCloud database
are also unaffected, but your data will no longer have a ThaiJam server copy.

## Permissions

| Permission | When it is used | Effect of declining |
| --- | --- | --- |
| Notifications | Local reminders when cards are due | Only reminders are disabled |
| Files | Import audio or a flashcard CSV you select | Only the import is unavailable |
| Photos | Select song artwork | Only photo selection is unavailable |
| Media and Apple Music | Search or play Apple Music after you enable it | Only Apple Music integration is unavailable |
| Microphone | Identify nearby music with ShazamKit or submit a pronunciation recording | Only those two features are unavailable |

ThaiJam does not use the camera, location, contacts or health data.

## Children and minors

ThaiJam is not primarily directed at children. AI Credit purchases use Apple's in-app purchase system
and remain subject to Screen Time, Ask to Buy and other parental controls. ThaiJam cannot bypass those
controls. Refund requests can be made through [Apple's refund process](https://support.apple.com/HT204084).

## Export, transfer and backup

- A CSV created by Export backup is stored or shared only where you choose; ThaiJam does not upload it.
- Cross-device sync stores selected study data on ThaiJam's Cloudflare services.
- iCloud audio backup stores imported audio and artwork in your private CloudKit database. Local app
  data may also be included in iCloud device backup if you enable that Apple feature.

## Content reports

Copyright owners and users can report problematic content to `support@thaijam.app`. AI-generated
content in the app also includes a problem-reporting action.

## Changes and contact

When this policy changes, the date at the top will be updated and the revised policy will be released
with the corresponding app version.

Questions or privacy requests: `support@thaijam.app`

---

*This policy describes ThaiJam's current behavior. Material changes to data handling will be
documented before release.*
