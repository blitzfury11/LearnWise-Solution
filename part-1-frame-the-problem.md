# Part 1: Frame the problem

Numbers come from the research pack. They're examples, not proof.

Today, every Custom Learning Experience is text-based, with students interacting one message at a time. While this works well for law, it is less suitable for other fields, such as nursing history-taking, counselling intakes, or negotiation exercises. In these situations, students are often assessed more on their ability to type quickly and write lengthy responses than on the practical skills they are meant to demonstrate. Important visual details, such as a patient's facial expressions or documents on a table, are reduced to written descriptions that students may easily overlook. Meanwhile, admins have little control over the interaction format or its costs, and instructors cannot easily predict what the student experience will actually look like. As a result, these limitations can affect student engagement and accessibility, leading to higher dropout rates and more incomplete learning experiences.

## Insights that matter most

1. The skill should determine how students practise. Nursing students need to read a patient's reactions while talking to them. Negotiation depends on silence, timing, and knowing when to respond. Law, on the other hand, relies on precise written communication. Using the same format for every course means that some students are not practising the skills they are actually being assessed on.

2. Long replies and a missing brief may be just as problematic as typing-only. Students write around 22 words per message, while the AI responds with approximately 148. Around 34% of attempts are abandoned, mostly between turns 3 and 6, and 47% of students reopen the brief during an attempt. These numbers are connected, but they don't prove that typing is the main problem. A better experience doesn't necessarily mean introducing voice. Shorter replies, a brief that stays visible, and clearer completion criteria could address the same issues more simply.

3. Voice only works when students are actually able to use it. One student completed an attempt on a train and couldn't speak. The same problem applies to shared rooms, blocked microphones, or students who have difficulty speaking or hearing. Courses can offer voice as a default, but typing must remain a complete alternative. Accessibility, including WCAG 2.2 AA, needs to be part of the experience from the start.

4. Trust needs to be established before students even begin. Admins are unlikely to approve a new interaction mode without knowing what data is stored, where it goes, how long it is kept, and what it costs per student. Instructors already preview experiences an average of 3.4 times, and 1 in 5 republish within a week. Yet one instructional designer still describes the experience as having "no idea what the student actually experiences until I try it myself. Several times." Even with previews available, instructors don't necessarily trust what they see.

## What I don't trust yet

Students may be leaving because AI replies are too long and the brief disappears, which would explain the same patterns seen in stop-and-start conversations. The 71-second pause includes reading a 148-word response and typing a reply, so it cannot be treated as pure thinking time. There is also no evidence in the research pack that students actually want to speak aloud. A list of skills does not always translate neatly into a choice between voice and text. On top of that, speech recognition may not be reliable enough for grading across English, Dutch, Spanish, and different English accents.

## The conflict that decides the rest

I'd delete the recording but keep the transcript. Timing could still be captured as a note, such as "12s silence", allowing instructors to assess pauses without needing access to the audio. However, tone and presence would be lost. Voice could help a nursing student who types slowly in her second language, but a poorly recognised accent could make that same feature work against her.

## Who is hurt most, and where text is enough

Nursing history-taking and counselling intakes are affected the most. Students cannot properly read the other person's reactions, there is no real sense of time pressure, and the patient responds with an essay instead of a natural answer. Negotiation comes next, since silence and timing are important parts of the exercise but disappear in a text-only interaction.

Students working in a second language, students with dyslexia, and those who think out loud may end up being assessed on their writing rather than the skills they are supposed to demonstrate. First-year students describe the experience as "texting someone who replies with an essay", with many abandoning their attempts between turns 3 and 6.

Law works well in text, as do later written assignments such as research proposals or create-and-reflect exercises. Typing must also remain available for students studying on a train, in shared spaces, without a microphone, or with a speech difference.

Ultimately, a strong writer can appear competent in a conversation that the exercise never actually tested.

## Key assumptions

A star marks a critical assumption: if it turns out to be wrong, the first product decision changes.

| # | Assumption | If this is wrong |
| --- | --- | --- |
| A1 ★ | Students can access and use a microphone inside Canvas or Brightspace, on their phones, and in the places where they actually study. | Don't make voice the default. Keep text first. |
| A2 ★ | The university's privacy review will allow speech-to-text processing followed by audio deletion, provided we clearly explain who processes the data, where, and how long the transcript is kept. Speech-to-text still counts as GDPR processing. | Voice cannot launch. Focus on improving the text experience instead. |
| A3 ★ | Speech recognition is accurate enough for grading in English, Dutch, Spanish, and accented English. | Keep voice for practice, but not for grading. |
| A4 ★ | Spoken and typed attempts can be assessed fairly using the same rubric, or the rubric clearly explains what each format demonstrates. | Students who cannot speak risk receiving lower grades for the wrong reasons. |
| A5 ★ | Live AI replies can still feel conversational at the speed and reliability we can deliver. | If voice feels broken, a faster text-based chat may be the better solution. |
| A6 | Instructors can grade transcripts with pause notes, such as "12s silence", without listening to recordings, and in roughly the same time as today. | Grading may require recordings, making privacy approval more difficult. |
| A7 ★ | Students leave because replies are too long, the brief disappears, and completion is unclear, rather than mainly because they cannot speak. | Improving text chat may not reduce the 34% abandonment rate. Voice needs to be explored earlier. |

## Research plan

Before building anything, I'd want to understand whether the problems we're seeing are caused by the current text experience, and whether universities would approve voice at all. I'd start with the simplest tests and only move towards a live pilot if the evidence supports it.

First, check the existing experience. The product team could spend a few days looking at whether longer AI replies are linked to more abandoned attempts, and when students reopen the brief. I'd also run a simple spoken role-play, with a person playing Mrs Jansen and deliberately introducing pauses and a few incorrect responses. This would help test whether the interaction genuinely benefits from voice and whether it can still work with realistic delays and imperfect replies (A5, A7). If long replies explain much of the abandonment, I'd fix the text experience first. If the spoken test only works when it is smoother than the AI could realistically deliver, I wouldn't move to a live voice pilot yet.

Then, understand what admins and instructors need.

- Admins at three universities: I'd show them a one-page explanation of the proposed data flow: speech converted to text, audio deleted, transcript retained, and who processes the data, where and for how long. I'd also include an estimated cost for 100 nursing students and ask what they'd need to see before approving it, including an acceptable cost ceiling (A2).
- Six instructors across nursing, counselling, negotiation and law: I'd show them a suggested activity setup, explain why that format is recommended, and let them try it as a student. I'd then ask them to grade the same case using the transcript alone and the transcript with pause notes, to understand whether those notes provide useful evidence (A4, A6).

Finally, test the experience with students and engineering.

I'd speak to eight students with different needs and circumstances, including a second-language speaker, a student with dyslexia, a commuter, and someone who cannot rely on speech. I'd talk to them in the places where they normally study and test microphone access within a copy of the LMS experience (A1).

In parallel, engineering would check microphone permissions in Canvas and Brightspace, speech recognition across Dutch, Spanish and accented English, and the expected response delays and cost per minute (A1, A3, A5).

After building, run a small pilot.

If the earlier research supports it, I'd pilot the experience in one nursing course and one negotiation course, keeping text available throughout. I'd compare actual costs with the estimates, check that no additional data is being stored, and time how long instructors take to grade ten paired records. I'd also track which mode students choose, when they switch between them, and where they abandon an attempt, then interview six students about their experience.

I wouldn't use the pilot for grading unless both the instructor and admin were comfortable with it. Before making that decision, I'd want to understand how they would assess spoken and typed attempts side by side. In particular, students with accents or those using a second language must not be disadvantaged by speech recognition or by the choice of interaction mode.
