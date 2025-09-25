# UX Research Repository

Welcome to our UX research repository! This repository is designed to **organize interview data, proto-personas, and refined personas** for your product or project. It’s structured to make it easy to collect, clean, and synthesize insights from user research.

---

## 1. Interview Workflow

This workflow helps you go from raw interview audio to structured insights.


This document describes the standardized workflow for conducting, processing, and documenting in-person interviews.  

The output of each interview should result in **two files** committed to the repository:
1. `cleaned-transcript.md`
2. `proto-persona.md`

---

## Workflow Steps

### 1. Conduct Interview
- Conduct interviews in-person or virtually.
- Use a voice recording app (e.g., Voice Memo on iPhone) with a clip-on mic for better clarity.
- Make sure to note **interviewee details**, **date/time**, **location**, and **any special context**.

---

### 2. Prepare Transcript
- Copy the audio transcript from the voice memo.

---

### 3. Generate Documentation with ChatGPT
Paste the transcript into ChatGPT with the following prompt:
```text
I have an interview transcript. Please generate two separate documents:

1. cleaned-transcript.md

Rewrite the transcript into a clean Q&A format.

Start with metadata about the interviewee and interview details.

Use the following template structure at the top:

# Interview 1

## Interview Details
- Interviewee: [Interviewee Name]
- Interviewer: [Interviewer Name]
- Date and time: [Interview Date and Time]
- Location: [Interview Location]
- Details: [Interview Details]

2.proto-persona.md

Summarize the interviewee into a proto persona in markdown format.

Use this structure:

# Proto Persona: [Name/Identifier]

## Demographics
- Age:  
- Nationality:  
- Current Location:  
- Education:  
- Career Stage:  
- Role:  

## Goals
-  

## Frustrations
-  

## Needs
-  

## Behaviors & Context
-  

## Tools & Technology
-  

Make sure both documents are clean and copy-paste ready in Markdown format.

Here is the raw transcript:
[PASTE TRANSCRIPT HERE]
```


---

### 4. Save Outputs
- Save the first output as `cleaned-transcript.md`.
- Save the second output as `proto-persona.md`.

---

### 5. Commit to Repository
- Place the files in your repository:
```bash
01-interviews/
interview-01-lavanya/
cleaned-transcript.md
proto-persona.md
```

- Commit both files into the appropriate folder of your repository for documentation.  
Use the following commit message format:  
`docs: add interview [#] transcript and proto persona`
Where `[#]` is the interview number.

---

## 2. File Structure Overview

Here’s an example of how to organize your UX research files:

```bash
├── 01-interviews/
│ ├── interview-01-lavanya/
│ │ ├── cleaned-transcript.md
│ │ └── proto-persona.md
│ ├── interview-02-xyz/
│ │ ├── cleaned-transcript.md
│ │ └── proto-persona.md
│ └── ...
├── 02-synthesis/
│ ├── personas/
│ │ ├── persona-lavanya.md # Refined persona from multiple proto-personas
│ │ └── persona-xyz.md
│ ├── patterns/
│ │ └── common-behaviors.md
│ └── insights/
│ └── key-findings.md
└── README.md
```

### Key Notes on Files

| File/Folder | Purpose |
|-------------|---------|
| `cleaned-transcript.md` | A **readable Q&A transcript** of a single interview. Useful for reviewing what was said without sifting through audio. |
| `proto-persona.md` | **Initial persona based on one interview**. Contains behaviors, goals, pain points, and context. Often includes quotes. |
| `persona-*.md` | **Refined personas** created after synthesizing multiple proto-personas or research sources. These are generalized, validated, and ready to guide design decisions. |
| `patterns/` | A place to summarize trends observed across multiple interviews, such as common behaviors, pain points, or motivations. |
| `insights/` | A folder to capture **key research takeaways** that inform product or UX decisions. |

---

## 3. Tips for Beginners
- Always capture **context**: location, device, and any external factors affecting the interview.
- Keep proto-personas **faithful to the interview** — don’t overgeneralize at this stage.
- Refined personas should be **synthesized and validated**, not just a copy of a single proto-persona.
- Use **consistent naming conventions** to make it easy to track interviews, proto-personas, and refined personas.

---

This structure ensures you can scale your UX research repository, keep all raw and processed data organized, and create actionable insights for your team.

