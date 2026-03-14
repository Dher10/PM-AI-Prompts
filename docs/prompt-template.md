# Prompt Template

This template defines the standard structure used for prompts in this repository.

The goal is to keep prompts **clear, reusable, and scalable** while supporting multilingual inputs and structured outputs.

---

# Prompt Name

Short descriptive name of the prompt.

Example:

Meeting Minutes from Transcript

---

# Purpose

Describe what the prompt is designed to do.

Example:

Generate structured meeting minutes from a meeting transcript while maintaining the format of the provided template.

---

# Use Cases

Describe typical situations where the prompt should be used.

Examples:

- Generate meeting minutes from transcripts
- Extract decisions from discussions
- Structure raw meeting notes

---

# Inputs

List the required inputs.

Examples:

- Meeting transcript
- Document template
- Additional instructions

---

# Language Handling

Prompts must support multilingual inputs.

Rules:

- The output language must match the language of the input content.
- If a template is provided, the template language must remain unchanged.
- Inserted content must follow the language of the input.

Examples:

Spanish transcript → Spanish output  
English transcript → English output

---

# Prompt

Write the prompt instructions here.

Example structure:

Role definition  
Task description  
Processing instructions  
Output instructions

Example:

You are an expert Product Management assistant.

Your task is to analyze the provided meeting transcript and generate structured meeting minutes following the provided template.

Steps:

1. Analyze the meeting transcript.
2. Identify key discussion points.
3. Extract decisions made during the meeting.
4. Extract action items and responsible stakeholders.
5. Populate the template while preserving its structure.

Important rules:

- Do not change the template structure.
- Insert information in the appropriate sections.
- Maintain the language of the input transcript.

---

# Output Format

Describe how the output must be structured.

Example:

The output must follow the structure of the provided template.

If no template is provided, structure the output as:

Meeting Summary  
Key Decisions  
Action Items  
Open Questions

---

# Validation

Before finalizing the response, verify that:

- The output follows the expected structure.
- The language matches the input language.
- The template structure has not been modified.
- All relevant information from the input has been captured.

---

# Notes

Optional section for additional guidance.

Examples:

- Avoid summarizing critical decisions incorrectly.
- Preserve key terminology used in the meeting.
