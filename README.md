# Psychiatry practice prototype

A clickable prototype of a psychiatry practice system: Home, Schedule, Patients, Visits, Inbox and Tasks, and the patient's intake as a phone chat.

Open it at https://jluo-stalwart.github.io/psych-practice-prototype/

Everything in it is made up: the clinic, the patients and the visits. Nothing is sent anywhere except what you ask the AI to write, which goes to Anthropic. Each visitor's changes stay in their own browser, and "Reset demo" in the top bar puts everything back.

The AI buttons run on your own Claude account. Choose "Connect Claude" in the top bar, or any AI button, then sign in to the Claude Console, create an API key and paste it. The key stays in your browser and is sent only to Anthropic, which bills your Console account for what the AI writes: roughly 10 to 25 cents a note, separate from any Claude Pro or Max plan. Without a key, the AI buttons offer the prompt to copy into a chat at claude.ai, and the demo patients' example notes and summaries still work. The record button plays a made-up session.

`index.html` is the whole prototype. It is built from separate source files kept elsewhere, so change those rather than this file.
