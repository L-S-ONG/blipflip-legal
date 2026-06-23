---
layout: default
title: Blipflip Privacy Policy
---

# Blipflip — Privacy Policy

**Last updated: 23 June 2026**

Blipflip ("the app", "we", "us") is a short‑video journaling app where you record
brief hourly clips and optionally share them with a private "squad" of friends or
with one partner in a "couple". This policy explains what we collect, why, and the
choices you have.

If you have any questions, contact us at **raynordev@gmail.com**.

> Host this page at a public URL (e.g. GitHub Pages or a Notion/Google Site) and
> paste that URL into the Google Play Console → *Store listing* and
> *App content → Privacy policy*.

## Who is responsible for your data

The app is operated by the Blipflip developer (Raynor Ong). Our hosting and
backend provider is **Supabase**, which stores your account, clips and messages on
our behalf. Push notifications are delivered through **Expo's** push service.

## What we collect

We only collect what the app needs to work. We do **not** use advertising or
third‑party analytics SDKs. We do keep **first‑party, anonymous usage analytics**
(stored in our own database, never shared) to understand which features help — you
can turn this off any time in **Settings → Help improve Blipflip**.

| Data | Why we collect it | Required? |
|---|---|---|
| **Email address** | To create and sign in to your account (or via Google/Apple sign‑in) | Required to use an online account (you can also use offline demo mode with no account) |
| **Display name / username** | Shown on your clips and in squad/couple feeds and chat | Optional (defaults from your email) |
| **Profile picture (avatar)** | Shown on your profile and next to your clips/name in squad/couple feeds | Optional — chosen from your photo library; the app works without one |
| **Videos & captions (your clips)** | The core feature — stored so you and people you share with can watch them | Yes, if you record |
| **Precise location** | Attached to a clip only when you record, to show the distance between you and your partner in *couple* mode | Optional — deny the permission and clips still save, just without location |
| **Chat messages & reactions** | To deliver squad/couple chat and reactions | Yes, if you use chat |
| **Push notification token** | To send you chat, hourly and new‑clip notifications | Optional — only if you enable notifications |
| **Usage analytics** | Anonymous in‑app events (e.g. "opened the app", "made a recap") to see which features are used — never your clip content or captions | Optional — turn off in Settings → Help improve Blipflip |

We do **not** collect contacts, browsing history, or background location. Location
is read **only at the moment you record a clip** (foreground), never in the
background.

## How your data is shared

- **With people you choose.** Clips you share to a squad or couple, your display
  name, your profile picture, your chat messages, and (in couple mode) the distance
  derived from your clip's location are visible to the other members of that
  squad/couple. Squads and couples are private and joined by invite code.
- **With our processors.** Supabase (database, file storage, authentication),
  Expo (push notification delivery), and Sentry (crash and error diagnostics)
  process this data so the app can function and stay reliable.
- We do **not** sell your data, and we do **not** share it with advertisers or
  data brokers.

We use **Sentry** to collect crash reports and error diagnostics (e.g. device
model, OS version, app version and the technical details of a crash) so we can fix
bugs. This does not include the content of your clips or messages.

## Where your data is stored and how it's protected

Clips are kept in a **private** storage bucket (served only via short‑lived signed
URLs). Database access is restricted with row‑level security so users can only read
their own data and data explicitly shared with their squad/couple. All traffic is
encrypted in transit (HTTPS).

Your **profile picture (avatar)** is kept in a **public** bucket so it loads quickly
in feeds. This means anyone with the (unguessable) image URL can view it — please
don't use a photo you consider sensitive. You can change or remove it any time from
your profile.

## How long we keep it

We keep your data until you delete it. Deleting a clip removes it; deleting your
account removes everything (see below).

## Deleting your data

You can delete individual clips at any time from the feed.

To delete your **entire account and all associated data** (clips, squads, couples,
chats, reactions and profile):

- **In the app:** open **Me → Delete account**. This permanently erases your data
  on our servers and on the device. This cannot be undone.
- **By request:** email **raynordev@gmail.com** from your account's email address
  and we will delete your account within 30 days.

## Permissions the app requests

- **Camera & microphone** — to record your clips.
- **Photos** — to choose a profile picture from your library. Optional.
- **Location (while using the app)** — to tag a clip with where it was recorded for
  the couple‑distance feature. Optional.
- **Notifications** — to send reminders and squad/couple alerts. Optional.

## Children

Blipflip is **not directed to children under 13** (or the minimum age of digital
consent in your country). We do not knowingly collect data from children. If you
believe a child has provided us data, contact us and we will remove it.

## Changes to this policy

If we change this policy we will update the "Last updated" date above and, for
material changes, notify you in the app.

## Contact

Questions or requests: **raynordev@gmail.com**
