---
title: Privacy Policy — Chalkieboard
permalink: /legal/privacy/
---

# Privacy Policy — Chalkieboard

한국어: [개인정보처리방침](/ko/legal/privacy/)

**Effective date: September 24, 2026**

Chalkieboard is an iPad app that elementary school teachers use to write on the board
during lessons. Because it is used in classrooms, it was **designed so that children's
information has no reason to enter the app**. This document describes that design
exactly as it is.

---

## 1. One-line summary

**Chalkieboard does not send personal information to the developer's servers.** Your lesson
materials, board work and timetables are kept only on your device and in your own iCloud.
The developer cannot see them.

There is one exception. **If you enter your own TypeSafe API key for Voice Commands (Pro)**,
the teacher's transcribed speech (which may include student names) and some text on the
screen are sent to TypeSafe in the United States so that the meaning of what was said can
be interpreted (Section 5). The audio itself never leaves the device in any case.

---

## 2. What the app handles and where it is kept

| What | Where it is stored | Can the developer see it? |
|---|---|---|
| Board work (handwriting, text, shapes) | On the device (the app's private storage) | No |
| Lesson materials (PPTX, PDF, HTML, images) | On the device · your iCloud Drive | No |
| Timetable, subjects, units, lessons | On the device | No |
| App settings (board color, pens, fonts) | On the device | No |
| Subscription record (Chalkieboard Pro) | Apple's servers (App Store) | No (handled by Apple) |
| Voice Commands audio | Turned into text on the device and not stored | No |
| Voice Commands transcribed text | On the device — sent to TypeSafe only if you entered a TypeSafe key (Section 5) | No |
| The teacher's voice feature values | On the device (Keychain) | No |
| Classroom scene estimate (scene name, time of change) | In device memory — erased when the class ends. 7 days if 'Keep Class Timeline' is on | No |
| Voice decision log | On the device (excluded from sync and backup) — up to 30 days or 50MB (Section 8) | No |

**There are no accounts.** Chalkieboard has no sign-up. It does not ask for or collect
names, email addresses, phone numbers, school names or student information.

---

## 3. Device permissions

- **Photos** — Used only when you attach a photo you chose yourself to the board surface.
  The app does not browse your whole photo library and does not send photos externally.
- **iCloud Drive** — The route for opening on the iPad the lesson materials you prepared
  on a Mac or Windows PC. The files are in **your own iCloud account** and do not pass
  through the developer's servers.
- **External display (AirPlay, HDMI)** — When a display is connected, the app sends the
  board screen to it. This output sends only the screen image and does not store any data.
- **Microphone and speech recognition** — Used only if you turn on Voice Commands (Pro) in
  Settings. Sound is turned into text **on this iPad** (on-device dictation). It is not
  recorded or stored, and sound is not sent off the device. To turn on Voice Commands, the
  teacher's voice must be registered. Its feature values (a list of numbers) are stored
  only in the device's Keychain. To recognize frequently used commands quickly, the app may
  remember on the device a fingerprint of what was said (a hash value that cannot be
  reversed) and the command name.
- **Classroom scene estimation** — During a class with Voice Commands on, the app examines
  classroom sound **only on this iPad** to guess what kind of scene the class is in, such
  as explanation, group activity or presentations. It uses only numbers, such as how many
  voices there are, the volume, and a score for whether it is the teacher's voice. Sound
  and students' speech are not recorded or stored, and are not sent off the device. This
  guess is used only to carry out voice commands more carefully.

---

## 4. Ads

While you use the app for free, the only ads are **rewarded ads that you choose to watch
yourself to top up class time**. Watching one ad adds 1 hour of class time. There are no
banner or full-screen ads that the app shows on its own, and no ads appear during class or
on the external display. Ads are provided by Google AdMob.

- Chalkieboard requests **non-personalized ads only**. It does not use the advertising
  identifier (IDFA) and does not ask for iOS App Tracking Transparency (ATT) permission.
- Even so, AdMob processes basic technical information, such as IP address and device
  type, to show ads and prevent fraudulent clicks. Details of this processing: https://policies.google.com/technologies/partner-sites
- Users in Europe may first see a consent form (Google UMP) before an ad is shown.
- **If you subscribe to Chalkieboard Pro, class time becomes unlimited, so you do not need to watch ads.**

Chalkieboard does not separately pass user data to AdMob for advertising purposes.

---

## 5. Interpreting what voice commands mean (TypeSafe)

By default, Voice Commands understands only set command phrases. If you enter **your own
TypeSafe API key** in Settings ▸ Voice Control (Beta), the following is sent to TypeSafe
(Jev) so that the meaning of speech that is not a set phrase can also be interpreted. The
cost of interpretation is charged to that key's credits.

- **The teacher's transcribed speech** — What is said after the wake word ("Hey Chalkie");
  what is said within 8 seconds after an action done by voice; and, among speech heard
  without the wake word, speech that contains the name of a material, tool or button on the
  screen, a function (turning pages, timer, underline, taking dictation, etc.), a page
  number or a time. Other transcription candidates that sounded similar are sent as well.
  **If a student's name is in the speech, it is sent as is.** The app tries to send only
  speech judged to be the teacher's voice, but this judgment is not perfect, so students'
  speech may be mixed in and sent.
- **Screen state** — Names of materials, tools and buttons; the material being viewed and
  its page number; the tool currently selected; a few lines of text printed on the page
  that overlap with what was said; the kinds of marks already drawn on those lines; and the
  action just done by voice.
- **Web page text (optional)** — Only if you turn on 'Web Page Voice Control' in Settings:
  button and name text on the open web page that overlaps with what was said. **This may
  include student names.** This setting is off by default.

Not sent: sound, classroom scene estimates, board work, lesson material files, photos.

**Transfer outside Korea.** The recipient is TypeSafe AI, and its servers are in the United
States. The purpose is to interpret the meaning of what was said. The transfer takes place
over the internet each time something is said. TypeSafe states that it does not use the
text it receives for AI training and keeps it "for as long as needed for the service";
there is no fixed retention period. TypeSafe also states that it does not knowingly
receive personal information of children under 18 (https://typesafe.ai/legal/privacy-policy).
If you do not want this, do not enter a key, or delete it. If you turn off Voice Commands,
nothing more is sent.

---

## 6. Payment

Chalkieboard Pro subscriptions are made only through **App Store in-app purchase**. Apple
handles payment information such as card numbers. Neither the app nor the developer
receives that information. You can manage or cancel your subscription in iOS Settings ▸
Apple Account ▸ Subscriptions.

---

## 7. Children's personal information

Chalkieboard is **a tool used by teachers**. It is not directed at children and does not
collect children's personal information. On the board screen, the status bar and account
indicators are hidden so that personal information is not exposed during class.

If a teacher writes a student's name or attaches a student's photo on the board surface,
that content stays **only on that device and in that teacher's iCloud**. The school and the
teacher are responsible for managing such material. The developer cannot access it.

If you use Voice Commands (Section 5) with a TypeSafe key, student names that the teacher
says (for example, "praise cards for Seonghu and Hyeonmin") and students' speech that
gets past the teacher-voice check may be sent to TypeSafe in the United States. If you turn
on 'Web Page Voice Control', student names shown on a web page may also be sent (off by
default). Please check that this fits the policies of your school and office of education
before using it. Classroom scene estimation happens only on the device, and students'
sound and speech are not stored or sent.

---

## 8. Retention and deletion

- If you delete the app, the board work, materials and settings on the device are deleted
  with it.
- **Voice decision log** — To improve Voice Commands, the speech sent to TypeSafe and the
  interpretation results are kept only on this device. The log is on by default in test
  builds (TestFlight) and off in the App Store version. Once entries are older than 30 days
  or the log exceeds 50MB, the oldest entries are deleted first. You can turn it off or
  delete it in Settings ▸ Voice Control (Beta). It is not synced or backed up, and it
  leaves the device only when you export it yourself.
- **Class timeline** (when 'Keep Class Timeline' is on) — Only scene names and the times
  they changed are kept, for 7 days.
- The `Chalkieboard` folder in iCloud Drive holds your files, so it remains. If you want to
  remove it, delete it yourself in the Files app or Finder.
- The developer keeps **no** user data. So there is no need to ask the developer to access,
  correct or delete your data.

---

## 9. Sharing with third parties

**No data is provided to third parties.** Chalkieboard does not sell, rent or share user data.
Google AdMob and Apple (Sections 4 and 6 above), and TypeSafe (Section 5, if you entered a key), each handle their own part under their own policies.

---

## 10. When this policy changes

If this policy changes, the effective date on this page will be updated. Important changes
will be announced in the app.

---

## 11. Contact

- Email: chalkieboard@207studio.dev
- Developer: 207 Studio

Inquiry emails are used only to reply to you, and are deleted once the reply is complete.
