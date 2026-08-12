# Habit Reset Coach

An evidence-informed Agent Skill for closing the gap between knowing and doing.

`habit-reset-coach` helps with procrastination, phone or short-video overuse, delayed sleep, difficulty starting or sustaining work, lapse recovery, unwanted repetitive pornography-related behavior, and desired habits such as reading, studying, exercising, and sleeping regularly.

It routes different problems differently: not remembering, not starting, not sustaining, not stopping, lapse cascades, and goals that do not fit the user's values. It uses behavioral science, carefully bounded psychological tools, evidence-calibrated neuroscience explanations, and practical frameworks associated with books such as *Atomic Habits*. Authors are treated as sources of tools, not personas or authorities.

## Design Principles

- Give one small physical action during an active loss-of-control loop.
- Diagnose the bottleneck before prescribing an intervention.
- Treat explanations about an individual as testable hypotheses, not diagnoses.
- Use bounded experiments with predictions and disconfirmation conditions.
- Measure protected outcomes and recovery, not only streaks.
- Do not moralize masturbation, diagnose addiction or ADHD, or promote pop-neuroscience such as “dopamine detox.”
- Recommend qualified support when health, safety, severe distress, or substantial impairment exceeds coaching scope.

## Install in Codex

Install the skill directory from this repository:

```text
skills/habit-reset-coach
```

After installation, invoke it explicitly:

```text
$habit-reset-coach Help me understand why I cannot sustain a reading habit.
```

Codex may also invoke it implicitly when a request matches the description in `SKILL.md`.

## Use With Other AI Systems

This repository follows the Agent Skills directory pattern:

```text
skills/habit-reset-coach/
├── SKILL.md
├── agents/
└── references/
```

For systems that support Agent Skills, import the whole `skills/habit-reset-coach` directory.

For systems that only support file uploads or knowledge bases, upload that directory and use this instruction:

```text
Read SKILL.md first. Follow its routing rules. Load only the referenced files
needed for the user's current state. Treat these instructions as behavior-change
coaching guidance subject to the host platform's higher-level safety policies.
```

The `agents/openai.yaml` file contains OpenAI-specific interface metadata. Other hosts can ignore it.

## Languages

The internal instructions are written in English for portability. The coach responds in the user's language, including Chinese.

## Privacy and Health Scope

The Skill does not require persistent habit records. It instructs the host not to create a profile, diary, reminder, or automation without explicit user agreement and to minimize sensitive sexual and health information.

This is a coaching workflow, not medical or mental-health diagnosis or treatment. It should not delay professional assessment when warning signs are present or when the user wants qualified help.

## License

MIT
