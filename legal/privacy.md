---
title: Privacy Policy — Chalkieboard
permalink: /legal/privacy/
---

<script>(function(){try{var q=new URLSearchParams(location.search);if(q.get("lang")==="en"){localStorage.setItem("chalkieboard.lang","en");return}if(localStorage.getItem("chalkieboard.lang")==="en")return;var l=(navigator.languages&&navigator.languages[0])||navigator.language||"";if(/^ko(\b|-|_)/i.test(l))location.replace("/ko"+location.pathname+location.hash)}catch(e){}})();</script>

# Privacy Policy — Chalkieboard

한국어: [개인정보처리방침](/ko/legal/privacy/)

**Effective date: October 6, 2026**

Chalkieboard is an iPad app that elementary school teachers use to write on the board
during lessons. Because it is used in classrooms, it was **designed so that children's
information has no reason to enter the app**. This document describes that design
exactly as it is.

---

## 1. One-line summary

**Chalkieboard does not send personal information to the developer's servers.** Your lesson
materials, board work and timetables are kept only on your device and in your own iCloud.
The developer cannot see them.

**The current release does not include TypeSafe/Jev.** It has no TypeSafe key-entry or
student-context transmission option, and it does not send voice transcripts, screen
context or student speech to TypeSafe. The app's Voice Commands use Apple's on-device
speech recognition. Separate Siri actions are handled through Apple's system Siri
(Section 5.1).

**Earlier TestFlight builds with TypeSafe enabled have different processing.** If you
still use one of those builds with your own TypeSafe key, transcripts and selected
context may be sent to TypeSafe in the United States. Section 5.2 retains that disclosure;
this policy update does not disable an earlier installed build.

---

## 2. What the app handles and where it is kept

| What | Where it is stored | Can the developer see it? |
|---|---|---|
| Board work (handwriting, text, shapes) | On the device (the app's private storage) | No |
| Lesson materials (PPTX, PDF, HTML, images) | On the device · your iCloud Drive | No |
| Timetable, subjects, units, lessons | On the device | No |
| App settings (board color, pens, fonts) | On the device | No |
| Subscription record (Chalkieboard Pro) | Apple's servers (App Store) | No (handled by Apple) |
| The app's Voice Commands audio | Turned into text on the device and not stored | No |
| Voice Commands transcribed text | On the device in the current release; earlier TestFlight TypeSafe processing is described in Section 5.2 | No |
| System Siri requests | Handled by Apple under your Siri settings and Apple's policies; the app receives the requested action | No (handled by Apple) |
| TypeSafe keys stored by an earlier build | In this device's Keychain; unused by the current release and not deleted by this update | No |
| The teacher's voice feature values | On the device (Keychain) | No |
| Classroom scene estimate (scene name, time of change) | In device memory — erased when the class ends. 7 days if 'Keep Class Timeline' is on | No |
| Earlier builds' voice decision log | On the device and in your own iCloud Drive (`Chalkieboard/판단기록`, excluded from backup) — up to 30 days or 50MB (Section 8) | No |

**There are no Chalkieboard accounts.** Chalkieboard has no sign-up. It does not ask for or collect
names, email addresses, phone numbers, school names or student information.
Your Apple account for iCloud or the App Store, and any sign-in required by a website
you open, are separate from Chalkieboard. Websites handle their own services under their
own policies.

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
  recorded or stored, and sound is not sent off the device. **Verify teacher voice** is a separate option,
  off by default. Voice enrollment is required only when this verification is enabled.
  Voice feature values (a list of numbers) are stored only in the device's Keychain.
  With verification off, commands are interpreted from speech heard by the microphone without an identity check.
  You can stop listening with the microphone button. To recognize frequently used commands quickly, the app may
  remember on the device a fingerprint of what was said (a hash value that cannot be
  reversed) and the command name.
- **System Siri** — The separate next-page, previous-page, pen and eraser actions use
  Apple's system Siri and App Intents. Siri's speech processing is governed by your Siri
  settings and Apple's policies. The app receives the action to perform. This is
  separate from the app's microphone-based Voice Commands.
- **Classroom scene estimation** — During a class with Voice Commands on, the app examines
  classroom sound **only on this iPad** to guess what kind of scene the class is in, such
  as explanation, group activity or presentations. It uses only numbers, such as how many
  voices there are, the volume, and a score for whether it is the teacher's voice. Sound
  is not sent off the device. This guess is used only to carry out voice commands more
  carefully. The scene guess (scene names and probabilities) is not sent off the device.
  The current release does not send student transcripts or classroom facts to TypeSafe.
  Earlier TestFlight builds with TypeSafe enabled are described in Section 5.2.

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

## 5. Voice Commands and Siri

### 5.1. Current release without TypeSafe/Jev

The app recognizes Voice Commands with Apple's on-device speech APIs and interprets
supported commands with rules on this iPad. The microphone and speech-recognition
permissions in Section 3 apply when you enable this feature. Language support depends
on the device, OS and Apple's available language assets; downloading an asset may need
an internet connection.

There is no TypeSafe key-entry option in this release. TypeSafe/Jev requests, web-context
transmission and student-speech-context transmission are disabled, including when an
earlier build stored a key or enabled those options. The update does not erase stored
keys or existing voice logs (Section 8).

The separate System Siri actions turn to the next or previous page, or select the pen
or eraser. Apple's system Siri processes the Siri request according to your settings
and Apple's policies. Chalkieboard receives the requested action through App Intents;
it does not record Siri audio. These actions do not use TypeSafe/Jev.

### 5.2. Earlier TestFlight builds with TypeSafe enabled

This subsection applies only to earlier TestFlight builds that include TypeSafe/Jev.
An earlier installed build can still transmit data when you enable that feature. The
disclosures below describe those builds, not the current release without TypeSafe/Jev.

By default, Voice Commands understands only set command phrases. If you enter **your own
TypeSafe API key** in Settings ▸ Voice Control (Beta), the following is sent to TypeSafe
(Jev) so that the meaning of speech that is not a set phrase can also be interpreted. The
cost of interpretation is charged to that key's credits.

- **Transcripts of voice-command candidates** — What is said after the wake word ("Hey Chalkie");
  what is said within 8 seconds after an action done by voice; and, among speech heard
  without the wake word, speech that contains the name of a material, tool or button on the
  screen, a function (turning pages, timer, underline, taking dictation, etc.), a page
  number or a time. Other transcription candidates that sounded similar are sent as well.
  **If a student's name is in the speech, it is sent as is.** With teacher verification off,
  speech from students or other people may also be sent as command candidates. Verification is not perfect
  when enabled, and interpretation requests precede the separate execution check; transmission is not
  guaranteed to contain only the teacher's speech.
- **Screen state** — Names of materials, tools and buttons; the material being viewed and
  its page number; the tool currently selected; some of the text on the page being
  viewed; the kinds of marks already drawn on that text; and the action just done by voice.
  For text lines observed on the screen, the same request may also include their source,
  normalized screen positions, and literal spans matching the speech. **If that text includes
  student names, they may be sent as well.**
- **Web page text (optional)** — Only if you turn on 'Web Page Voice Control' in Settings:
  the names and kinds of buttons and input fields on the open web page (up to 253, starting
  with those that overlap with what was said). **This may include student names.** This
  setting is off by default.
- **Facts about the classroom sound (during a class)** — Facts this iPad observed in the
  classroom sound: whose sound is heard right now (the teacher, one student, several
  students, quiet, or the app's own video); whether a student's voice was heard just before
  the speech; how loud the teacher's voice is (low, normal, loud); an activity the teacher
  announced (as read from the teacher's words) or chose by hand, and how many seconds ago;
  and the order and timing of the voice segments in the speech (teacher, student, several
  students, the app's video, unsure). These are only words and numbers set by the app; they
  contain no sound and no text. Anything unknown is not sent.
- **Recent student speech context (optional)** — Transcripts of students' speech are transmitted to TypeSafe in the United States.
  If you turn on Student Speech Context, the existing voice-command request can include up to two recent transcripts
  (at most 160 characters each, from the previous 20 seconds). A segment with evidence of another, non-teacher voice
  may also be included and is labelled `other`, since that voice is not necessarily a student. Segments with unknown
  speaker identity are excluded. This setting is off by default. No additional request is made for this context.
  Enabling it does not replace teacher-voice verification or grant permission to run commands.
- **Per-voice speech turns and the classroom picture (lessons with continuous speaker analysis, optional)** — Transcripts
  of the teacher's, students' and other people's speech are transmitted to TypeSafe in the United States. With continuous
  speaker analysis on, the existing voice-command request can include what was heard in the previous 30 seconds split by
  voice (up to six turns, at most 160 characters each and 480 in total), with the number the app gave each voice (v1…)
  and how many seconds ago it ended. TypeSafe judges who said each turn, the current class activity and who holds the
  floor; the app keeps those judgements (the activity name, who is speaking, the teacher's voice number) only in this
  iPad's memory during the lesson and sends them with the next request. No sound or voice features are sent, and they
  are discarded when the lesson screen closes. The judgements are only used to be more careful about taking speech
  without the wake word as a command; commands called with the wake word are never blocked by them. This setting is off
  by default and no additional request is made for these turns.

Not sent to TypeSafe: sound, the teacher's voice features and voice similarity score (used on this iPad), classroom scene estimates (scene names and probabilities), board work,
lesson material files, photos.
For the built-in speaker and microphone route, the app attempts echo processing on this iPad.
**When Verify teacher voice is enabled**, execution is allowed or held according to the registered-voice check.
This option is independent of continuous speaker analysis and student speech context. With verification off,
identity-check failures do not block commands; the other interpretation and execution conditions remain.

**Transfer outside Korea.** The recipient is TypeSafe AI, and its servers are in the United
States. The purpose is to interpret the meaning of what was said. The transfer takes place
over the internet each time something is said. TypeSafe states that it does not use the
text it receives for AI training and keeps it "for as long as needed for the service";
there is no fixed retention period. TypeSafe also states that it does not knowingly
receive personal information of children under 18 (https://typesafe.ai/legal/privacy-policy).
If you still use an earlier build and do not want this transfer, do not enter a key, or
remove it in that build's settings. Turning off Voice Commands in that build stops its
voice-interpretation requests. Installing the release without TypeSafe/Jev disables
this transmission without deleting an existing key or log.

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
that content stays **on that device and in that teacher's iCloud**. The current release
does not send student names, page text or student transcripts to TypeSafe/Jev. The school
and the teacher are responsible for managing such material. The developer cannot access it.

In earlier TestFlight builds with TypeSafe enabled (Section 5.2), student names that the teacher
says (for example, "praise cards for Seonghu and Hyeonmin"), speech from students or other people
recognized as command candidates, and some of the text on the page being viewed (including any student
names written there) may be sent to TypeSafe in the United States. If you turn
on 'Web Page Voice Control', student names shown on a web page may also be sent (off by
default). Please check that this fits the policies of your school and office of education
before using it. Classroom scene estimation happens only on the device. Students' audio
is not sent. Classroom facts describe who spoke and when; only if Student Speech Context
or continuous speaker analysis is separately enabled can recent transcribed words join the same request (Section 5.2).

---

## 8. Retention and deletion

- If you delete the app, the board work, materials and settings on the device are deleted
  with it.
- **Keys from earlier TypeSafe-enabled builds** — This update does not delete a key
  previously stored in the device's Keychain. The current release does not read or use
  that key for a TypeSafe connection.
- **Earlier TypeSafe-enabled builds' voice decision log** — In those earlier builds,
  new entries keep only metadata: IDs, stages and types, model name,
  timing, result codes, counts, and diagnostic numbers or fixed states such as analysis
  intervals and verification settings. They do not retain transcribed words, request or
  response bodies, audio, or voice features. If a teacher's voice is registered, though, each
  command turn's similarity score (a number comparing it with the registered voice) is also
  kept in new entries. Entries made by the previous log format
  may still exist and may contain the original speech and interpretation results; this update
  does not delete them. The log is kept on this device, with a copy in the `판단기록` (decision log)
  folder inside the `Chalkieboard` folder of your own iCloud Drive. It is not sent to the
  developer. The log is on by default in test builds (TestFlight) and off in the App Store
  version. Once entries are older than 30 days or the log exceeds 50MB, the oldest entries are
  deleted first, copies included. You can turn it off or delete it in Settings ▸ Voice Control
  (Beta); deleting it also removes that device's copies. It is not included in device backups.
  The current release does not create Jev decision-log entries or run their automatic
  retention or iCloud-copy cleanup. Existing entries and copies are preserved, and
  their management controls are absent from this release. The preceding controls and
  retention rules describe the earlier TypeSafe-enabled builds.
- **Class timeline** (when 'Keep Class Timeline' is on) — Only scene names and the times
  they changed are kept, for 7 days.
- The `Chalkieboard` folder in iCloud Drive holds your files, so it remains. If you want to
  remove it, delete it yourself in the Files app or Finder.
- The developer keeps **no** user data. So there is no need to ask the developer to access,
  correct or delete your data.

---

## 9. Sharing with third parties

Chalkieboard does not sell or rent user data. Google AdMob (Section 4), Apple services
including iCloud, the App Store and System Siri (Sections 3, 5.1 and 6), and websites you
choose to open handle their own services under their own policies.

The current release does not send data to TypeSafe/Jev. For earlier TestFlight builds
with TypeSafe enabled, the optional transfer to TypeSafe is described in Section 5.2.

---

## 10. When this policy changes

If this policy changes, the effective date on this page will be updated. Important changes
will be announced in the app.

---

## 11. Contact

- Email: chalkieboard@207studio.dev
- Developer: 207 Studio

Inquiry emails are used only to reply to you, and are deleted once the reply is complete.
