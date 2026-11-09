# Psychiatry practice prototype

A clickable prototype of a psychiatry practice system: Schedule, Day, Patients, Inbox and Tasks, with Home behind the clinic name, and the patient's intake as a phone chat.

Open it at https://jluo-stalwart.github.io/psych-practice-prototype/

Everything in it is made up: the clinic, the patients and the visits, so enter made-up details only. Each visitor's changes stay in their own browser, and "Reset demo" in the name menu at the top right puts everything back. What you enter leaves your browser only when you use the AI, record a visit or send an intake link, as described below. Loading the page also fetches its font from Google Fonts.

The AI buttons are free to use. They send what the AI needs, such as the transcript, the note or the intake answers, to this prototype's small server on Cloudflare, and Cloudflare's AI (the open model gpt-oss-120b) writes the result. The server keeps a daily count of how much AI was used, not what was sent. The free allowance is limited each day; once it's used up, the page says when it starts again (midnight UTC).

The record button records from your microphone, and Deepgram, a speech-to-text service, turns the speech into text and tells the voices apart. The audio goes straight from your browser to Deepgram, with a short-lived key from the server, so use made-up voices only. In the rare browser that can't send audio that way, its own speech recognition is used instead, and the browser's maker hears the audio. The made-up sessions are in the menu beside the record button, and browsers that can't record play them instead.

Sending an intake link, from a patient's Intake tab or when booking a consult, makes a real link to the patient's page, https://jluo-stalwart.github.io/psych-practice-prototype/intake/, for the clinic to copy into a text or email; the prototype doesn't send them itself. The patient's answers are sealed with a key that's only in the link, so the server can't read them. They wait on the server until the clinic's page picks them up, and are deleted then or after 7 days. The demo clinic starts afresh each day, so answer a link from the demo on the day it was sent.

A testing version for invited testers is at https://jluo-stalwart.github.io/psych-practice-prototype/trial/. It opens on a sign-in, and each test account gets its own clinic that starts empty and keeps the tester's work in their browser.

`index.html` is the prototype, `trial/index.html` is the testing version and `intake/index.html` is the patient's page that an intake link opens. `assets/` holds the code and styles the three share. They're built from separate source files kept elsewhere, so change those rather than these files.
