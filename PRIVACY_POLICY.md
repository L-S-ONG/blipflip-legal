---
layout: default
title: Blipflip Privacy Policy
permalink: /privacy/
---

# Blipflip — Privacy Policy

**Last updated 3 November 2026.**

Blipflip ("the app", "we", "us") is a short‑video journaling app where you record
brief hourly clips and optionally share them with a private "squad" of friends or
with one partner in a "couple". This policy explains what we collect, why, and the
choices you have.

If you have any questions, contact us at **labratrayray@gmail.com**.

## Who is responsible for your data

The app is operated by the Blipflip developer (Raynor Ong). Our hosting and
backend services include **Supabase** for accounts and database records,
**Cloudflare R2** for media storage, and **Google Cloud Run** for media processing.
Supabase Storage is also used for media, including fallback clip storage and
avatars. Push notifications are delivered through **Expo's** push service.

## What we collect

We collect data to provide app features, understand feature usage, and diagnose
technical problems. We do **not** use your data for advertising or marketing,
sell it to data brokers, or combine it with data from other companies for targeted
advertising. Our first-party usage analytics are stored in our Supabase database
and **linked to your account ID; they are not anonymous**. You can turn these
usage events off using **Help improve Blipflip** in your profile settings.

| Data | Why we collect it | Required? |
|---|---|---|
| **Email address** | To create and sign in to your account (or via Google/Apple sign‑in) | Required for an online account; Apple may provide a private relay address |
| **Display name / username** | Shown on your clips and in squad/couple feeds and chat | Optional (defaults from your email) |
| **Profile picture (avatar)** | Shown on your profile and next to your clips/name in squad/couple feeds | Optional — chosen from your photo library; the app works without one |
| **Photos, videos, recorded audio, captions and stickers** | Recording, cloud sync, sharing, sticker creation and recap/export features; cloud features transmit the relevant media or media URLs to our services | Depends on the features you use; locally stored media is distinct from uploaded media |
| **Precise or approximate location and place labels** | Attached to clips and newly created stickers to provide location features, including couple distance and sticker location views | Optional — deny location permission to create clips and stickers without a location tag |
| **Chat messages & reactions** | To deliver squad/couple chat and reactions | Yes, if you use chat |
| **Account IDs and social connections** | To identify accounts, manage squad/couple membership, deliver shared content and support blocking/reporting | Required for the relevant online features |
| **Push notification token and device/installation identifiers** | To deliver notifications and associate technical diagnostics with an installation or device | Push notifications are optional; diagnostics are collected when reporting is enabled in the app build |
| **Usage and purchase events** | Events such as app opens, clip publication, recap opens, paywall views and Plus purchases, together with account ID, event properties, platform, app version and time | Usage analytics are enabled by default for signed-in users and can be turned off with Help improve Blipflip |
| **Crash, performance and other diagnostic data** | To troubleshoot problems: errors, technical logs, interaction breadcrumbs, device/OS details, app version and performance traces | Collected by the configured diagnostics service; the usage-analytics switch does not disable crash reporting |
| **Support requests and content reports** | To respond to your requests and investigate reported content | Only if you submit a request or report |

We do **not** read your phone's address book or collect browsing history or background location.
We do store your in-app squad/couple connections (your social graph), which Apple
includes in its "Contacts" privacy category. Location is requested in the
foreground when recording a clip or creating a sticker, with your permission.
The app does not request background location access.

## How your data is shared

- **With people you choose.** Clips you share to a squad or couple, your display
  name, your profile picture, your chat messages, and (in couple mode) the distance
  derived from your clip's location are visible to the other members of that
  squad/couple. Squads and couples are private and joined by invite code.
- **With our service providers.** Supabase (database, storage and authentication),
  Cloudflare (R2 media storage and delivery), Google Cloud Run (recap rendering,
  sticker cutouts and video processing), Expo (notifications and app updates),
  and Sentry (crash, performance and other diagnostics) process data for these
  features. Cloud media-processing requests can include your photos, clips,
  media URLs and editing instructions.
- **With sign-in and purchase providers.** Apple or Google handle their respective
  sign-in and store-payment flows. Blipflip uses the resulting account or purchase
  information to support these features; we do not receive your payment-card details.
- We do **not** sell your data, and we do **not** share it with advertisers or
  data brokers.

We use **Sentry** to collect crash reports, performance traces and error diagnostics
so we can fix bugs. Default personally identifying information collection is
disabled in our Sentry configuration, but reports can still contain installation
or device identifiers, interaction breadcrumbs, URLs and error context. This
setting does not make all diagnostics anonymous. We do not intentionally attach
your recorded media or chat-message bodies to diagnostic reports.

## Where your data is stored and how it's protected

Cloud sync uses private **Cloudflare R2** storage. Blipflip checks your account
and sharing permissions before issuing viewing links. **R2 viewing links expire
after 15 minutes.** Anyone holding a viewing link can use it until it expires.
Removing someone from a group prevents them from obtaining new viewing links.
Previously issued links remain usable until expiry, and copies already saved on
another device may remain. Supabase fallback clips and recaps also use signed
viewing links, with their own expiry periods.

Access through the former permanent public media URLs was disabled on
**3 November 2026**. Older app versions that use those URLs need an update for
cloud playback and uploads.

Cloud-service requests use HTTPS. Uploaded media is readable by the services
that store and process it to provide the app's features.

Your **profile picture (avatar)** is kept in a **public** bucket so it loads quickly
in feeds. This means anyone with the (unguessable) image URL can view it — please
don't use a photo you consider sensitive. You can change or remove it any time from
your profile.

## How long we keep it

Account and content records are retained to provide the app's features until
removed through the applicable deletion process. Removing an item from the app
does not necessarily erase every uploaded file or a copy another person has saved.
Diagnostic records, service logs and backups may have separate retention periods.
Contact us for help with removal of uploaded media and information about retention.

## Deleting your data

Deleting an individual clip from the feed removes its local entry and file from
that phone. It does not currently delete an uploaded or shared cloud copy. Use
account deletion or contact support if you need uploaded media removed.

To delete your account or request removal of associated data:

- **In an updated app:** open your **profile → Delete account**. The server records
  the request and blocks new writes covered by the deletion controls. The app asks
  you to **retry after ten minutes**, allowing existing upload links to expire.
  Deletion does not currently finish automatically in the background. On retry,
  the server removes account-owned media from Cloudflare R2 and the configured
  Supabase media buckets before deleting the account. If storage cleanup fails,
  the account is not deleted and you can retry or contact support. After successful
  cloud deletion, the app attempts to clear its local clips, stickers and caches;
  exports saved to Photos or other locations need to be removed separately.
- **Older app versions:** update Blipflip before requesting account deletion. The
  older account-only deletion route is disabled because it could leave media behind.
- A minimal deletion-request record is retained to prevent further writes and
  support cleanup reconciliation. Service logs, diagnostics, backups and copies
  saved by other people may have separate retention and deletion processes.
- **By request:** email **labratrayray@gmail.com** from your account's email address
  for account or media-deletion help. Do not send your password. Copies already
  downloaded or shared outside Blipflip cannot be removed from other people's devices
  by deleting your account.

## Permissions the app requests

- **Camera & microphone** — to record your clips.
- **Photos** — to select images for avatars or stickers and save exported media,
  where you choose those features. Optional.
- **Location (while using the app)** — to tag recorded clips and newly created
  stickers for location features. Optional.
- **Notifications** — to send reminders and squad/couple alerts. Optional.

## Children

Blipflip is **not directed to children under 13** (or the minimum age of digital
consent in your country). We do not knowingly collect data from children. If you
believe a child has provided us data, contact us and we will remove it.

## Changes to this policy

If we change this policy we will update the "Last updated" date above and, for
material changes, notify you in the app.

## Contact

Questions or requests: **labratrayray@gmail.com**
