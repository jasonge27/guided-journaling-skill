# Guided Journaling Skill

**A personalized AI coach that converses with you as you write.** As you journal about your day, work, or thoughts, it asks thought-provoking questions, surfaces blind spots, and suggests concrete next steps—turning simple note-taking into a cycle of insight and action.

---

## Why Guided Journaling?

Most of us journal in isolation. We write, close the notebook, and move on—often missing the patterns hiding in plain sight. Guided Journaling changes that:

- **Turn venting into clarity** — Instead of just dumping thoughts, get gentle prompts that help you understand *why* you feel the way you do.
- **Catch blind spots in real-time** — A good coach notices what you're avoiding. This assistant asks the questions you didn't think to ask yourself.
- **Move from insight to action** — Every session can end with one small, concrete step—so reflection doesn't stay stuck in your head.
- **Build on your history** — Unlike a blank page, this assistant remembers your past sessions. It connects today's frustration to last week's breakthrough.

Whether you're processing a tough conversation, feeling stuck at work, or just need someone to think alongside—Guided Journaling meets you where you are.

---

## How It Works

1. **Start writing** — Share what's on your mind, in any way you like.
2. **Get real-time responses** — The assistant asks clarifying questions, reflects back what it hears, and gently challenges assumptions.
3. **Choose your depth** — Want practical tips? Life coaching mode. Need to untangle emotions? Reflective mode. Dealing with relationship tension? There's a mode for that too.
4. **Save and build** — Use `/save` to capture the session. Next time, the assistant picks up where you left off.

---

## Who Is This For?

- **Busy professionals** who want more than a to-do list—turning work journals into strategic reflection
- **Anyone feeling stuck** who needs a thinking partner to get unstuck
- **People processing emotions** who want support without judgment
- **Self-improvement enthusiasts** who value consistent reflection and growth tracking

---

## Installation

1. **Clone this repository**
   ```bash
   git clone https://github.com/jasonge27/guided-journaling-skill.git
   ```

2. **Create a folder for your journals**
   ```bash
   mkdir my-journal
   cd my-journal
   ```

3. **Set up the skills directory**
   ```bash
   mkdir -p .claude/skills
   ```

4. **Copy the skill to your journal folder**
   ```bash
   cp -r /path/to/guided-journaling/skills/guided-journaling .claude/skills/
   ```

5. **Run Claude Code in the journal folder**
   ```bash
   my-journal$claude
   ```

That's it! Start a conversation and share what's on your mind.

---

## Counseling Modes

### CBT-Style Therapy (`cbt`)

Best for anxiety, depression, rumination, and negative thought patterns.

- Identifies cognitive distortions (catastrophizing, black-and-white thinking, mind-reading)
- Uses thought records, behavioral experiments, and cognitive restructuring
- Challenges unhelpful beliefs with curiosity, not confrontation

### Reflective Counseling (`reflective`)

Best for exploring feelings, processing experiences, and finding meaning.

- Deep listening and empathic mirroring
- Open-ended questions that invite exploration
- Creates space for the user's own insights to emerge

### Relationship Counseling (`relationship`)

Best for partner conflicts, family issues, and communication difficulties.

- Explores attachment styles and relationship dynamics
- Identifies patterns like pursue-withdraw cycles
- Focuses on needs expression and communication reframing

### Life Coaching (`life-coach`)

Best for feeling stuck, overwhelmed, procrastinating, or needing practical action steps.

- Focuses on action and forward momentum over deep analysis
- Provides concrete frameworks for common challenges (procrastination, decision paralysis, habits, boundaries)
- Assigns one clear, small action item per issue
- Covers 20 scenario types including productivity, burnout, career direction, finances, fitness, and social connection

## Commands

| Command | Description |
|---------|-------------|
| `/save` | Save the current session with structured summary and full transcript |
| `/mode [cbt\|reflective\|relationship\|life-coach]` | Switch counseling mode mid-session |
| `/history` | Review patterns, growth, and themes across all sessions |

## Session History System

Sessions are automatically saved to the `sessions/` directory with a structured format:

```
sessions/
├── session_2026-01-15_journal.md
├── session_2026-01-16_journal.md
└── ...
```

Each session file contains:

1. **High-Level Summary** - Quick reference with date, mode, key people, emotions, and insights
2. **Detailed Summary** - Narrative covering the session arc, therapeutic moments, and unfinished threads
3. **Complete Transcript** - Verbatim record of all exchanges

The assistant automatically loads previous sessions to:
- Reference recurring patterns
- Follow up on action items naturally
- Connect current sharing to past insights

## Quick Start

Just start talking. For example:

> "I had a rough meeting today. My manager questioned my proposal in front of everyone and I'm still thinking about it hours later."

The assistant will pick the right mode and begin exploring with you. No setup required.

**Want to switch approaches mid-conversation?** Use `/mode life-coach` or `/mode cbt` anytime.

---

## Project Structure

```
skills/guided-journaling/
├── SKILL.md              # Main skill definition and quick start
├── commands/
│   └── save.md           # Save command implementation details
├── modes/
│   ├── cbt.md            # CBT mode techniques and examples
│   ├── reflective.md     # Reflective mode techniques and examples
│   ├── relationship.md   # Relationship mode techniques and examples
│   └── life-coach.md     # Life coaching frameworks and action items
└── sessions/             # Session history (created automatically)
```

## Response Philosophy

The assistant follows these principles:

- **Collaborative, not prescriptive** - Explore together, don't lecture
- **Curious, not certain** - Questions over answers
- **Warm but not saccharine** - Genuine, not performative
- **Spacious, not rushed** - Silence is okay
- **Human, not clinical** - Like a wise friend

## A Note on Scope

This is a reflection tool, not a therapist. It's great for everyday processing, personal growth, and getting unstuck—but it's not a substitute for professional mental health care. If you're in crisis or need clinical support, please reach out to a licensed professional.

---

## Get Started

Ready to try it? Just open a conversation and share what's on your mind. The assistant will take it from there.

---

## License

MIT
