# Psychiatry practice prototype

A clickable prototype of a psychiatry practice system: Schedule, Day, Patients, Inbox and Tasks, with Home behind the clinic name, and the patient's intake as a phone chat.

Open it at https://jluo-stalwart.github.io/psych-practice-prototype/

Everything in it is made up: the clinic, the patients and the visits. Nothing is sent anywhere except what you ask the AI to write, which goes to Anthropic. Each visitor's changes stay in their own browser, and "Reset demo" in the top bar puts everything back.

The AI buttons run on your own Claude account. Choose "Connect Claude" in the top bar, or any AI button, then sign in to the Claude Console, create an API key and paste it. The key stays in your browser and is sent only to Anthropic, which bills your Console account for what the AI writes: roughly 10 to 25 cents a note, separate from any Claude Pro or Max plan. Without a key, the AI buttons offer the prompt to copy into a chat at claude.ai, and the demo patients' example notes and summaries still work.

In Chrome, Edge or Safari, the record button records from your microphone and turns speech into text with the browser's speech recognition. The browser's maker hears the audio (Google for Chrome, Microsoft for Edge, Apple for Safari), so use made-up voices only. The made-up sessions are in the menu beside the record button, and other browsers play them instead.

A testing version for invited testers is at https://jluo-stalwart.github.io/psych-practice-prototype/trial/. It opens on a sign-in, and each test account gets its own clinic that starts empty and keeps the tester's work in their browser.

`index.html` is the whole prototype, and `trial/index.html` is the testing version. Both are built from separate source files kept elsewhere, so change those rather than these files.
