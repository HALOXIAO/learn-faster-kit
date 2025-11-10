# Learn FASTER

> Accelerate learning with the FASTER framework - spaced repetition, progress tracking, and hands-on practice using AI coaching.

**[Claude Code](https://claude.com/claude-code) Only** - This tool launches Claude Code with FASTER framework coaching mode.

## What is FASTER?

-   **F**orget: Beginner's mindset
-   **A**ct: Learn by doing
-   **S**tate: Optimize focus
-   **T**each: Explain to retain
-   **E**nter: Consistent sessions
-   **R**eview: Spaced repetition

## Features

-   Auto-generated syllabi tailored to your level and goals
-   Spaced repetition review system
-   Progress tracking and reports
-   Practice exercise generation
-   Teaching-based retention prompts

## Installation

**Prerequisites:** [uv](https://docs.astral.sh/uv/) package manager

```bash
# Install uv if you haven't already
curl -LsSf https://astral.sh/uv/install.sh | sh
```

### Option 1: Persistent Installation (Recommended)

Install once and use across all projects:

```bash
uv tool install learn-faster --from git+https://github.com/cheukyin175/learn-faster-kit.git
```

Then in any project directory, simply run:

```bash
learn-faster
```

This will auto-initialize on first run and launch Claude Code with FASTER coaching mode.

### Option 2: One-Time Use

Run directly without installation:

```bash
uvx --from git+https://github.com/cheukyin175/learn-faster-kit.git learn-faster
```

### What Gets Installed

On first run, learn-faster creates:

```
your-project/
├── .claude/
│   ├── agents/practice-creator.md
│   ├── commands/
│   │   ├── learn.md
│   │   ├── review.md
│   │   └── progress.md
│   └── settings.local.json
├── .learning/
│   ├── config.json (tracks initialization)
│   ├── scripts/
│   │   ├── init_learning.py
│   │   ├── log_progress.py
│   │   ├── review_scheduler.py
│   │   └── generate_syllabus.py
│   └── references/faster_framework.md
└── CLAUDE.md
```

## Quick Start

1. **Install the tool (one time)**

    ```bash
    uv tool install learn-faster --from git+https://github.com/cheukyin175/learn-faster-kit.git
    ```

2. **Navigate to your project and run**

    ```bash
    cd your-learning-project
    learn-faster
    ```

    This will:
    - Initialize the project structure (first time only)
    - Launch Claude Code with FASTER coaching mode
    - You're ready to start learning!

3. **Start learning with the `/learn` command**
    ```bash
    /learn "Golang fundamentals"
    ```

## CLI Commands

-   `learn-faster` - Auto-init and launch Claude Code with coaching mode
-   `learn-faster init` - Force re-initialization
-   `learn-faster version` - Show version

## Commands in Claude Code

-   `/learn [topic]` - Initialize or continue learning a topic
-   `/review` - Conduct spaced repetition review session
-   `/progress` - Show detailed progress report

## Development

### Setup

```bash
# Clone the repository
git clone https://github.com/cheukyin175/learn-faster-kit.git
cd learn-faster-kit

# Install uv if needed
curl -LsSf https://astral.sh/uv/install.sh | sh

# Install dependencies
uv sync
```

## Requirements

-   Python 3.12+
-   [Claude Code](https://claude.com/claude-code)
-   [uv](https://docs.astral.sh/uv/) package manager

## License

MIT License - See LICENSE file for details

---

**Master any topic faster** with spaced repetition, active practice, and teaching-based reinforcement.
