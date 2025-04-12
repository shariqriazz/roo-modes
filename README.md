# Roo-Code Custom Modes Repository

This repository contains custom mode definitions for the Roo-Code VSCode extension, exploring different approaches to AI-assisted software development workflows.

## Overview

The repository is organized into two main approaches:

1.  **`builder-dynamic/`**: This directory contains the definition for a dynamic **Builder** mode. This mode acts as a project lead, dynamically generating a tailored team of specialist modes (like Architect, Designer, Developers, Reviewer) based on the specific project requirements and user preferences. It orchestrates the entire workflow using this custom-generated team.
2.  **`original-modes/`**: This directory contains the definitions for a set of 12 pre-defined specialist modes (Orchestrator, System Architect, UI/UX Designer, Frontend Developer, Backend Developer, etc.). This represents a more static approach where the user (or an Orchestrator) selects and coordinates between these fixed roles.

## Directory Structure

```
.
├── .gitignore
├── builder-dynamic/
│   ├── .roomodes                 # JSON definition for the Builder mode
│   ├── builder-dynamic.md        # Markdown definition & instructions for the Builder mode
│   └── README-builder-dynamic.md # Detailed documentation for the Builder mode workflow
├── original-modes/
│   ├── .roomodes                 # JSON definitions for all original specialist modes
│   ├── 1-orchestrator.md         # Markdown definition for Orchestrator
│   ├── 2-system-architect.md     # Markdown definition for System Architect
│   ├── ...                       # (Definitions for modes 3 through 12)
│   └── README-original-modes.md  # Documentation for the original modes and their workflow
└── README.md                     # This file - Repository overview
```

## Usage

Each directory (`builder-dynamic/` and `original-modes/`) contains:

*   A `.roomodes` file: This JSON file contains the mode definitions ready to be loaded by the Roo-Code extension. You would typically use *one* of these files at a time, depending on whether you want to use the dynamic Builder workflow or the original static modes workflow.
*   Markdown definition files (`*.md`): These files contain the detailed role definitions and custom instructions for each mode, providing human-readable insight into their logic and behavior.
*   A dedicated README file (`README-*.md`): This provides specific documentation for the workflow and usage of the modes within that directory.

Refer to the README file within each subdirectory for detailed information on how to use that specific set of modes.