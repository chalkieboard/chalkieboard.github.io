---
title: Privacy Policy — Chalkieboard
permalink: /legal/privacy/
---

<script>(function(){try{var q=new URLSearchParams(location.search);if(q.get("lang")==="en"){localStorage.setItem("chalkieboard.lang","en");return}if(localStorage.getItem("chalkieboard.lang")==="en")return;var l=(navigator.languages&&navigator.languages[0])||navigator.language||"";if(/^ko(\b|-|_)/i.test(l))location.replace("/ko"+location.pathname+location.hash)}catch(e){}})();</script>

# Privacy Policy — Chalkieboard

한국어: [개인정보처리방침](/ko/legal/privacy/)

**Effective date: October 6, 2026**

Chalkieboard is an iPad tool for teachers and presenters. It does not provide student
accounts or ask teachers to register student identities. Lesson materials, handwriting
and spoken commands can still contain personal information. This policy explains local
processing and the optional sharing described below.

---

## 1. Summary

**Chalkieboard does not send your lesson files, board images or timetable to the developer's
servers.** They are kept on your device and, when you choose to use it, in your own iCloud.
The developer cannot access them.

**The version with a Use Jev setting keeps Jev off by default, including after an update
with a previously saved TypeSafe key.** The app's Voice Commands use Apple's on-device
speech recognition. With Jev off, supported commands are interpreted on this iPad and
no connection checks, connection prewarming or interpretation requests go to TypeSafe.
If you explicitly consent, turn on Jev and provide your own TypeSafe key, selected command
transcripts and screen context are sent to TypeSafe AI in the United States (Section 5.2).

Build `202610061343` does not include Jev. Earlier TypeSafe-enabled TestFlight builds have
different controls and may also send optional student speech context (Section 5.3).
Updating this policy does not change the behavior of an earlier installed build.

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
| Voice Commands transcribed text and selected screen context | On the device with Jev off; sent to TypeSafe with consent and Jev on (Section 5.2). Earlier builds: Section 5.3 | No |
| System Siri requests | Handled by Apple under your Siri settings and Apple's policies; the app receives the requested action | No (handled by Apple) |
| Your TypeSafe API key, including a previously stored key | In this device's Keychain; used to authenticate TypeSafe requests only with Jev on. Turning Jev off keeps the key | No |
| The teacher's voice feature values | On the device (Keychain) | No |
| Classroom scene estimate (scene name, time of change) | In device memory — erased when the class ends. 7 days if 'Keep Class Timeline' is on | No |
| Earlier builds' voice decision log | Existing device and personal iCloud Drive files are preserved; the current version does not resume writing or automatic cleanup (Section 8) | No |

**There are no Chalkieboard accounts.** Chalkieboard has no sign-up and does not ask you
to register names, email addresses, phone numbers, school names or student identities.
Personal information in your content or spoken commands may be processed as described
in Sections 5 and 7.
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
- **System actions and Siri** — App Intents expose voice on/off, open lesson, next/previous
  page and pen/eraser actions to Siri and Shortcuts. When invoked through Siri, speech
  processing follows your Siri settings and Apple's policies. The app receives the action
  to perform. These system entry points are separate from the app's microphone-based
  Voice Commands and do not use Jev (Section 5.1).
- **Classroom scene estimation** — During a class with Voice Commands on, the app examines
  classroom sound **only on this iPad** to guess what kind of scene the class is in, such
  as explanation, group activity or presentations. It uses only numbers, such as how many
  voices there are, the volume, and a score for whether it is the teacher's voice. Sound
  is not sent off the device. This guess is used only to carry out voice commands more
  carefully. The scene guess (scene names and probabilities) is not sent off the device.
  With Jev on, separate classroom facts such as sound-source labels, loudness and segment
  timing may be sent with a command request (Section 5.2). These facts contain no audio
  or transcript text. Extra recent student context and per-voice transcripts are absent
  from the current version; their use in earlier builds is described in Section 5.3.

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

## 5. Voice Commands, optional Jev and system actions

### 5.1. Apple speech and commands on this iPad

The app transcribes microphone audio with Apple's on-device speech APIs and uses rules on
this iPad for supported commands. This does not require saying “Hey Siri” or turning on
Siri. If Only Listen After Wake Word is off, the app's own wake word is not required either.
Voice Commands requires Pro and the microphone/speech permissions in Section 3. Language
support depends on the device, OS and Apple's language assets; downloading an asset may
need internet. If on-device recognition is unavailable, the app does not silently switch
to server speech recognition.

With Jev off, supported page/tool commands, supported Korean polite expressions, uniquely
matched material names, explicit English/Korean dictation or reveal commands and uniquely
matched visible app-button names are handled on this iPad. This is a defined set of commands;
it does not promise to understand every sentence. Highlighting selected text and more
flexible requests can use Jev when you choose to enable it.

The separate App Intents actions turn Voice Commands on/off, open a lesson, turn to the
next/previous page or select pen/eraser. They can be invoked through Shortcuts or system
controls. You can also configure Apple's Vocal Shortcuts in iPad accessibility settings
for a spoken phrase without “Hey Siri”; this is a separate system feature you set up.
When you use Siri, Apple processes that request according to your Siri settings and policies.
Chalkieboard receives the requested action, does not record Siri audio and does not use
TypeSafe for those actions.

### 5.2. Optional Jev in the version with a Use Jev setting

Jev is off by default, even with an API key stored by an earlier version. Saving a key does
not enable Jev or check the connection. Before enabling Jev for the first time, the app
asks for explicit permission to share the listed command text and context with TypeSafe AI
in the United States. If this disclosure changes, permission is required for the new version.
You need your own TypeSafe API key, an internet connection and available TypeSafe credits.
Interpretation costs are charged to that key's credits, separately from Chalkieboard Pro.

With Jev on, command candidates admitted by the app may be sent for interpretation:

- **Command transcripts and alternative transcriptions** — Speech after the app's wake
  word, short follow-ups within 8 seconds of a voice action, or speech without the wake word
  that matches a material, tool, button, function, page number or time. **Personal names in
  that speech can be sent as written.** Microphone commands may come from students or other
  people when teacher verification is off. Verification does not perfectly identify a
  speaker, and interpretation and execution checks are separate; transmission is not
  guaranteed to contain only the teacher's words.
- **Selected screen context** — Material, tool and button names; the current material/page
  and tool; matching page text and marks on it; source, normalized screen position and
  matching spans of observed text; recent voice actions and state of visible app controls.
  **Personal information in these names or text can be included.** The app sends selected
  text/context, not the full document file, photo or a recording of the board screen.
- **Classroom sound facts** — App-produced labels/numbers for the sound source (teacher,
  student, several voices, silence or app media), whether a student voice preceded the
  command, loudness, an announced or manually chosen activity and elapsed time, and the
  order/timing of voice segments. App-produced activity/floor labels from earlier judgments
  and their elapsed times may also be included. These facts contain no audio or transcript text.
- **Web context, only with a separate choice** — Web Page Voice Control is off by default,
  including after updating from an older enabled setting. If you turn it on as well as Jev,
  the current web page title, button/input names and kinds (up to 253, ranked by overlap with
  the speech), permitted action types and matching visible page text can be sent. They may
  contain student names or other personal information. Opening a website by itself does
  not enable this Jev option; websites otherwise operate under their own policies.

Raw microphone audio, voice feature values and voice similarity scores are not sent to
TypeSafe. The current version does not add recent student-speech context or per-voice
transcript turns to requests. Activity/floor labels are separate text-free classroom facts. It does not resume
Jev decision logging when Jev is enabled. This does not exclude a student's words or name
from a command candidate or visible text described above.

While Jev is on, the app may prepare a connection to TypeSafe. Check Connection sends a
fixed test command. TypeSafe receives the API key for authentication and the network
information needed to handle those requests. Turning Use Jev off stops new interpretation,
prewarming and connection-check requests, cancels pending requests and ignores their late
results. It keeps your key, materials and existing logs. It cannot retract data a service
has already received. To stop microphone commands too, turn Voice Commands off.

TypeSafe is the recipient of the optional text/context transfer and hosts its services in
the United States. Its [privacy policy](https://typesafe.ai/legal/privacy-policy) states that
it collects submitted prompts, data and other Input, may collect technical/usage information,
and does not train or fine-tune models on Input. It retains personal data for as long as
reasonably necessary for its services or business/commercial purposes; no fixed number of
days is specified. TypeSafe also states that its service is not directed to children and
that it does not knowingly collect, maintain or use personal data from children under 18.

[TypeSafe's legal documentation](https://docs.typesafe.ai/legal) offers zero data retention
to enterprise customers. Chalkieboard does not assume that an ordinary personal API key
has that arrangement or promise immediate deletion. Disabling Jev is not a server-side
deletion request; contact TypeSafe about information it has already received.

### 5.3. Previously installed TestFlight builds

Build `202610061343` excludes TypeSafe/Jev: there is no key-entry or transmission option,
and a previously saved key is unused for TypeSafe connections. It preserves existing keys
and logs. It is distinct from the version with the Use Jev toggle described in Section 5.2.

Earlier TypeSafe-enabled TestFlight builds can still send the command-candidate, screen,
web and classroom context described above while Voice Commands is on and a key is available.
They do not have the new independent Use Jev consent control. Updating this policy does
not disable an installed older build. To prevent its interpretation requests, avoid entering
a key, remove any saved key in that build's settings, or turn off Voice Commands.

Those older builds can also have these separately enabled transcript-context features:

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


These older features do not replace teacher verification or grant permission to execute
commands. Raw audio and voice features remain on the device. Their optional transcript
sharing and old logging behavior are not resumed by installing the current version.

---

## 6. Payment

Chalkieboard Pro subscriptions are made only through **App Store in-app purchase**. Apple
handles payment information such as card numbers. Neither the app nor the developer
receives that information. You can manage or cancel your subscription in iOS Settings ▸
Apple Account ▸ Subscriptions. Optional Jev interpretation is charged by TypeSafe to
your own API key; Chalkieboard does not sell TypeSafe credits or take that payment (Section 5.2).

---

## 7. Children's personal information

Chalkieboard is a tool for teachers, not a student account service. A teacher may include
student names, photos or other personal information in lesson materials or board work.
Those files stay on the device and, if chosen, in the teacher's iCloud. The developer
cannot access them.

With Jev off, the app sends no command transcripts or screen context to TypeSafe. With
Jev on, a student's name or words in a command candidate, material/button name or matching
page text may be sent to TypeSafe in the United States (Section 5.2), even though extra
recent student context is unavailable. Web context requires its separate choice. Raw
student audio is not sent. Earlier builds may also transmit the optional recent student
and per-voice transcripts described in Section 5.3.

Use Jev only for information you are authorized to share, following your school and office
of education's rules and applicable requirements for children's data. A teacher's consent
to Jev does not by itself establish permission to share another person's information.

---

## 8. Retention and deletion

- If you delete the app, the board work, materials and settings on the device are deleted
  with it.
- **TypeSafe keys** — This update preserves a previously stored key in this device's
  Keychain. Saving a key or turning Jev off does not enable interpretation or erase the
  key. You can remove the key in Settings ▸ Voice Control (Beta); removing it also turns
  Jev off and cancels pending requests. An existing key alone is not permission to send data.
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

TypeSafe/Jev is an optional recipient only when you consent and enable Jev, as described
in Section 5.2. Previously installed TestFlight builds have the behavior in Section 5.3.

---

## 10. When this policy changes

If this policy changes, the effective date on this page will be updated. Important changes
will be announced in the app.

---

## 11. Contact

- Email: chalkieboard@207studio.dev
- Developer: 207 Studio

Inquiry emails are used only to reply to you, and are deleted once the reply is complete.
