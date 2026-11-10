# LearnWise

## What this repo is about

A prototype for Custom Learning Experiences. Every attempt today is typed, one message at a time. That suits a skill graded on writing. A nursing history, a counselling intake, or a negotiation needs the student to talk to a person, and the grade mostly tracks typing and patience with long replies. Students write about 22 words, the AI replies with about 148, and 34% leave between turns 3 and 6.

The case is a history with Mrs Jansen. She is anxious and hard of hearing.

## How I solved the problem

Speaking is on when the skill is a conversation. Typing stays a full way to finish.

An admin allows speaking only after they record who turns speech into text, where, how long the transcript is kept, that the recording is deleted, and a minute cap. Past the cap, the same attempt continues in typing.

The instructor answers one question: precise writing, or a spoken conversation. A history suggests speaking, with the reason in one sentence. They can leave typing as the default.

The student speaks every turn, types every turn, or switches midway. Switching keeps the same attempt. Replies stay short, the brief stays on screen, and a misheard line can be corrected before it counts. The grade is the transcript. Spoken turns include pauses, such as "12s silence." A typed attempt marks timing as not evidenced.

`direction-b.html` is that flow for an admin, an instructor, a student, and grading.

## How to run the prototype

```bash
npm install
npx serve .
```

Open `http://localhost:3000/direction-b.html`. React loads from the network. The stylesheets are in `node_modules`.
