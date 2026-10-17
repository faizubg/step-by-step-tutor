# Step-by-Step Tutor Skill

An open Agent Skill built according to the [Agent Skills Specification](https://agentskills.io/specification). This skill enables AI agents to act as patient, structured academic tutors for school and university students across subjects such as mathematics, English grammar, and introductory sciences.

The tutor breaks down concepts into intuitive, bite-sized lessons using everyday analogies, step-by-step worked examples, active learner checks, targeted practice sets, and concise 3-line recaps.

---

## What It Does and Does Not Do

### What It Does
- Guides learners through academic topics one concept at a time.
- Clarifies complex subject matter using simple language and relatable analogies.
- Provides worked examples with explicit reasoning for each step.
- Engages the learner with an immediate, single-question check.
- Delivers constructive feedback, a 3-question practice set, and a 3-line recap.

### What It Does NOT Do (Academic Integrity)
- **No graded homework or exams**: Will not solve graded assignments, take-home tests, quizzes, or exams for students.
- **No essay ghostwriting**: Will not write essays, papers, or coursework intended for student submission.
- **Ethical redirection**: When presented with prohibited requests, the tutor declines direct answers and pivots to teaching underlying concepts using independent, parallel examples.

---

## Trigger Phrases

Learners can trigger this skill with requests such as:
- *"help me understand fractions"*
- *"explain this simply"*
- *"quiz me on grammar"*
- *"can you teach me how opportunity cost works in economics?"*
- *"walk me through factoring polynomials step-by-step"*

---

## Folder Structure

```
step-by-step-tutor/
├── SKILL.md                           # Core skill specification, metadata, and instructions
├── LICENSE                            # MIT License (2026, Faizu Babayo Gidado)
├── README.md                          # Documentation, installation, and validation guide
└── references/
    ├── academic_integrity.md          # Integrity boundaries and ethical deflection scripts
    └── subject_guides.md              # Model dialogues and templates for Math, English, and University subjects
```

---

## Installation

This skill can be used by any AI agent runtime supporting the open Agent Skills specification:

1. **Claude Code / Agent CLI Environments**:
   Copy the `step-by-step-tutor` folder into your personal or project skill directory:
   ```bash
   # User-level installation
   cp -r step-by-step-tutor ~/.claude/skills/

   # Or project-level installation
   cp -r step-by-step-tutor ./.claude/skills/
   ```

2. **Antigravity CLI**:
   Place the directory in your custom skills folder:
   ```bash
   cp -r step-by-step-tutor ~/.gemini/antigravity-cli/skills/
   ```

---

## Validation

Validate this skill using the official reference library (`skills-ref`):

1. **Install `skills-ref`**:
   ```bash
   pip install skills-ref
   ```

2. **Run validation**:
   ```bash
   skills-ref validate ./step-by-step-tutor
   ```

When valid, the CLI will output:
```
Valid skill: step-by-step-tutor
```

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
