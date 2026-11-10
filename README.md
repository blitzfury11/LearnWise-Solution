# LearnWise

A direction and a clickable prototype for Custom Learning Experiences. Spoken skills, such as a nursing history, are practised as a conversation. Typing stays a full way to finish.

## The problem

Every Custom Learning Experience is typed, one message at a time. That suits a skill graded on precise writing, such as law. A nursing history, a counselling intake, and a negotiation need the student to read a person, sit with a silence, and finish the encounter. The grade mostly tracks typing speed and how long a student will sit with a long reply.

Students write about 22 words. The AI replies with about 148. They abandon 34% of attempts, mostly between turns 3 and 6, and 47% reopen the brief during an attempt. The screen describes a patient's face in paragraphs. The admin cannot set the mode or predict the cost. The instructor cannot tell how the attempt will feel until they try it themselves.

Shorter replies, a brief that stays on screen, and a clear end test the same leaving, and they need no microphone. Voice only works where the student can speak: a train, a shared room, a blocked microphone, or a speech difference all fail the same way. Typing has to remain a complete path, including WCAG 2.2 AA. Nothing ships until an admin knows what is stored, where, for how long, and what it costs per student.

The numbers are from the research pack. They are examples, and they sit in [part-1-frame-the-problem.md](part-1-frame-the-problem.md) with the assumptions and the research plan.

## How I solved it

I kept the written fixes and added speaking only where the skill is a conversation. The write-up is [part-2-explore-and-choose.md](part-2-explore-and-choose.md). The case is Mrs Jansen: take a history, 12 turns, 2 attempts. She is anxious and hard of hearing.

Three endings all count as one finished attempt.

- They speak every turn.
- They type every turn.
- They switch partway. The same attempt continues, and the second attempt is still unused.

**Admin.** Typing stays on. Speaking stays off until they approve who turns speech into text, where, how long the transcript is kept, that the recording is deleted, and a minute cap per student. Past the cap, that attempt continues in typing. These settings override the instructor. If the university refuses the page, the course stays written: short replies, the brief on screen, and a clear end.

**Instructor.** One question on the template they already publish: precise writing, or a spoken conversation. For a history, the system suggests speaking. The reason on screen is one sentence: "A history is a conversation. A written attempt shows the writing." They can set the default to typing. They cannot remove typing. They try the attempt as the student, then publish.

**Student.** Before the microphone, the screen says they can speak or type, speech becomes text, and the recording is not kept. Mrs Jansen's replies are short and captioned. The brief stays on screen. They see each spoken line and can correct it before it counts. At the turn limit, or when the history is covered, the attempt is finished and saved. They then choose which finished attempt to submit.

**Grading.** The transcript opens in the LMS grader. Each turn is marked spoken or typed. Pauses stay in the text, such as "12s silence." A reconnecting gap is the system's and is left out of the student's pauses. If every turn was typed, timing reads "not evidenced." Tone of voice leaves with the recording.

## The prototype

[`direction-b.html`](direction-b.html) is one page. A bar at the top jumps between Admin, Instructor, Student, and Grading.

- **Admin** publishes the nursing template. Title, description, and guardrails can be locked. Text is always on. Voice is a choice, with an estimated cost per participant. GDPR consent can be required.
- **Instructor** sets attempts and turns inside the admin's ranges, then previews a sample attempt and saves.
- **Student** reads the brief on the same screen, picks Voice or Chat, accepts processing of personal information, and starts. A spoken attempt shows who is speaking and notes a 12s silence. If voice stalls, the same attempt continues in text. They retry within the attempt cap, then submit.
- **Grading** opens that transcript. The recording was deleted. The rubric scores the symptom, the onset, and the pause, then an overall grade out of 3 with feedback.

The page is Astryx components inside a LearnWise theme. I compiled [`learnwise-styleguide.md`](learnwise-styleguide.md) from the public site and applied it as [`src/themes/learnwise`](src/themes/learnwise/learnwiseTheme.ts): cream page, navy ink, Satoshi, and the product indigo for actions. That replaced restyling a component library by hand.

## Open it

```bash
npm install
npx serve .
```

Open `http://localhost:3000/direction-b.html`. The page loads React from esm.sh, so it needs a network connection. The Astryx stylesheets are local, from `node_modules`.

[part-4-how-i-worked-with-ai.md](part-4-how-i-worked-with-ai.md) is a short note on how I used Cursor for the write-ups, the styleguide, and this prototype.
