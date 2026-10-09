---
permalink: /privacy-policy-android-en/
---

<!--
  English translation of privacy-policy-android.md. The Chinese page is the
  source of truth: change that one first, then bring this one in line.
-->

# ThaiJam Privacy Policy (Android)

**Last updated: 1 September 2026**

[繁體中文版](/privacy-policy-android/)

> This page applies to the **Android version**. The iOS version has a
> [separate policy](/privacy-policy-en/) because the two platforms offer different
> features (Android has no iCloud backup), so data is handled differently.

## In one sentence

ThaiJam does **not** sell your data or use it for advertising or tracking. There are no
ad SDKs, **no third-party analytics and no crash reporting tools** (AI feature usage is
logged; see "Usage records" below).

**Signing in is optional, and it decides one important thing:** if you don't sign in,
the app runs entirely on your device and nothing is uploaded. **Once you sign in, your
learning content is synced to our servers** so you can continue on a new phone or
another device. You can sign in with **Google or Apple**.

## What we collect

### Not signed in: nothing

No data leaves your device. Lessons, audio and the Thai word-segmentation dictionary
are all bundled in the app.

### After signing in with Google or Apple

**1. Your account identifiers**

- The **identifier** of your Google or Apple account (a string issued by that provider,
  **not your password**)
- That account's **email address**

These let your learning progress and AI credits belong to you, so you can recover them
on a new phone. We do not use them for marketing emails and do not share them with
third parties.

If you choose "Hide My Email" when signing in with Apple, Apple gives us a forwarding
address (`@privaterelay.appleid.com`) and **we never see your real email address**.

**2. Your learning content (only exists after you sign in)**

The following is uploaded to our servers (Cloudflare) and synced to your other devices
signed in to the same account:

| Content | What exactly |
| --- | --- |
| Learning records and review schedule | How many times you got each card right or wrong, when it is next due, which lessons on the learning map you completed and your quiz scores for them |
| Flashcards you add or import | Thai, romanization, translation, part of speech, example sentences |
| Decks you create | Name, icon, colour |
| Lyrics and translations you paste in | Line-by-line Thai, romanization, translation, timestamps |
| Song information you create | Title, artist, Spotify link, duration |
| Daily study amount | How many questions you answered each day (for the heatmap and streak) |
| Your state on built-in cards | Which cards you hid, moved to another deck, or added to your new-words list |
| Renamed or recoloured built-in decks | The names and colours you gave built-in decks |
| AI word notes and song analyses | AI results you paid credits for |
| Two learning settings | **Only** cards reviewed per day and card colour theme — the first affects daily-goal rewards, the second is bought with coins |
| Learning coin transactions | Coins earned and spent, check-ins, which colour themes and icons you bought |
| Hint tickets and streak shields | How many you have left and how many you used |
| Pronunciation score summary | Number of attempts, best score, latest score and time. **Only these four numbers** — the recording itself is never stored (see "7. Pronunciation assessment" below) |
| AI credit purchase records | Product ID, credits added, time, and a **hash** of the purchase token. **No payment details at all** (see "8. Buying AI credits" below) |

**The following is never uploaded and stays on this device:**

- **Audio files and cover images you import** (only text such as the song title is
  synced, not the files themselves)
- **All other display preferences:** romanization style, card front, light/dark
  appearance, text size, Thai font, notification time, speech speed and the auto-play
  switches

Display preferences are deliberately not uploaded — they are choices you made **for that
device**. A larger text size on your tablet should not follow you to your phone.

Why learning coins are uploaded: **they decide what you can buy.** If they only lived on
the device, switching phones would throw away the coins you earned, and only the server
can stop the same coins from being spent once on each of two devices.

### What we do not collect

**No advertising ID and no location.**
The app does not record which screens you open, how long you stay or what you tap.
(Sign-in uses Firebase Authentication, but **only the sign-in module** — no Analytics,
no Crashlytics; see "2. Sign-in" below.)

### Usage records: each AI request is logged

**Every AI feature request leaves a record** tied to your account:

| What is recorded | Why |
| --- | --- |
| Which AI feature and which model was used | Reconciliation: the credits you are charged must match actual usage |
| Input/output token counts and cost | Our own cost control and daily budget cap |
| Success or failure, and time | Failed requests are refunded; unusual frequency is a sign of abuse |

We look at these in **aggregate** to see daily request volume and cost — this is
necessary to keep the service running. **The records do not contain the content you sent.**

**One device identifier (only after signing in):** so that daily study counts can be
tracked per device (two devices studying on the same day should add up, not overwrite
each other), we generate a **random ID** for this app and upload it with your study
counts. It is random, belongs only to this app and disappears when you uninstall. It is
**not** your phone's identifier and cannot be used to track you across apps.

## How long we keep data

- **Your account and learning content: until you delete your account.**
- When you delete your account, your account, email, device tokens and **all learning
  content** on the server are deleted together.
- **Exception — purchase and credit records are kept for 5 years under a pseudonym that
  cannot be traced back to you.** That is the retention period for accounting records
  under Taiwan tax law, and it also lets refund notices that arrive later still match
  their transaction. These records **do not contain** your email, name or any field that
  identifies you — what remains is "a transaction of this amount happened", not "who
  made it".
- Records flagged by abuse protection are kept for up to **2 years** (or until manually
  resolved) — to stop the same person from repeatedly claiming free allowances.

## Getting a copy of your data

**You can export it in the app: Me → Account → Export my data.**

This gathers the data on our servers that belongs to you into a JSON file, and you choose
where to save it. Exporting does not delete or change anything, and you can export again
at any time.

The file **does not include** things that only ever lived on this phone (imported audio,
cover images, display preferences) — they were never uploaded. It also does not include
the raw sign-in identifiers; if you need those, email `support@thaijam.app`.

## Deleting your data

**You can delete your account in the app: Me → Account → Delete account.**

This deletes your account, email and all synced learning content on the server. It
cannot be undone.

Other options:

- **Uninstalling the app** deletes all local data on this device, but **does not**
  delete your account on the server — use the option above for that.
- **Signing out** only clears the sign-in state on this device; your data on the server
  remains.
- You can also email `support@thaijam.app`.

## Network connections

Without signing in there are two: lyrics search (only when you tap the button), and
fetching the social invitation card's content at launch (item 11 — no account, no device
identifier).

### 1. Lyrics search (no sign-in needed)

When you tap "Search lyrics" on a song page, the app sends **the title and artist you
entered** to [lrclib.net](https://lrclib.net) (a free public lyrics database). The
returned lyrics are shown to you first, and you decide whether to import them. **No tap,
no connection.**

Only those two fields are sent — not your learning records, flashcards or device
identifier, **and not your account or email (even if you are signed in)**. LRCLIB is a
third-party service; how it handles queries is governed by its own policy.

### 2. Sign-in

When you tap "Sign in with Google" or "Sign in with Apple", the app sends the identity
credential issued by that provider to our own server (Cloudflare) in exchange for a
session. No tap, no connection.

**Both sign-in methods go through Google's Firebase Authentication.**
After you finish signing in on Google's or Apple's screen, Firebase issues an identity
token to the app, and the app exchanges it with ThaiJam's server for a session.

As a result, **Google knows you have signed in to ThaiJam with that account** and keeps
an account record on the Firebase side (identifier, email, sign-in method). Your password
is always entered on the provider's own page; ThaiJam never sees it.

Firebase's data handling is governed by the
[Google Privacy Policy](https://policies.google.com/privacy).

**Firebase is used only for sign-in.** We have not installed Firebase Analytics,
Crashlytics or any other Firebase module — no usage statistics and no crash reports.

### 3. Learning content sync (only after signing in)

Once you sign in, the app syncs the content listed in the table above with the server
**when it opens, when it returns to the foreground, and after you add or change
content**. This is the main purpose of signing in.

It never happens if you don't sign in, and stops once you sign out.

### 4. AI credits and AI features (only after signing in)

Checking your credit balance and history, and redeeming a code, send requests to our
server.

**What AI features send**

| Feature | What is sent |
| --- | --- |
| Song analysis | The lyrics you pasted (with repeated choruses and section markers removed) |
| Dictionary lookup | The Thai word you entered |
| Sentence breakdown | The Thai text of that sentence |
| Extra example sentences | The pattern's formula, explanation and existing examples (all built-in lesson content, none of your data) |

**Where it goes**

First to ThaiJam's server (Cloudflare Workers), which then forwards it to the
[OpenAI](https://openai.com/policies/privacy-policy) API to generate the result.
ThaiJam authenticates the request with your account session for credits, rate limits
and abuse prevention, but what is forwarded to OpenAI **does not include your Google
sign-in identifier, email or any other information that directly identifies you** —
only the text in the table above.

**Not sent by AI text features:** your learning records, review progress, word lists,
decks, song audio or cover images. Pronunciation recordings go only to Azure Speech as
described in "7" below, never to OpenAI.

OpenAI is a third-party service; how it handles content is governed by OpenAI's own policy.

**AI result cache:** to improve speed and consistency, the system may temporarily cache
AI-generated results keyed by a hash of the content.

### 5. Account deletion

When you tap "Delete account" and confirm, a deletion request is sent to our server.

### 6. Spotify search and playback (you must set it up first; off by default)

**This connection exists only after you enter a Spotify Client ID in settings and link
your account.** Without that setup it never happens — it is not on by default.

- Linking: the app opens the system browser to Spotify's sign-in page, and **you
  authorize directly on Spotify's website**. ThaiJam never sees your Spotify password.
- Only one scope is requested: **`app-remote-control`** (controlling playback in the
  Spotify app). **We cannot read your playlists, listening history or profile** — those
  are separate scopes we do not request.
- Searching: only **the keywords you type** are sent — not your learning records,
  flashcards or ThaiJam account.
- Results contain only public track information (title, artist, album art, duration,
  Spotify link), and we store only the title, artist and track link of the song you
  **choose**.
- **Playback: audio is played by the Spotify app itself, not ThaiJam.** After you choose
  Spotify as the source on a song page and press play, ThaiJam sends play/pause/seek
  commands through Spotify's App Remote and reads **the current track and playback
  position** — used to keep the lyrics in time with the music. ThaiJam **does not
  download or play** Spotify audio itself.
- The playback position stays in memory for scrolling the lyrics; it is not written to
  the database or sent to ThaiJam's server.
- The authorization token is stored on this device, and you can "Disconnect" at any time
  in Settings → Spotify.

Spotify is a third-party service; how it handles requests is governed by Spotify's own policy.

### 7. Pronunciation assessment (only after signing in, and only while you hold the record button)

Recording starts only while you **hold** the microphone button on a card page, for up to
10 seconds, and stops when you let go. The recording exists only in memory (it is never
written to a file); it is sent to our server, which forwards it to **Microsoft Azure's
pronunciation assessment service** for scoring.

- Only **the recording** and **the Thai word or sentence you are practising** are sent
- Only scores come back (overall, accuracy, fluency, completeness, and per-word scores)
- **We do not store the recording or the text Azure recognized.** Only the four numbers
  in the table above are kept
- No press, no recording and no connection

Azure is a third-party service; how it handles audio is governed by Microsoft's own policy.

### 8. Buying AI credits (only after signing in, and only when you tap buy)

**Payment is handled entirely by Google Play. ThaiJam cannot see or receive your card
number, billing address or any payment details.**

After you tap buy and complete payment on Google Play's screen:

- The app sends our server only two things: **the product ID you bought** and **the
  purchase token issued by Google Play**. No personal data beyond your account email,
  and no payment details.
- Our server asks Google whether the purchase is genuine and the amount correct, and only
  then adds the credits to your account.
- The stored purchase record is: transaction ID, order ID, product ID, credits added, time,
  and a **hash of the purchase token** (SHA-256) — **not the token itself**. The hash
  prevents the same purchase from being redeemed for credits twice.

Refunds are handled by Google Play. After you request a refund on Google Play, we receive
the refund notice from Google and take back the corresponding credits.

### 9. Apple Music (you must link it first; off by default)

**This connection exists only after you link Apple Music on a song page.** It requires
your own Apple Music subscription.

- Linking: the app opens **Apple's MusicKit authorization screen**, and you agree directly
  in Apple's interface. ThaiJam never sees your Apple password.
- The **music user token** obtained after authorization **stays on this device only**; it
  is not sent to ThaiJam's server or synced to other devices.
- Searching: only **the keywords you type** are sent — not your learning records or
  flashcards.
- Results contain only public track information (title, artist, album art, duration), and
  we store only the song you **choose**.
- **Playback: audio is played by Apple Music; ThaiJam does not download audio files.**
  The app sends play/pause/seek/speed commands and reads the playback position to keep the
  lyrics in time. The position stays in memory, is not written to the database and is not
  sent to the server.

Apple Music is a third-party service; how it handles requests is governed by Apple's own policy.

### 10. Song recognition (only when you tap the recognize button; uses the microphone)

After you tap song recognition on a song page and allow microphone access, the app
**listens to music playing around you** to identify the song.

- The app uses Apple's **ShazamKit** to turn what it hears into an **audio fingerprint
  on this device**; it is the fingerprint, **not the raw recording**, that is sent for
  matching.
- **The recording is not stored** and is not sent to ThaiJam's server.
- Only public information about the matched song comes back (title, artist, album art).
- No tap, no recording. Listening stops when recognition finishes or you leave the screen.

Matching is performed by Apple / Shazam services under their own policies.

### 11. The in-app social invitation card (no sign-in needed)

At launch the app fetches the content for this card from our own server (Cloudflare) —
text, links and (if configured) one or more images. This lets us change campaign wording
without shipping an app update.

**This request contains no account, no email, and no learning records or flashcards.**
It carries the three headers the app sends with **every** request to our own server —
app version, platform (android) and interface language — with no advertising ID, no
SSAID and nothing that could identify your device. The server returns the same content
to every user.

The content is saved on your device; without a network connection the last copy is used,
and if none was ever fetched the version built into the app is shown — so offline the card
is just as complete and just as easy to close.

**This is not third-party advertising.** The card currently shows only ThaiJam's own
content (for example, our social media accounts). In the future it may show content from
**creators who partner with ThaiJam** — in that case the card will be labelled
"Partner" so you can tell at a glance that it is not our own.

Whoever the content is from, four things always hold: **no third-party ad SDK, no
advertising ID, no record of how often you saw or whether you tapped it, and images are
stored on ThaiJam's own server** — seeing the card never connects you to anyone else's
server.

### Everything else is offline

1,583 lesson items, 1,727 audio recordings and the Thai word-segmentation dictionary
(21,654 words) are bundled in the app. Audio playback, Thai word segmentation, tracing
scores and romanization all happen on the device.

**Of the eleven connections above, only item 11 (the social invitation card) happens
without you doing anything first** — every other one requires you to tap a button or
sign in.

## Permissions

| Permission | Purpose |
| --- | --- |
| Internet (`INTERNET`) | The connections listed above. Without signing in, only lyrics search uses it, and only when you tap the button. |
| Notifications (`POST_NOTIFICATIONS`) | Review reminders and streak reminders. **Scheduled entirely on the device, never through any server.** Each can be turned off in settings; denying the permission does not affect anything else. |
| File access | **The app declares no storage permissions.** Importing flashcard CSVs and song audio goes through Android's system file picker, where you choose the file — the app can read only the file you picked and nothing else. Song audio is **copied** into the app's private storage (access granted by the system picker can expire at any time, and without a copy that song could no longer play), and the copy is deleted when you delete the song. |
| Microphone (`RECORD_AUDIO`) | **Used by two features, both started by you.** (1) **Pronunciation assessment** — records only while you **hold** the microphone button, up to 10 seconds; the recording goes to our server and on to Azure for scoring (see "7"). (2) **Song recognition** — after you tap the recognize button it listens to music around you and sends an **audio fingerprint** computed on the device, not the raw recording (see "10"). The app does not ask for this permission at launch, and denying it affects nothing else. |

**The app does not use the camera, location, contacts or health data.**

## Children and minors

This app is not directed primarily at children; its age rating is shown by Google Play
based on the content rating questionnaire and local standards. ThaiJam does not collect
personal data for advertising (the app has no third-party ads and no third-party
analytics; the only promotional content is the in-app invitation card — currently
ThaiJam's own content only, and partner creators' content would be labelled; see item 11
under "Network connections").

The Android version has one paid item: **AI credits** (a consumable). It is always
processed through Google Play billing, and purchases by minors are subject to Google
Play's parental controls (parents can require authentication before purchases); we do not
and cannot bypass these settings. For how purchase data is handled, see "8. Buying AI
credits" above.

## Changes

If this policy changes, we will update the date at the top of this page and publish it
together with the new version of the app.

## Contact

For any questions, email: `support@thaijam.app`

---

*This policy describes **the actual current behaviour** of ThaiJam for Android. If we
change how data is handled, we will update this policy before releasing the change.
If this English translation and the [Traditional Chinese version](/privacy-policy-android/)
differ, the Traditional Chinese version prevails.*
