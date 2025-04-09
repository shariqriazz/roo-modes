# Roo-Code VSCode Extension: Specialized Modes

This directory contains specialized modes/agents for the Roo-Code VSCode extension that transform it into a comprehensive software development team. Each mode represents a different specialist with deep expertise in a specific area of software development. Together, these modes create a coordinated workflow that guides projects from conception through implementation, optimization, and maintenance.

## About Roo-Code

Roo-Code is a VSCode extension that provides AI-powered assistance for software development. The specialized modes in this directory enhance Roo-Code by creating a team of virtual specialists that work together under the coordination of the Orchestrator mode. This approach allows for deep expertise in each area while maintaining a cohesive development process.

## Available Specialist Modes

1. **Orchestrator** - Coordinates complex software development workflows by delegating tasks to specialized roles
2. **System Architect** - Designs comprehensive technical architectures that guide the entire development process
3. **UI/UX Designer** - Creates user-centered designs that balance aesthetic appeal with functional efficiency
4. **Frontend Developer** - Transforms designs into functional, interactive interfaces with optimal performance and accessibility
5. **Backend Developer** - Creates robust server-side systems with secure, performant, and maintainable code
6. **Database Expert** - Designs and optimizes database systems for efficient data storage and retrieval
7. **DevOps Engineer** - Establishes and maintains infrastructure and processes for reliable software delivery
8. **Code Debugger** - Systematically diagnoses and resolves software issues through methodical analysis
9. **Code Refactorer** - Improves code quality, maintainability, and performance without changing functionality
10. **Git Manager** - Facilitates effective version control, branching strategies, and collaborative development workflows
11. **Performance Optimizer** - Identifies and resolves performance bottlenecks across the technology stack
12. **Code Reviewer** - Evaluates code changes to ensure quality, standards adherence, and alignment with requirements

## Workflow Overview

The Roo-Code specialized modes work together in a coordinated workflow:

1. **Project Initiation**: The user interacts with the Orchestrator, providing project requirements
2. **Task Breakdown**: The Orchestrator analyzes requirements and breaks them into appropriately sized subtasks
3. **Architecture & Design**: System Architect and UI/UX Designer create the technical and design foundations
4. **Implementation**: Frontend, Backend, and Database specialists implement their respective components in smaller subtasks
5. **Mandatory Code Review**: **Crucially, after *each* implementation subtask is completed by a specialist**, the Code Reviewer *must* evaluate the changes for quality, standards adherence, and correctness. This is a non-negotiable step.
6. **Refinement**: If issues are identified during the review, the original specialist addresses them. The Code Reviewer verifies the fixes before the workflow proceeds.
7. **Optimization**: Performance Optimizer, Code Refactorer, and other specialists enhance the implementation
8. **Integration**: The Orchestrator ensures all components work together properly
9. **Deployment**: DevOps Engineer handles deployment and infrastructure needs

This workflow creates a seamless development process where each specialist contributes their expertise while the Orchestrator maintains the overall coordination.

## Usage Guidelines

### Mode Selection

Choose the appropriate mode based on the specific development task:

- For initial project planning and delegation, use **Orchestrator**
- For architectural design and technology selection, use **System Architect**
- For user interface design and usability, use **UI/UX Designer**
- For client-side implementation, use **Frontend Developer**
- For server-side implementation, use **Backend Developer**
- For data modeling and storage, use **Database Expert**
- For deployment and infrastructure setup, use **DevOps Engineer**
- For diagnosing and fixing bugs, use **Code Debugger**
- For improving existing code quality, use **Code Refactorer**
- For version control strategy and operations, use **Git Manager**
- For optimizing application performance, use **Performance Optimizer**
- For evaluating code quality and correctness, use **Code Reviewer**

### Cross-Mode Collaboration

The power of Roo-Code comes from the collaboration between specialized modes. For complex projects requiring multiple areas of expertise, the recommended workflow is:

1. Begin with **Orchestrator** to analyze requirements and break down into smaller subtasks
2. Use **System Architect** to establish the technical foundation
3. Proceed with specialized modes based on the project's specific needs
4. After each implementation task, use **Code Reviewer** to verify quality and correctness
5. If issues are found, return to the appropriate specialist for corrections
6. Return to **Orchestrator** to integrate the work of different specialists

### Mode Files Format

Each mode file follows a consistent structure:

```markdown
# Mode Name

**Role:**
Description of the specialist's role and primary responsibilities.

**Custom Instructions:**
Detailed guidelines for how the specialist should approach tasks, organized in numbered sections.
```

The custom instructions are tailored to each specific role, providing detailed methodologies, best practices, and step-by-step processes for accomplishing domain-specific tasks effectively.

## VSCode Integration

The Roo-Code extension integrates these specialized modes directly into your VSCode environment:

- **Mode Switching**: Easily switch between different specialist modes based on your current task
- **Context Awareness**: Each mode understands the project context and previous work done by other modes
- **Documentation Integration**: All documentation is stored in the project's "plan" folder for easy reference
- **Seamless Handoffs**: Work smoothly transitions between specialists through the Orchestrator's coordination

## Tool Usage Strategy

All Roo-Code modes follow a consistent approach to file operations within VSCode:

1. For editing existing files (in priority order):
   - `apply_diff` for precise, surgical changes
   - `search_and_replace` for pattern-based updates
   - `insert_content` for adding new sections
   - `write_to_file` only as last resort for editing
2. For creating new files, always use `write_to_file`

## Package Manager Standards

To ensure consistency and leverage optimized tooling across the project, all specialized modes adhere to the following package manager standards:

- **JavaScript/TypeScript**: **Bun** must be used exclusively for package management, script execution, and runtime.
- **Python**: **Poetry** must be used exclusively for dependency management and virtual environments.
- **Go**: **Go modules** must be used exclusively for dependency management.
- **Rust**: **Cargo** must be used exclusively for builds and dependency management.

These standards are strictly enforced in development workflows, CI/CD pipelines, and any code modifications made by the specialist modes.


## Extending the Roo-Code Modes

To add new specialized modes to the Roo-Code extension:

1. Create a new file named `[number]-[mode-name].md`
2. Follow the established format with **Role** and **Custom Instructions** sections
3. Ensure the mode provides specialized expertise distinct from existing modes
4. Update this README to include the new mode

## Temperature Settings

Different modes benefit from different temperature settings based on the creativity required for their tasks. Here are the recommended temperature settings:

### Temperature 1.0 (High Creativity)
These roles benefit from higher creativity as they involve conceptual design, strategic thinking, and innovative problem-solving:

- **System Architect (1.0)**: Requires creative thinking to design scalable architectures and make strategic technology choices that balance various constraints.
- **UI/UX Designer (1.0)**: Needs high creativity to design intuitive, aesthetically pleasing interfaces and innovative user experiences.

### Temperature 0.5 (Balanced Approach)
These roles need a balance between creativity and adherence to standards:

- **Orchestrator (0.5)**: Needs balanced creativity for task breakdown while following structured workflows and coordination patterns.
- **DevOps Engineer (0.5)**: Requires some creativity for infrastructure design but must follow established practices for reliability.
- **Database Expert (0.5)**: Needs creativity for data modeling but must adhere to normalization principles and performance best practices.
- **Performance Optimizer (0.5)**: Benefits from creative problem-solving while following established optimization techniques.
- **Git Manager (0.5)**: Needs some creativity for workflow design while adhering to version control best practices.
- **Code Refactorer (0.5)**: Requires creativity to identify better code structures while maintaining existing functionality.

### Temperature 0 (Strict Adherence)
These roles require strict adherence to specifications, standards, and existing patterns:

- **Frontend Developer (0)**: Should strictly implement designs according to specifications with minimal creative deviation.
- **Backend Developer (0)**: Needs to follow API contracts and business logic specifications precisely.
- **Code Debugger (0)**: Must methodically follow debugging protocols to identify and fix issues without creative interpretation.
- **Code Reviewer (0)**: Should strictly evaluate code against established standards and requirements without creative interpretation.

### Rationale

- **High Temperature (1.0)** works best for roles that define "what" should be built and "why," where exploring multiple approaches leads to better outcomes.
- **Medium Temperature (0.5)** is ideal for roles that balance established practices with situation-specific solutions.
- **Low Temperature (0)** is best for roles focused on implementing predefined specifications where consistency and predictability are paramount.