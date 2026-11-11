# Custom Learning Experiences

## Design rationale

### Key decisions and trade-offs

I explored two directions before choosing Option B as my proposed direction for this assignment. While I believe voice could add value to certain learning experiences, I wouldn't necessarily jump straight into introducing it in a real product project. I'd first want to improve the existing text experience, understand whether those changes solve some of the current problems, and identify where voice would genuinely make a difference.

- Option A – Improve text-based role-play: shorter AI replies, a brief that stays visible, and clearer attempt completion. This addresses existing friction and supports activities where precise written communication is the skill being assessed.
- Option B – Add flexible voice interaction: allow students to speak, type or switch between both within one attempt. This could better support activities such as nursing and negotiation, where listening, timing and spoken interaction matter.

For this assignment, I chose to develop Option B because it offers more flexibility across different learning experiences. The proposed design builds on the improvements identified in Option A, while exploring how voice could work alongside text.

The main trade-offs are flexibility versus consistent grading, realistic interaction versus privacy, and accessibility versus standardisation. Voice introduces additional questions around data processing, recognition accuracy, cost and transcript quality. My initial preference is to let students choose how they interact, while keeping typing as a complete alternative. However, this needs to be tested to ensure different modes can be assessed fairly.

## Part 1 – Understanding the problem

### Problem framing

The text-only format works for activities that assess written communication, but is less suited to skills involving listening, reading reactions and timing. It can end up testing how well students type rather than the skill they are practising. Long AI replies, a disappearing brief and unclear completion may add further friction. Instructors also lack visibility into the student experience, while administrators need predictable costs and confidence in privacy.

### Key insights

1. The skill should determine the interaction. Nursing and negotiation involve listening, reactions and timing; legal work may benefit from precise writing. One mode will not suit every activity.

2. The text experience needs improvement too. AI replies average 148 words, compared with 22 words for student messages. 34% of started attempts are abandoned, mostly around turns 3–6, and 47% of students reopen the brief. These figures don't prove the causes, but suggest testing shorter replies, a persistent brief and clearer completion.

3. Voice isn't always accessible. Students may be in shared spaces, on public transport or unable to use a microphone. Typing must remain a complete alternative.

4. Trust matters. Administrators need clarity on privacy, retention and cost. Instructors need confidence before publishing; they preview activities an average of 3.4 times, and one in five republish during the first week.

### Who is most affected?

Students practising spoken or interpersonal skills, especially in nursing and negotiation, are most limited by text-only interaction. Students who type slowly or use a second language may also struggle. However, students who cannot speak in their environment need an equally good text option. Some written activities may not need voice at all.

### What I still need to validate

I don't know whether long replies and the disappearing brief are the main reasons for abandonment. The 71-second median pause includes both reading and typing. I also need to test speech recognition across supported languages and accents, and whether instructors can fairly assess transcripts without audio.

### Assumptions and research plan

I assume institutions can approve voice processing, speech recognition is sufficiently accurate, students can switch modes without losing progress, and transcripts provide fair evidence for grading.

I would first test improvements to the text experience with students and instructors, measuring completion, brief usage and perceived clarity. If problems remain, I would run a small, consent-based voice pilot across different activities and student contexts. Instructor feedback on transcript quality would help guide decisions about privacy, cost and grading.

## Part 4 – Use of AI

1. I used Cursor to analyse the brief and research pack, organise my ideas and explore possible directions.
2. I used Cursor to draft Parts 1 and 2 from my notes, then reviewed and edited the content.
3. I used Cursor to create a LearnWise style guide from the public website and apply it with Astryx, avoiding manual restyling of the component library.
4. I used Cursor to build the prototype as a single HTML file, with the theme and Astryx stylesheets included in the repo.
5. I used the chat-council skill to review the prototype and documents against the brief and identify areas for improvement.
6. I used ChatGPT to format the rationale and polish the writing.
