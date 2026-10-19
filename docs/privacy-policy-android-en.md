---
permalink: /privacy-policy-android-en/
---

# ThaiJam Privacy Policy (Android)

**Last updated: 19 October 2026**

[繁體中文](/privacy-policy-android/) | [简体中文](/privacy-policy-android-zh-cn/)

> This page applies to the **Android version**. The iOS version has a [separate policy](/privacy-policy-en/)
> because the two platforms differ (Android has no iCloud backup), so data is handled differently.

## In one sentence

ThaiJam **does not sell your data or use it for ad tracking**. There is no advertising SDK,
**no third-party analytics and no crash-reporting tool** (AI usage is recorded; see "Usage records" below).

**Signing in with Google or Apple is optional.** If you choose "Start learning" on first launch, the app
creates an **anonymous account with no name or email**, so you can use server features without registering;
if you sign in, your Google or Apple account is used instead. **Either way, your study content is synced to
our servers** so you can switch phones or continue on another device. AI and speech features send the content
you submit to **third-party AI providers** for processing (see section 4).

## What we collect

### Anonymous account (when you choose "Start learning")

The app asks our server for an **anonymous account identifier**. It contains no name, email or anything that
points to you personally, but it is a persistent identifier, and the study content in parts 2 and 3 below is
linked to it. When you later sign in with Google or Apple, we link the sign-in to the same account where
possible so your existing data is kept.

### After you sign in with Google or Apple

**1. Your account identifiers**

- The **identifier** of your Google or Apple account (a string issued by them, **not your password**)
- That account's **email**

They give your study progress and AI credits an owner, so you can recover them on a new phone.
We do not use them for marketing email and do not share them with third parties.

If you choose "Hide My Email" when signing in with Apple, Apple gives us a forwarding address
(`@privaterelay.appleid.com`) and **we never see your real inbox**.

**2. Your study content**

The following is uploaded to our servers and synced to your other devices signed in to the same account:

| Content | What exactly |
| --- | --- |
| Study records and review schedule | How often each card was right or wrong, when it is due next, which learning-map lessons you finished and their quiz scores |
| Flashcards you add or import | Thai, romanization, translation, part of speech, example sentences |
| Decks you create | Name, icon, colour |
| Lyrics and translations you paste | Thai, romanization, translation and timestamps for each line |
| Song details you create | Title, artist, Spotify link, length |
| Daily study count | How many questions you answered each day (heat map and streak) |
| Your state for course cards | Which cards you hid, moved to another deck or added to your word list |
| Renamed and recoloured official decks | The names and colours you gave official decks |
| AI word notes and song analysis results | AI results you paid credits for |
| Two study settings | **Only** daily review count and card colour scheme: the first affects daily-goal rewards, the second is bought with coins |
| Study coin history | Coins earned and spent, check-ins, colour schemes and icons bought |
| Hint tickets and streak shields | How many are left and how many you used |
| Pronunciation assessment summary | Number of attempts, best score, latest score and time. **Only these four numbers**; the recording itself is not kept (see section 7) |
| AI credit purchase records | Product ID, credits added, time and a **hash** of the purchase token. **No payment details** (see section 8) |

**The following is never uploaded and stays on this device:**

- **Song audio and artwork you import** (only text such as the title is synced, never the files)
- **All other display preferences**: romanization style, card front, appearance, text size, Thai font,
  notification time, speech speed and auto-play switches

Display preferences are deliberately not uploaded: they are choices you made **for that device**. A larger
text size on a tablet should not follow you to your phone.

Why study coins are uploaded: **they decide what you can buy.** Kept only on the device, switching phones
would throw away the coins you earned, and only the server can stop the same coins being spent twice on two devices.

**3. Features added in 1.1**

All of the following is stored on our servers under your account. **None of it keeps a recording.**

| Feature | What is stored |
| --- | --- |
| Topic mission plan | Which drama series you chose, which one you are on, your daily pace and (if you set it) your departure or use date |
| Topic mission answers | For each question: mission and question IDs, answer mode (speak, type, word blocks, fill-in, choice), result, stars, hints used, time and course version. **No recordings and nothing you said or typed** |
| Skill badges | Which badge, when, how it was earned (speaking or typing) and the answer record IDs used to verify it |
| Personal study set (ThaiJam Max) | **Saved only when you tap "Save to study set"**: the course item ID, **what you said (recognized text) or typed, kept as is, which may include a name you said**, feedback and stars, your own title and notes. No recordings. **Only you can see it**; it never appears in the community. You can delete items one by one or export them |
| Backpack and tickets | For each batch of tickets you hold (trial, make-up check-in, double coins, card pack, outfit): source, quantity, expiry, and claim, use and expiry records. When we issue tickets we record the staff member and reason; the audit record does not include your email. Redemption codes are stored only as hashes |
| Invite friends | Your invite code (stored as is so we can show it to you), who invited whom and the rewards given; for invited friends we record only the dates they studied, to check the reward threshold. To stop the same phone claiming twice we use the **one-way hashed device fingerprint** also used for the new-user bonus; it cannot be turned back into your phone's identity |
| AI conversation and custom role-play | After a conversation ends: the **text transcript** (what both sides said), number of turns, pronunciation and fluency scores and the sentences you practised; custom role-play also stores the role, goal, constraints and stage you reached. **Recordings are not kept.** Only you can see it |
| Push notifications | Only after you allow notifications: this phone's push token (issued to the app by Google), app language and time zone, whether you agreed to **service notices** (support replies, rewards arriving) and **promotional notices** (off by default) and when, and whether each notice was delivered. Notices are delivered through Google's push service |
| Collectible cards: nearby landmarks and QR cards | Nearby landmarks are checked **on your phone**; **your coordinates never leave it**. When you scan a QR card the image is recognized on the phone and only the code inside it goes to our server. The server records only which card you got, when and by which route |
| Card leaderboard and nickname | Scored by the cards you collect. **Anonymous by default**; others see your nickname and Jammy avatar card only if you turn on "Show on leaderboard" in your profile. Top places are frozen at the end of a season to award season cards |

**4. Plus / Max subscriptions (signed-in only)**

Subscriptions are bought and renewed through **Google Play**; **payment details are handled by Google and we never receive them**. We store:
plan (Plus / Max), monthly or yearly, current status (active, grace period, retrying payment, expired, revoked), start and end dates and whether it auto-renews;
for each period the transaction ID, dates, offer type and amount paid (for membership months and refund checks); the Google Play order ID and a **hash of the purchase token** (not the token itself).
The account reference we give Google is a **one-way hash** of your ThaiJam account, so Google never receives your ThaiJam account identifier.

**Deleting your ThaiJam account does not cancel a subscription.** Cancel it first in Google Play under "Payments & subscriptions", otherwise it renews and charges as usual.

**Official weekly community: your progress is private by default.** It is shown publicly only when you choose to share, see a preview and confirm.
A share card can **only** contain the mission or badge name and, if you choose, your nickname, Jammy avatar and one fixed comment.
It **cannot** contain free text, recordings, photos, your answers, study dates or account identifiers; your personal study set never appears in the community.
Cheers and votes use fixed options; only you know whom you blocked, and once blocked neither of you sees the other.
Reports (fixed reasons) and moderator actions are kept for **1 year** and then deleted. Withdrawing a share removes only the public card, not your private progress.

**Drama audio:** pre-recorded lines are downloaded from our servers to a cache on your phone (up to 200 MB);
**download requests carry no account or identifier**. Lines without a recording are synthesized by our server:
it sends only **that Thai line from the course and the voice gender** to a third-party AI provider; results are cached by content hash with no account attached.
Lines that would contain your name **are never read aloud**, so your name is never sent for synthesis.

### What we do not collect

**No advertising ID, and no background location tracking.**
The app does not record which screens you open, how long you stay or what you tap. There is no analytics or crash-reporting SDK.

### Usage records: AI requests are logged

**Every AI request leaves one record** linked to your account:

| What is recorded | Why |
| --- | --- |
| Which AI feature and which model | Accounting: the credits you are charged must match actual usage |
| Input / output token counts and cost | Our own cost control and daily budget limits |
| Success or failure and time | Failed requests are refunded; unusual frequency signals abuse |

We look at these **in aggregate** for daily request volume and cost, which is necessary to run the service.
**The records do not contain the content you sent.**

**One device identifier:** so that "questions answered per day" can be counted per device
(two devices studying on the same day should add up, not overwrite each other), the app
generates a **random number** and uploads it with your study count. It is random, belongs only to this app
and disappears when you uninstall; it is **not** your phone's identifier and cannot track you across apps.

## How long we keep data

- **Your account and study content: until you delete your account.**
- When you delete your account, the account, email, device credentials and **all study content** on the server are deleted,
  including topic mission plans and answers, skill badges, your personal study set, backpack tickets and redemption records, AI conversation and custom role-play records, push tokens and delivery records, and leaderboard places and nickname; your weekly community shares, cheers and votes are removed.
- **Invite records are an exception:** study dates are deleted immediately and your invite code is deleted or disabled; "who invited whom" is kept under a code that cannot identify you for **1 year** and then deleted
  (to stop deleting and re-registering to claim invite rewards again). Rewards the other person already received are not taken back.
- **Weekly community reports and moderator actions are an exception: kept for 1 year and then deleted.** After you delete your account, your account in records still within that period is replaced by an unidentifiable code.
- **Purchase and credit records (including Plus / Max subscription records) are an exception: kept for 5 years under a code that cannot identify you.**
  That is the retention period Taiwan's tax law sets for accounting records, and it also lets refund notices that arrive later
  still match the transaction. Those records contain **no** email, name or any field that identifies you:
  what remains is "a transaction of this amount happened", not "who bought it".
- Records flagged by abuse protection are kept for up to **2 years** (or until manually resolved),
  to stop the same person repeatedly using the free allowance.

## Getting a copy of your data

**You can export it in the app: Profile → Account → "Export my data".**

The data on our server that belongs to you is collected into a JSON file, saved wherever you choose, including the 1.1 topic mission records, skill badges, personal study set, backpack tickets, weekly community shares
and Plus / Max subscription records (plan, status, periods, amount paid and offers, auto-renewal; no order IDs or token hashes). Exporting does not delete or
change anything, and you can export again at any time.

The file **does not include** things that stay only on this phone (imported audio and artwork, display preferences),
because they were never uploaded. It also does not include raw sign-in identifiers; for those, email
`support@thaijam.app`.

## Deleting your data

**You can delete your account in the app: Profile → Account → "Delete account".**

This deletes the account, email and all synced study content on the server. It cannot be undone.

Other options:

- **Uninstalling the app** deletes all local data on this device but **does not** delete your account on the server;
  use the option above to delete the account.
- **Signing out** only clears this device's sign-in; your data stays on the server.
- You can also email `support@thaijam.app`.

## Network connections

These are the cases in which the app connects to the internet. Apart from the community invitation card (item 11, which carries no account or device identifier), each needs you to use the matching feature first.

### 1. Lyric search (no sign-in needed)

When you tap "Search lyrics" on a song page, the app sends **the title and artist you entered** to
[lrclib.net](https://lrclib.net) (a free public lyrics database). The lyrics that come back are shown to you
to confirm before anything is imported. **Without tapping that button this connection never happens.**

Only those two fields are sent: none of your study records, flashcards or device identifiers,
**and not your account or email (even when you are signed in)**. LRCLIB is a third-party service
and its own policy governs how it handles queries.

### 2. Sign-in

When you tap "Sign in with Google" or "Sign in with Apple", the app sends the identity credential they issue
to our server in exchange for a session. Without tapping, this connection does not happen.

**On Android both sign-in methods go through Google's identity service**, so **Google knows you signed in to ThaiJam with this account**
and keeps an account record (identifier, email, sign-in method) under [Google's privacy policy](https://policies.google.com/privacy).
Passwords are always entered on their pages; ThaiJam never sees them.

### 3. Study content sync

The app syncs the content in the table above with the server **when it opens, when it returns to the foreground and after you add or change content**
(the same for anonymous and signed-in accounts). After you sign out it stops.

### 4. AI credits and AI and speech features

Checking your credit balance and history, and entering a redemption code, send requests to our server.
Content leaves your phone only when you use one of the AI or speech features below.

**We ask for your consent before the first use.** Until you agree, no recording or text is sent to third-party AI providers; if you decline, AI features stay off and the rest of the app works as usual. You can turn it on or off at any time in Settings → About. (Example sentences, Jammy quizzes and line playback use only built-in course content, contain nothing of yours, and do not need this consent.)

**What is sent**

| Feature | What is sent |
| --- | --- |
| Song analysis | Lyrics you paste (after repeated choruses and section labels are removed) |
| Dictionary lookup, sentence breakdown | Thai you enter or that is on the card |
| Example sentences, Jammy quizzes | Built-in course content (none of your data) |
| AI conversation, custom role-play | Your recording, the recognized text and the earlier part of that conversation |
| Pronunciation assessment | Up to 10 seconds of recording and the Thai you are practising (see section 7) |
| Line and example playback | Thai from the course and the voice gender |

**Where it goes**

It goes first to ThaiJam's server, which forwards it to **third-party AI providers** to produce the result (translation, analysis, reply, speech or score).
ThaiJam verifies requests with your account session for credits, rate limits and abuse prevention,
but what is forwarded to AI providers **contains no account identifier, sign-in identifier, email or other information that directly identifies you**, only the content in the table above.

**Never sent to AI providers**: your study records, review progress, word list, decks, song audio or artwork.

**AI result cache**: to respond faster and keep results consistent, the system may temporarily cache
AI-generated results by content hash.

### 5. Account deletion

When you tap "Delete account" and confirm, the app sends a deletion request to our server.

### 5a. Speech recognition for speaking practice

Speaking exercises in topic missions, example fill-ins and pattern practice use the Android system speech recognition service (usually provided by Google) to turn your Thai into text.
Depending on the system, recognition may happen on the phone or on the recognition service's servers, under that service's privacy policy; ThaiJam uses only the recognized text to check your answer and keeps no recording.

### 5b. Push notifications

After you allow notifications, the app gets a push token from Google's push service and gives it to our server to send the notices you agreed to (see part 3 above). You can turn them off at any time in system or app settings.

### 6. Spotify search and playback (you set it up yourself; off by default)

**This exists only after you enter a Spotify Client ID in settings and link your account.** Without that,
the connection never happens; it is not on by default.

- Linking: the app opens the system browser at Spotify's sign-in page and **you authorize directly on Spotify's
  website**. ThaiJam never sees your Spotify password.
- Only one scope is requested: **`app-remote-control`** (controlling playback in the Spotify app).
  **It cannot read your playlists, listening history or profile**; those are separate scopes we do not request.
- Searching: only **the keywords you type** are sent, none of your study records, flashcards or ThaiJam account.
- What comes back is public track information (title, artist, album art, length, Spotify link),
  and we keep only the title, artist and track link of the track you **choose**.
- **Playback: the Spotify app plays the audio, not ThaiJam.** After you choose Spotify as the source on a song page and tap play,
  ThaiJam sends play, pause and seek commands through Spotify App Remote and reads **the current track and position**
  so the lyrics follow the music. ThaiJam **does not download or play** Spotify audio itself.
- The position is kept only in memory for scrolling lyrics; it is not written to a database
  or sent to ThaiJam's server.
- The authorization token is stored on this device; you can disconnect at any time in Settings → Spotify.

Spotify is a third-party service and its own policy governs how it handles requests.

### 7. Pronunciation assessment (you hold the record button)

Recording starts only while you **hold** the microphone button on a card page, for up to 10 seconds, and ends when you let go.
The recording exists only in memory (it is never written to a file); it is sent to our server, which forwards it
to a third-party AI provider for scoring.

- Only **that recording** and **the Thai word or sentence you are practising** are sent
- Only scores come back (overall, accuracy, fluency, completeness and per-word scores)
- **We do not store the recording or the recognized text.** Only the four numbers in the table above
  are kept
- Without holding that button there is no recording and no connection

### 8. Buying AI credits (you tap the buy button)

**Payment is handled entirely by Google Play. ThaiJam cannot see or receive your card number,
billing address or any payment details.**

After you tap buy and complete payment on Google Play's screen:

- The app sends our server only two things: **the product ID** and **the purchase token issued by Google Play**.
  No personal data beyond email, and certainly no payment details.
- Our server asks Google whether the purchase is genuine and the amount is right,
  and adds the credits to your account only after confirming.
- The purchase record kept is: transaction ID, order ID, product ID, credits added, time
  and a **hash of the purchase token** (SHA-256), **not the token itself**.
  The hash stops the same purchase being redeemed for credits twice.

Refunds are handled by Google Play. After you request a refund there, we receive the refund notice from Google
and take back the matching credits.

### 9. Apple Music (you link it yourself; off by default)

**This exists only after you link Apple Music on a song page.** It needs your own Apple Music subscription.

- Linking: the app opens **Apple's MusicKit authorization screen** and you agree directly in Apple's
  interface. ThaiJam never sees your Apple password.
- The **music user token** you get is **stored only on this device**; it is not sent to ThaiJam's
  server or synced to other devices.
- Searching: only **the keywords you type** are sent, none of your study records or flashcards.
- What comes back is public track information (title, artist, album art, length),
  and we keep only the track you **choose**.
- **Playback: Apple Music plays the audio; ThaiJam does not download it.**
  The app sends play, pause, seek and speed commands and reads the position so the lyrics follow the music.
  The position stays in memory and is not written to a database or sent to a server.

Apple Music is a third-party service and Apple's own policy governs how it handles requests.

### 10. Song recognition (you tap the button; uses the microphone)

After you tap song recognition on a song page and allow the microphone, the app **listens to music playing around you**
to find out which song it is.

- The app uses Apple's **ShazamKit** to turn what it hears into an **audio fingerprint on this device**;
  the fingerprint is sent for matching, **not the recording**.
- **The recording is not stored** and is not sent to ThaiJam's server.
- Only public information about the matched song comes back (title, artist, album art).
- Without tapping the button there is no recording. It stops when recognition ends or you leave the screen.

Matching is done by Apple / Shazam under their own policies.

### 11. Community invitation card in the app (no sign-in needed)

When the app starts it fetches the content of this card from our own server:
text, links and (if set) one or more images. That way we can change a line of campaign text without shipping an app update.

**This request contains no account, no email and no study records or flashcards.**
It carries the three headers the app sends with **every** request to our own server:
app version, platform (android) and interface language. No advertising ID, no SSAID
and nothing that identifies your device. The server returns the same content to every user.

Once fetched it is stored on your device and reused when offline; if it has never been fetched, the version built into
the app is shown, so the card is complete and can be closed even offline.

**This is not third-party advertising.** For now the card shows only ThaiJam's own content (such as our social accounts).
In future it may show content from **creators who work with ThaiJam**; in that case the card will be labelled "Partner"
so you can tell at a glance it is not ours.

Whoever's content it shows, four things hold: **no third-party advertising SDK, no advertising ID,
no record of how many times you saw or tapped it, and images are hosted on ThaiJam's own servers**,
so seeing the card never connects you to someone else's server.

### Everything else is offline

The course content (1,583 items), 1,727 pronunciation audio files and the Thai word-segmentation dictionary (21,654 words) are packaged
in the app. Pronunciation playback, word segmentation, tracing scores and romanization all happen on the device.

**Of the connections above, only item 11 (the community invitation card) needs nothing from you first**;
every other one needs you to use the matching feature.

## Permissions

| Permission | Use |
| --- | --- |
| Internet (`INTERNET`) | The connections listed above. |
| Notifications (`POST_NOTIFICATIONS`) | Review and streak reminders (scheduled on the device); once allowed, also ThaiJam's service notices and any promotional notices you separately agreed to (see part 3). Each can be turned off in settings; declining the permission does not affect other features. |
| Location (`ACCESS_FINE_LOCATION`, `ACCESS_COARSE_LOCATION`) | "Nearby landmarks" for collectible cards, used only while the app is in use to check on the phone whether you are near a landmark; **coordinates never leave the phone**. Declining only turns off nearby landmarks. |
| Camera (`CAMERA`) | Scanning QR cards; the image is recognized only on the phone. Declining only turns off QR scanning. |
| File access | **The app declares no storage permission.** Importing a flashcard CSV or song audio uses the Android system file picker, where you choose one file; the app can read only that file and nothing else. Song audio is **copied** into the app's private storage (access from the system picker can expire at any time, and without a copy the song would stop playing) and deleted when you delete the song. |
| Microphone (`RECORD_AUDIO`) | **Always started by you**: pronunciation assessment (see 7), speaking practice (see 5a), AI conversation and custom role-play (see 4), and song recognition (which sends an **audio fingerprint** computed on the phone, see 10). The app does not ask for it at launch; declining only turns off features that need speaking. |

**No background location tracking, and no use of contacts or health data.**

## Children and minors

The app is not directed primarily at children; its age rating is shown by Google Play based on the content rating questionnaire and
local standards. ThaiJam does not collect personal data for advertising (the app has no third-party ads
and no third-party analytics; the only promotional content is the in-app invitation card, which currently shows only ThaiJam's
own content and will be labelled if it shows partner creators' content in future; see item 11 under "Network connections").

Purchases in the Android version (AI credits and Plus / Max subscriptions) are always processed through
Google Play billing, and purchases by minors are subject to Google Play's parental controls
(parents can require authentication for purchases); we do not and cannot bypass these settings.
See "8. Buying AI credits" above for how purchase data is handled.

## Categories of service providers we use

To provide the features above we use service providers in the following categories. What each one receives is described under the matching feature above:

| Category | Use |
| --- | --- |
| Cloud hosting and storage | Running ThaiJam's servers, storing account and sync data, delivering course content and audio |
| Third-party AI providers | AI analysis and conversation, speech synthesis, pronunciation assessment (see 4) |
| Sign-in services (Google, Apple) | Signing in with your Google or Apple account |
| Payments (Google Play) | In-app purchases and subscriptions; payment details are handled by Google and never reach ThaiJam |
| Push service (Google) | Delivering notices to your phone |
| Lyric and music services | Only when you use song features (see 1, 6, 9 and 10) |

## Changes

If this policy changes, we update the date at the top of this page and publish it with the new app version.

## Contact

For any questions email: `support@thaijam.app`

---

*This policy describes what the Android version of ThaiJam **actually does today**. If we change how data is handled,
we will update this policy before the change ships.*
