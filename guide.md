# Guide for Good AI Collaboration Practices

Use these principles to effectively integrate AI (LLMs, ChatGPT, Gemini, Claude, etc.) into your daily work. The key is to shift your mindset from mere “code writer” to planner, architect, designer, product owner, project manager, patient lead developer, and “baby sitter” manager. Let AI accelerate your productivity rather than threaten it.

---

## 1. Why AI Matters

- **Stay Relevant:** AI isn’t a sign of weakness. It’s a tool for anyone who wants to remain impactful in an environment that prizes adaptability.
- **Broader Use:** We’ve used some form of AI (autocomplete, code linting, etc.) for years. Today’s models are more accessible, making deeper collaboration possible.
- **Extend Your Reach:** AI can help you break down tasks, generate ideas, and catch blind spots. Ignore it at your own risk.

---

## 2. Your New Roles

1. **Planner**
   - Know what you want to build and how you’ll measure success.
   - Outline features, goals, and milestones for the AI to reference.

2. **Architect**
   - Envision the system’s structure.
   - Ensure the AI’s outputs align with the overall design.

3. **Designer**
   - Clarify user flows and experience.
   - Direct the AI toward solutions that match real user needs.

4. **Product Owner**
   - Prioritize features and set the roadmap.
   - Keep the AI informed about business goals and constraints.

5. **Project Manager**
   - Track tasks, deadlines, and deliverables.
   - Maintain a shared context (e.g., `.notes/` folder) so the AI knows current priorities.

6. **(Patient) Lead Developer**
   - Guide the AI in coding tasks.
   - Review code suggestions carefully, as you would a junior developer’s pull request.

7. **(Baby Sitter) Manager**
   - Oversee the AI’s “work.”
   - Correct misinterpretations, steer it away from irrelevant contexts, and ensure alignment with project goals.

### Not a Teacher

- You can’t truly “teach” an LLM in the same way you teach a human.
- Large language models learn through specialized training pipelines, not via ad-hoc advice in a single session.
- **Workaround:** Provide context repeatedly using system prompts, `.notes/`, or specialized instructions.

---

## 3. The Key Mindset: Humility + Curiosity

- **Ask Good Questions:** Quality prompts lead to better answers.
- **Listen and Adapt:** Iterate on the AI’s feedback. Ask “Why?” to uncover hidden assumptions.
- **Stay Skeptical:** Too much agreeableness leads to critical blind spots. Validate the AI’s recommendations with real tests.

---

## 4. Approaches for New vs. Mature Projects

- **New Projects:**
  - Document everything up front (requirements, architecture, design).
  - Think in a more “waterfall” style to feed the AI well-defined specs.

- **Mature Projects:**
  - Incremental updates.
  - Maintain living documentation to keep track of evolving requirements and architecture.

---

## 5. Problem Decomposition

- **Keep It Small:** LLMs consider the entire input at once. The more you cram in, the higher the risk of losing focus.
- **Break Tasks Down:** Provide smaller, well-defined chunks to the AI.
- **Sequence Them:** Outline each subtask as a separate prompt and reassemble the solutions yourself.

---

## 6. Living Documentation

- Maintain an ongoing record of strategic decisions and lessons learned in `.notes/`.
- Update documents like `project_overview.md` and `task_list.md` with new insights, keeping your AI in sync.
- Approach each LLM conversation as an iterative design review: specify changes, track them, and feed those changes back into your docs.

---

## 7. Development Strategy and Continuous Evolution

- **Iterate and Refine:** Each new insight should reflect in both your code and your documentation.
- **Focus on Architecture:** Good architecture decisions now mean fewer headaches later.
- **Validate Assumptions:** AI may skip verification of real-world constraints. You must anchor suggestions in reality.

---

## 8. Example Setup with Cursor IDE

### 8.1 Project Setup

Use a clear project structure to help both you and the AI navigate the codebase.

1. **.cursorrules**
   Defines how the AI operates (e.g., always read `.notes/project_overview.md` and `.notes/task_list.md`, never break type safety, etc.).

2. **.cursorignore**
   Excludes unimportant files (like `/node_modules` or build outputs) from the AI’s view.

3. **.notes/**
   A knowledge hub for your AI collaboration.
   - `project_overview.md`: Goals, architecture, key features.
   - `task_list.md`: Tasks, statuses, assignments.
   - `directory_structure.md`: A map of the repo.
   - `meeting_notes.md`: Log of AI interactions, Q&A, and decisions.

### 8.2 Prompting in Cursor

- Use `@filename` references to focus the AI on relevant code or docs.
- Ask for self-evaluation: “Gemini, how would you improve this function? Explain your reasoning.”
- Encourage Socratic problem-solving: “Claude, what assumptions are we making here? Could any be incorrect?”

---

## 9. Prompt Mastery

- **Be Specific:** Ask pointed questions—avoid vagueness.
- **Use MECE:** Break big tasks into smaller, mutually exclusive parts.
- **Ask “Why” and “What If”:** Force the model to reveal assumptions and handle edge cases.
- **Remember When:** Refer back to prior decisions (“Gemini, recall our plan for optimistic UI updates—how do we apply it to tasks?”).
- **Iterate:** Rerun prompts until you get clarity. The first draft is rarely the final.

---

## 10. Workflow Tips

- **Make Atomic Commits:** Save incremental progress.
- **Commit Often:** Each step informs the next.
- **Keep a Consciousness Stream:** Update `meeting_notes.md` to track your dialogues, ideas, and changes.

---

## Conclusion

Working with AI in its current state means becoming a proactive orchestrator rather than a purely hands-on coder. You guide the AI, question assumptions, and refine outputs. As AI grows more advanced, you’ll adapt—but the best practices of clear documentation, humble inquiry, and careful review remain vital. Embrace AI daily and watch your impact on delivery cycles multiply.

# Real-World Generative AI Use Cases

