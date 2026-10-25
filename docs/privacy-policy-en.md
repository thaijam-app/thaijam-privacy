---
permalink: /privacy-policy-en/
---

# ThaiJam Privacy Policy (iOS)

**Last updated: 26 October 2026**

[繁體中文](/privacy-policy/) | [简体中文](/privacy-policy-zh-cn/)

> This page applies to the **iOS version**. The Android version has a
> [separate policy](/privacy-policy-android-en/) because it has no iCloud backup.

## In one sentence

ThaiJam does **not** sell your data. The only ads are rewarded ads you choose to watch, served by
Google AdMob (see "Ads: watching an ad for cans"); we don't give advertisers your account or learning data. Most data
starts on your device. Depending on the features you choose, the app may connect to ThaiJam's
servers, your private iCloud database, lyric and music services, or the **third-party AI providers**
that process content for AI and speech features, as described below. **The one connection that does not wait for
you to do anything is the launch-time fetch of the social invitation card's content** (item 4 under
outbound network connections) — that request carries no account, no device identifier and no study
data.

## Data we collect and store

On first launch, ThaiJam asks you to choose between **starting to learn straight away** and
linking an Apple or Google account. If you choose to start straight away, ThaiJam creates a
random **anonymous ThaiJam account identifier and session** — this lets server-backed features
work without asking for your name or email. If you choose to sign in, no anonymous account is
created. Most on-device features do not require Apple or Google sign-in. You must link Apple or Google before buying
AI Credits or using the same ThaiJam account reliably on another device. Spotify uses its own
authorization page.

ThaiJam includes Google AdMob only for rewarded ads (see "Ads: watching an ad for cans") and has no third-party
analytics package. It does not record which
screens you open or how long you spend on them. AI service usage records are described under
“AI usage records.”

| Data | Where it is stored | Purpose |
| --- | --- | --- |
| Study results, review schedule, streak activity, and which learning-map lessons you finished with their quiz scores | On-device database; ThaiJam servers if cross-device sync is enabled | Schedule reviews and continue on another device |
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

The anonymous identifier is created only when you choose to start without signing in. It
contains no name, email address, or provider account. It is persistent and is associated with
server-backed data. If you later sign in with Apple or Google, ThaiJam
attempts to link that provider to the same user ID so your existing data is preserved. If the
provider already belongs to another ThaiJam account, the app asks before switching and does not
merge the two server accounts automatically.

## Data from features added in 1.1

The features below belong to your ThaiJam account and are stored on ThaiJam's servers.
**None of them stores recordings.**

### Topic missions: plans and answer records

| Data | Purpose |
| --- | --- |
| Which dramas you picked, which one you are studying now, your daily pace and, if you set one, your departure or target date | Pick "today's step" and continue across your devices |
| A record for each answer: mission and question IDs, how you answered (spoken, typed, word tiles, fill-in, choice), result, stars, hints used, time, content version | Continue progress, schedule next-day checks, award ability badges and Study Coins |
| Ability badges you earned: which badge, when, how you earned it (spoken or typed), and the IDs of the answer records it rests on | Keep your badges on a new device or after reinstalling; never pay the same badge twice |

Answer records **contain no recordings and none of the words you said or typed** — only the result.

### Personal study set (ThaiJam Max)

Something is saved only when you tap "Save to study set". A saved item holds:

- the lesson IDs it refers to (the lesson content itself is not copied)
- **what you said (the speech-recognition text) or typed**, exactly as it was — this can include personal details such as a name you said during practice
- the feedback, stars and hints for that answer, plus any title and note you wrote
- for a before/after comparison, the IDs of the two answer records

**Recordings are not saved.** Your study set is **visible only to you** and never appears in the weekly community or any public page. You can delete any item, export selected items as text, and everything is deleted with your account. If your plan ends, saved items stay readable and deletable; you just can't add new ones.

### Backpack and tickets

| Data | Purpose |
| --- | --- |
| The tickets you hold (trial, make-up check-in, double coins, card pack, outfit) — source, quantity and expiry of each batch | Keep them on every device |
| Each time a ticket is received, used or expires; when double coins are active; trial history | Prevent double claims or double use; support requests |
| When ThaiJam grants tickets: the staff member and the reason | Internal audit. Audit records do not contain your email |

For redeem codes, the server stores only a hash of the code and who redeemed it, not the code itself.

### Inviting friends

- Your invite code is linked to your account (stored as-is so it can be shown to you).
- When someone enters your code, we record who invited whom and the rewards given; for the invited person we keep only the dates they studied, to check whether the reward threshold was reached.
- To stop one device from claiming twice: iOS uses Apple's DeviceCheck (ThaiJam stores no device identifier); for Android see the Android policy.
- When you delete your account: your study dates are deleted at once; your invite code is deleted or disabled and can no longer be used; the record of who invited whom is kept in pseudonymized form for **one year**, then deleted. Rewards the other person already received are not taken back.

### Weekly community topics

**Your results are private by default.** They become public only when you choose to share, look at the preview and confirm. A shared card can **only** contain:

- the name of the mission or ability badge
- optionally, your nickname, a Jammy avatar and one preset reflection

A card **cannot** contain free text, recordings, photos, your answers, study dates or account identifiers; nothing from your personal study set appears in the community.

| Data | Notes |
| --- | --- |
| Your shares, the encouragement you give to others, your vote for next week's topic | Fixed options only; one encouragement per share and one vote per week, both changeable |
| Who you blocked | Only you know; once blocked, neither of you sees the other |
| Reports (fixed reasons) and moderators' decisions | Deleted automatically after **one year** |

Withdrawing a share removes only the public card, not your private progress or badges. When you delete your account, your shares, encouragement and votes are removed; in reports and moderation records still within their retention period, your account is replaced by an identifier that cannot be traced back to you.

### Drama audio

- Pre-recorded lines are downloaded from ThaiJam's servers and cached on your device (up to 200 MB; the least recently used files are removed first). **These downloads carry no account or identifier.**
- Lines without a recording are synthesized on demand by ThaiJam's server: only **the Thai line from the lesson and the voice gender** are sent, then passed to a third-party AI provider for speech synthesis. Results are cached by content hash with no account attached. To prevent abuse, this request needs a signed-in account and app verification, and counts toward a daily limit.
- Lines that would contain your own name are **never read aloud**, so your name is never sent for synthesis.

### AI conversations and custom role-play

- During a conversation, your **recording and the recognized text** are sent through ThaiJam's server to third-party AI providers to recognize what you said and produce Jammy's reply and voice. Recordings are **not** stored.
- When a conversation finishes, we keep its **text transcript** (what both sides said), the number of turns, pronunciation and fluency scores, and the phrases you practised, so you can review it in your conversation history and learning report and continue on another device.
- Custom role-play also keeps the role, goal and constraint you chose and which part you reached.
- These records are **visible only to you** and are deleted with your account.

### Push notifications

Only after you allow notifications. To deliver them we keep:

| Data | Purpose |
| --- | --- |
| This device's push token (issued to the app by Apple or Google), platform, app language and time zone | Deliver to the right device, in your language, at a suitable time |
| Whether you agreed to **service notifications** (support replies, rewards) and to **promotional notifications**, and when you agreed to the latter | Send only the kinds you agreed to; promotional notifications are off by default |
| Which device each notification was sent to and whether it was delivered | Avoid duplicates and troubleshoot delivery |

Notifications are written by ThaiJam and delivered through Apple's push service (iOS) or Google's push service (Android). You can turn them off at any time in system or app settings; tokens and delivery records are deleted with your account.

### Lock-screen streak countdown (iOS Live Activity)

If you turn on the streak countdown, we keep this device's Live Activity token, time zone, language, how many hours ahead to remind you, and today's goal, answers and streak, to update the countdown on the Lock Screen and Dynamic Island. Turning it off stops updates; it is deleted with your account.

### Collectible cards: nearby landmarks and QR cards

- **Nearby landmarks:** if you turn this on and allow location "While Using the App", the app checks **on your device** whether you are near a landmark and unlocks that exploration card when you arrive. **Your coordinates never leave the device**; the server records only which card you got, when, and how (for example "landmark"). The app does not track your location in the background.
- **QR cards:** when you scan an event or partner QR card with the camera, the image is recognized on the device and only the code inside the QR is sent to the server to verify and grant the card.

### Card leaderboard and nickname

- The leaderboard scores the cards you collect. **It is anonymous by default**: others see only "Anonymous player" and a number that cannot be traced to your account.
- Only if you **turn on "Show on leaderboard"** in your profile can other users see your nickname and the Jammy avatar card you chose.
- At the end of a season the top places are frozen as that season's results to grant reward cards; your results are deleted with your account.

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

ThaiJam does not use any third-party analytics or crash-reporting SDK, and it
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
   AI results and Study Coin data are sent to ThaiJam's servers and linked to your
   ThaiJam account.
2. **iCloud audio backup.** If enabled, imported audio and artwork are stored in your private
   CloudKit database. ThaiJam cannot read that private database and keeps no server copy.
3. **Content updates.** The app downloads public learning content from ThaiJam's content service.
   The request includes a random installation identifier for downloads and error handling. Cards,
   study history, songs and lyrics are not sent to the content-update service.
4. **In-app social invitation card.** On launch the app fetches what the card shows — text, links and
   (if any are configured) one or more images — from ThaiJam's server, so that changing a line of copy does not
   require an app update. **The request carries no account, no device identifier and no study data**,
   and the response is identical for every user. The result is stored on the device and reused when
   offline; if it has never been fetched, the app shows its built-in version — so the card stays
   complete and dismissible with no network. **This is not third-party advertising.** Today the card
   carries only ThaiJam's own content, such as our social account. In future it may carry content
   from creators we collaborate with; when it does, the card is labelled "Partner" so you can tell
   it apart from our own. Either way: no ad SDK involved, no advertising identifier used, no record of
   whether you saw or tapped it, and the image is served from ThaiJam's own storage — seeing the
   card never connects you to someone else's server.
5. **Lyric search.** The song title and artist you enter are sent to
   [LRCLIB](https://lrclib.net). No ThaiJam identifier is attached.
6. **Apple Music.** If authorized, MusicKit searches Apple's catalog, fetches basic track details
   and plays music. [Apple's privacy policy](https://www.apple.com/legal/privacy/) applies.
7. **Spotify.** Search text is sent to Spotify's Web API. The authorization token stays in the
   device Keychain. When iCloud audio backup is enabled, your Client ID is stored in iCloud KVS;
   Spotify authorization itself must be granted separately on each device. A selected track ID is
   included in song data and reaches ThaiJam's servers only when cross-device sync is enabled.
   App Remote lets Spotify play audio while ThaiJam reads the current track and playback position
   to align local lyrics. [Spotify's privacy policy](https://www.spotify.com/legal/privacy-policy/) applies.
8. **Shazam.** After you choose Identify song and allow microphone access, ShazamKit matches an
   audio signature. ThaiJam does not keep or upload the raw recording. Apple's terms apply.
9. **Pronunciation assessment.** After you record and submit up to 10 seconds of speech, the audio
   and Thai reference text are sent through ThaiJam's server to a third-party AI provider.
   The recording is buffered temporarily and deleted after submission or when you leave the screen.
   Neither ThaiJam nor the provider writes the recording or recognized text to a database.
   The returned score remains locally; if cross-device sync is enabled, only the score and timestamp
   sync to ThaiJam.
10. **AI text and speech features.** These are described in the next section.
11. **Speech recognition for speaking practice.** Speaking exercises (topic missions, example
    fill-in, guided speaking) use Apple's speech recognition to turn your Thai into text. As Apple
    designs it, recognition may happen on the device or on Apple's servers;
    [Apple's privacy policy](https://www.apple.com/legal/privacy/) applies. ThaiJam uses only the
    recognized text to check your answer and does not keep the recording.
12. **Push notifications.** See "Push notifications" above.

Read-aloud, Apple Translation, word segmentation and tracing scores run on the device.

## Ads: watching an ad for cans

From version 1.2, ThaiJam has **rewarded ads**. An ad plays only when you tap "Watch an ad", and finishing it
gives you cans to exchange for in-app items. There are no banner ads and no ads inside lessons. Every learning
feature works without watching ads. Only accounts linked to Apple or Google can watch ads.

**Ads are served by Google AdMob.** When you open a screen that offers an ad (the cans card in the shop, the
pronunciation check after you run out, cans in your backpack), the app preloads one ad from AdMob and discards it
when you leave. If you never open those screens, the app does not connect to AdMob.

While loading and showing an ad, Google may collect and process:
- your IP address and the approximate location derived from it
- basic device and app information (such as model, OS version, language and app version)
- **your advertising identifier (IDFA), only if you allow it in the "Allow tracking" prompt**
- your interaction with the ad (such as whether you finished or tapped it), and diagnostics such as crash and performance data

Google uses this data to provide, measure and improve ads and to prevent fraud, as described in the
[Google Privacy Policy](https://policies.google.com/privacy) and
[How Google uses information from sites or apps that use its services](https://policies.google.com/technologies/partner-sites).

**We do not give Google your ThaiJam account ID, email, nickname or learning data.**
Cans are credited only when AdMob's servers notify ThaiJam; that notification carries a token issued by ThaiJam
that contains no identity. Our server keeps the transaction number and time to prevent double credits and to
count the daily limit. Your cans history is part of your account data: you can export it, and it is deleted with
your account.

**Your choices:**
- In the European Economic Area, the UK, Switzerland and similar regions, Google's consent form appears before
  your first ad; you can change your choice later from "Privacy options" in the cans shop.
- Before your first ad, the app explains why and asks whether to allow tracking. **If you decline, you can still
  watch ads and still get cans**; the ads just won't be chosen by your interests. You can change this later in
  Settings → Privacy & Security → Tracking. We never offer cans or any other reward in exchange for your consent.

## AI features: where your content goes

Content leaves the device only when you use one of the AI or speech features below.

**We ask for your consent before the first use.** Until you agree, no recording or text is sent to third-party AI providers; if you decline, AI features stay off and the rest of the app works as usual. You can turn it on or off at any time in Settings → About. (Example sentences, Jammy quizzes and line playback use only built-in course content, contain nothing of yours, and do not need this consent.)

| Feature | What is sent |
| --- | --- |
| Song analysis | Lyrics you provide, after repeated choruses and section labels are removed |
| Dictionary lookup, AI explanation | The Thai you enter or the Thai on that card |
| Extra examples, Jammy quizzes | Built-in lesson content (none of your data) |
| AI conversation, custom role-play | Your recording, the recognized text and the conversation so far |
| Pronunciation assessment | Up to 10 seconds of audio and the reference text |
| Reading lines and examples aloud | The Thai from the lesson and the voice gender |

Content first reaches ThaiJam's server and is then forwarded to **third-party AI providers** to
produce the result (translation, analysis, reply, voice or score). ThaiJam authenticates your request
with your account session for credits, rate limiting and abuse prevention. The content forwarded to
AI providers contains **no ThaiJam account ID, Apple or Google identifier, email address or other
direct identifier** — only what the table lists.

Not sent to AI providers: your study history, review progress, decks, imported audio or artwork.

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

Google sign-in is handled by Google's authentication service, so Google learns that the selected
Google account signed in to ThaiJam and keeps an authentication record;
[Google's privacy policy](https://policies.google.com/privacy) applies. Sign in with Apple uses
Apple's native iOS flow; [Apple's privacy policy](https://www.apple.com/legal/privacy/) applies.

### Plus and Max subscriptions

Subscriptions are bought and renewed through the App Store (iOS) or Google Play (Android). **Payment details are handled by Apple or Google; ThaiJam never receives them.** To know which plan you have and how long you have been a member, we keep:

| Data | Purpose |
| --- | --- |
| Plan (Plus or Max), monthly or yearly, current status (active, grace period, billing retry, expired, revoked), start and expiry dates, whether it auto-renews | Decide which features you can use now |
| For each period: transaction ID, dates, offer type and the amount paid | Member-card months, offers and refund reconciliation |
| Apple transaction IDs and a hash of the signed payload; the Google Play order ID and a **hash of the purchase token** (not the token itself) | Verify the transaction with Apple or Google |
| Subscription notifications from Apple: notification ID, type, transaction ID, processing status and time | Reflect renewals, refunds and revocations promptly; this log does not contain your account |

When you buy on Google Play, the account reference we give Google is a **one-way hash** of your ThaiJam account, so Google never receives your ThaiJam account ID.

**Deleting your ThaiJam account does not cancel a subscription.** Cancel it first in App Store or Google Play subscription settings, or it will keep renewing. After deletion, subscription records are kept in pseudonymized form for **five years**, like purchase records, then deleted automatically.

### Export your data

Profile → Account settings → Export my data downloads a machine-readable JSON file containing study
data held by ThaiJam, Study Coin data, the AI credit ledger and purchase records, plus your topic-mission
plans and answer records, ability badges, personal study set, backpack tickets, weekly-community shares, and your Plus/Max subscription records
(plan, status, periods, amount paid and offers, auto-renew; not transaction IDs or token hashes). It excludes imported
media, original Apple or Google identifiers, and deleted items. Contact support if you need a broader
access request covering internal account fields.

### Delete your account

Profile → Account settings → Delete account works for anonymous and signed-in accounts and does not
require contacting support.

Deletion closes the active ThaiJam account and removes any Apple or Google sign-in link, email,
App Attest device-key information, feedback, remaining AI Credits, and the server copy of cards,
study progress, songs, lyrics, AI results and Study Coin data. Topic-mission plans and answer records,
ability badges, your personal study set, backpack tickets and redeem records, AI conversation and
custom role-play records, push and Live Activity tokens, and leaderboard results and nickname are
deleted too, and your
weekly-community shares, encouragement and votes are removed (see "Weekly community topics" for reports).

Purchase, credit-spending and related service records (including Plus/Max subscription records) are
retained in **pseudonymized form for five years**, then deleted automatically. Records of who invited
whom are kept in pseudonymized form for **one year** (to stop the same person deleting and re-registering
to claim invite rewards again), then deleted automatically. They retain no link to a sign-in account and are kept for tax
recordkeeping and delayed App Store refund reconciliation.

Local data on the device is not deleted. Imported audio and artwork in your private iCloud database
are also unaffected, but your data will no longer have a ThaiJam server copy.

## Permissions

| Permission | When it is used | Effect of declining |
| --- | --- | --- |
| Notifications | Local review reminders; once allowed, also ThaiJam's service notifications and any promotional notifications you opt into (see "Push notifications") | Only notifications are disabled |
| Files | Import audio or a flashcard CSV you select | Only the import is unavailable |
| Photos | Select song artwork | Only photo selection is unavailable |
| Media and Apple Music | Search or play Apple Music after you enable it | Only Apple Music integration is unavailable |
| Microphone | Identify music with ShazamKit, pronunciation assessment, speaking practice or AI conversations | Only features that need speech are unavailable |
| Speech recognition | Turn your spoken Thai into text in speaking practice | You can answer by typing or with word tiles instead |
| Location (while using the app) | Nearby-landmark cards, checked on the device; coordinates never leave it | Only nearby landmarks are unavailable |
| Camera | Scan QR cards; the image is recognized on the device | Only QR scanning is unavailable |
| Tracking (App Tracking Transparency) | Before your first ad for cans; if you allow it, Google may use your advertising identifier to choose ads (see "Ads: watching an ad for cans") | You can still watch ads and get cans |

ThaiJam does not track your location in the background and does not use contacts or health data.

## Children and minors

ThaiJam does not collect children's personal data for advertising. Its only third-party ads are rewarded ads users choose to watch (see "Ads: watching an ad for cans"), and it has no third-party analytics SDK; the only other promotional content is the in-app invitation card described under outbound network connections — today it carries only ThaiJam's own content, and content from collaborating creators would be labelled as such. ThaiJam is not primarily directed at children. AI Credit purchases use Apple's in-app purchase system
and remain subject to Screen Time, Ask to Buy and other parental controls. ThaiJam cannot bypass those
controls. Refund requests can be made through [Apple's refund process](https://support.apple.com/HT204084).

## Export, transfer and backup

- A CSV created by Export backup is stored or shared only where you choose; ThaiJam does not upload it.
- Cross-device sync stores selected study data on ThaiJam's servers.
- iCloud audio backup stores imported audio and artwork in your private CloudKit database. Local app
  data may also be included in iCloud device backup if you enable that Apple feature.

## Categories of service providers

We use the following categories of service providers to run the features above. They process data
only on our instructions and only to provide that feature:

| Category | Purpose |
| --- | --- |
| Cloud hosting and storage | Run ThaiJam's servers, store account and synced data, serve lessons and audio |
| Third-party AI providers | AI analysis and conversation, speech synthesis, pronunciation assessment |
| Sign-in (Apple, Google) | Let you sign in with an Apple or Google account |
| Payments (Apple, Google) | In-app purchases and subscriptions; payment details stay with them |
| Push delivery (Apple, Google) | Deliver notifications to your device |
| Lyric and music services | Only when you use song features (see outbound connections) |
| Advertising (Google AdMob) | Only when you watch an ad for cans; Google processes this data under its own privacy policy (see "Ads: watching an ad for cans") |

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
