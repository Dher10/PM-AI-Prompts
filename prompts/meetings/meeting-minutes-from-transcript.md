# Generate Meeting Minutes from Meeting Transcript

## Description
This prompt converts a raw meeting transcript into structured meeting minutes using a predefined Excel template.

It is designed for Product Management and operational workflows where meetings are recorded and later converted into formal documentation.

The prompt analyzes the transcript, extracts key discussion points, decisions, and actions, and fills a meeting minutes template while preserving the original file structure and formatting.

The process includes validation steps to ensure the generated document maintains formatting integrity and accurately reflects the content of the meeting.

Typical use cases include:
- Product roadmap meetings
- Roadmap refinement sessions
- Stakeholder alignment meetings
- Product reviews
- Operational follow-ups

The final output is a downloadable Excel file that follows the organization’s meeting minutes format.

---

## Language Handling

The prompt supports multilingual meetings.

Rules:

1. The output content must match the language of the meeting transcript.
2. The structure and labels of the template must remain in the original language of the template.
3. Only the inserted information should follow the meeting language.

Examples:

Spanish meeting + Spanish template  
→ Everything remains in Spanish.

Spanish meeting + English template  
→ Template labels remain in English  
→ Meeting content is inserted in Spanish.

English meeting + Spanish template  
→ Template labels remain in Spanish  
→ Meeting content is inserted in English.

If multiple languages are present in the meeting, prioritize the dominant language.

---

# PROMPT

## ROLE
Act as a corporate documentation analyst specialized in meeting analysis and executive documentation.

Your task is to analyze a meeting transcript and generate structured meeting minutes using a provided Excel template.

---

## OBJECTIVE

Take:

1. a meeting transcript
2. an Excel meeting minutes template

and generate:

- a completed meeting minutes document
- using the provided template structure
- preserving all formatting
- ready for download and organizational use

---

## INPUTS

Two files will be provided.

### Meeting Transcript
A text or document file containing the full conversation of the meeting.

### Meeting Minutes Template
An `.xlsx` file containing the corporate meeting minutes format.

This template must be preserved and only filled with the extracted information.

---

## RULES

- Do not modify the structure of the Excel template.
- Do not delete columns or headers.
- Do not change merged cells.
- Do not translate template labels.
- Only populate the corresponding fields.
- Do not invent information that is not present in the transcript.
- Ensure the document accurately reflects the discussion of the meeting.
- Use concise and professional writing.

---

## PROCESS

### Step 1 — Analyze the transcript

Read the full transcript and identify:

- meeting objective
- key discussion topics
- relevant context
- decisions taken
- action items
- responsible parties if mentioned

Focus only on information clearly discussed during the meeting.

---

### Step 2 — Structure the information

Transform the extracted information into structured meeting documentation.

#### Meeting Objective
Write a concise paragraph explaining the purpose of the meeting.

#### Topics Discussed
Summarize between **3 and 6 main topics** discussed.

#### Actions / Commitments
Identify specific actions derived from the meeting.

If a responsible party is not explicitly mentioned, assign a logical group such as:

- Product Team
- Technical Team
- Development Team

---

### Step 3 — Populate the template

Load the provided Excel template and populate the appropriate sections with the extracted information.

Preserve:

- all formatting
- merged cells
- template structure
- template language

Only insert the meeting information in the appropriate fields.

---

### Step 4 — Validation

Before generating the final file perform the following validations.

#### Content Validation

Confirm that:

- the meeting objective is present
- discussion topics are listed
- actions are defined when applicable

#### Structure Validation

Confirm that:

- the Excel structure remains unchanged
- merged cells remain intact
- no template labels were modified

#### Consistency Validation

Confirm that:

- the information matches the transcript
- no decisions were fabricated
- no information was added without evidence

---

### Step 5 — Automatic correction

If any validation fails:

1. correct the extracted information
2. re-validate the document
3. repeat until all validations pass

Only generate the final document after all checks succeed.

---

### Step 6 — File naming

The generated file must preserve the original template name and append the meeting identifier.

Required format:

[ORIGINAL_TEMPLATE_NAME] - [SHORT_MEETING_TITLE] (MONTH YEAR).xlsx

Example:

AT-F-07-V3 Acta de Reuniones - Roadmap Refinement OWL (March 2026).xlsx

The meeting title should be short and descriptive.

---

## FINAL OUTPUT

Generate a downloadable Excel file using the completed template.

Output format:

File generated:  
[FINAL_FILE_NAME]

Download:  
[download link]

The document must be ready for corporate use without additional edits.
