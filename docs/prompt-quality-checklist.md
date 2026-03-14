# Prompt Quality Checklist

This checklist helps validate prompts before adding them to the repository.

The objective is to ensure prompts remain **clear, reliable and reusable**, while avoiding unnecessary complexity or ambiguity.

Before committing a new prompt, review the following points.

---

# 1. Clarity

- [ ] The prompt clearly states what the model must do.
- [ ] Instructions are direct and easy to understand.
- [ ] There are no ambiguous or vague instructions.

Example of vague instruction:

"Help with this document."

Better instruction:

"Analyze the document and extract the key decisions."

---

# 2. Purpose

- [ ] The prompt clearly defines the purpose of the task.
- [ ] The expected outcome is easy to understand.

The reader should immediately know **what the prompt is designed to produce**.

---

# 3. Input definition

- [ ] The prompt clearly defines the inputs required.
- [ ] Inputs are described in a way that avoids confusion.

Examples of inputs:

- meeting transcript
- template document
- supporting data

---

# 4. Structured instructions

- [ ] The task is structured into logical steps when needed.
- [ ] The instructions guide the model through the reasoning process.

Example:

1. Analyze the content.
2. Extract key information.
3. Organize the output.

---

# 5. Output structure

- [ ] The prompt defines the expected output structure.
- [ ] Sections or headings are clearly defined.

Example:

Meeting Summary  
Key Decisions  
Action Items  
Open Questions

---

# 6. Multilingual handling

- [ ] The prompt supports multilingual inputs.
- [ ] The output language matches the input language.
- [ ] Templates preserve their original language.

---

# 7. Hallucination control

- [ ] The prompt explicitly prevents the model from inventing information.
- [ ] Instructions include a rule such as:

"Do not generate information that is not present in the input."

---

# 8. Validation step

- [ ] The prompt includes a validation stage before final output.
- [ ] The model verifies structure, language and completeness.

Example validation rule:

"Verify that the output follows the required structure before finalizing."

---

# 9. Reusability

- [ ] The prompt can be reused in different scenarios.
- [ ] Instructions are not overly dependent on a single use case.

Reusable prompts increase the value of the prompt library.

---

# 10. Simplicity

- [ ] The prompt avoids unnecessary complexity.
- [ ] Instructions are as simple as possible while remaining effective.

If a prompt feels overly complicated, it should probably be simplified.

---

# Final check before commit

Before committing a prompt to the repository, verify:

- [ ] The prompt follows the repository template
- [ ] The instructions are clear and structured
- [ ] The output format is defined
- [ ] Multilingual handling is supported
- [ ] The prompt is reusable

If all items are satisfied, the prompt is ready to be added to the repository.
