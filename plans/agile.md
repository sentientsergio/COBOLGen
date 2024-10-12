# Agile Plan for Building the MVP of COBOLGen Benchmark Pilot

## Table of Contents

1. [Introduction](#introduction)
2. [Project Goals](#project-goals)
3. [Agile Development Approach](#agile-development-approach)
4. [Sprint Overview](#sprint-overview)
   - [Sprint 0: Project Setup and Planning](#sprint-0-project-setup-and-planning)
   - [Sprint 1: Feature Matrix and Combination Engine](#sprint-1-feature-matrix-and-combination-engine)
   - [Sprint 2: Requirement Generation Engine](#sprint-2-requirement-generation-engine)
   - [Sprint 3: AI-Assisted Code Generation Module](#sprint-3-ai-assisted-code-generation-module)
   - [Sprint 4: Validation and Quality Assurance Layer](#sprint-4-validation-and-quality-assurance-layer)
   - [Sprint 5: Documentation and Metadata Generator](#sprint-5-documentation-and-metadata-generator)
   - [Sprint 6: Dataset Assembly and Initial LLM Testing](#sprint-6-dataset-assembly-and-initial-llm-testing)
5. [Roles and Responsibilities](#roles-and-responsibilities)
6. [Communication and Collaboration](#communication-and-collaboration)
7. [Tools and Technologies](#tools-and-technologies)
8. [Risk Management](#risk-management)
9. [Conclusion](#conclusion)
10. [Appendix: User Stories](#appendix-user-stories)

---

## Introduction

This agile plan outlines the step-by-step approach to develop the MVP of the **COBOLGen Benchmark Pilot**. The goal is to build a system that can generate a comprehensive library of synthetic, non-trivial COBOL programs, systematically covering all COBOL language features and mainframe capabilities.

## Project Goals

- **Systematic Feature Coverage**: Ensure that all COBOL language features and mainframe capabilities are included across the generated programs.
- **Realistic Program Generation**: Create programs that simulate real-world business logic in common application domains.
- **AI-Assisted Generation**: Utilize AI models for generating detailed requirements and COBOL code.
- **Validation and Quality Assurance**: Implement automated validation processes to ensure code correctness.
- **Scalable Architecture**: Design the system to efficiently generate large datasets suitable for LLM training.

## Agile Development Approach

- **Iteration Length**: Each sprint is two weeks long.
- **Methodology**: Agile Scrum with flexibility to adapt as needed.
- **Principles**:
  - Deliver working software frequently.
  - Welcome changing requirements.
  - Collaborate closely and communicate openly.

## Sprint Overview

### Sprint 0: Project Setup and Planning

**Duration**: 1 Week

#### Goals

- Set up development and collaboration tools.
- Finalize project scope and MVP definition.
- Prepare initial product backlog.

#### Tasks

- **Project Initialization**:
  - Set up the GitHub repository with appropriate branching strategies.
  - Configure Python development environment with `pipenv` or `poetry`.
- **Tool Configuration**:
  - Set up Notion for backlog management (Kanban board).
  - Install necessary IDE extensions (VSCode with Python and COBOL support).
- **Backlog Creation**:
  - Define user stories and acceptance criteria.
  - Prioritize user stories for upcoming sprints.
- **Meeting Schedule**:
  - Establish a schedule for stand-ups, sprint planning, reviews, and retrospectives.

#### Deliverables

- Initialized GitHub repository.
- Configured development environment.
- Populated and prioritized product backlog.
- Agreed-upon meeting schedule.

---

### Sprint 1: Feature Matrix and Combination Engine

**Duration**: Weeks 1-2

#### Sprint Goal

Develop the Feature Matrix and build the engine to generate valid feature combinations for systematic coverage.

#### User Stories

- **US01**: As a **developer**, I want to **create a comprehensive Feature Matrix**, so that **all COBOL features and mainframe capabilities are identified**.
- **US02**: As a **system**, I need to **generate valid combinations of features**, so that **we can systematically cover all scenarios**.

#### Tasks

- **Feature Matrix Development**:
  - List all COBOL language features.
  - Enumerate mainframe capabilities.
  - Identify common application domains.
- **Feature Dependency Mapping**:
  - Document dependencies and incompatibilities between features.
- **Combination Engine Development**:
  - Write a Python script to generate valid feature combinations.
  - Implement constraints to avoid invalid combinations.
- **Documentation**:
  - Document the Feature Matrix and combination logic.

#### Deliverables

- Completed Feature Matrix with dependencies mapped.
- Working Feature Combination Engine script.
- Documentation on Feature Matrix and combination process.

---

### Sprint 2: Requirement Generation Engine

**Duration**: Weeks 3-4

#### Sprint Goal

Develop the Requirement Generation Engine that creates detailed requirement specifications based on feature combinations.

#### User Stories

- **US03**: As a **developer**, I want to **generate requirement templates**, so that **we can standardize requirement specifications**.
- **US04**: As a **system**, I need to **automate requirement generation using AI**, so that **requirements are realistic and detailed**.

#### Tasks

- **Template Design**:
  - Create requirement specification templates with placeholders for features.
- **Prompt Engineering**:
  - Develop prompts for AI models to generate enriched requirements.
- **Requirement Generation Script**:
  - Implement a script to automate the generation of requirements using the templates and prompts.
- **Integration with AI Models**:
  - Set up API access to AI models (e.g., OpenAI GPT-4).
  - Handle API key management securely.
- **Testing and Validation**:
  - Generate sample requirements and validate their quality.
- **Documentation**:
  - Document the requirement generation process and how to adjust templates and prompts.

#### Deliverables

- Requirement specification templates.
- Requirement Generation Engine script.
- Sample generated requirements.
- Documentation on the requirement generation process.

---

### Sprint 3: AI-Assisted Code Generation Module

**Duration**: Weeks 5-6

#### Sprint Goal

Develop the module that uses AI models to generate COBOL code based on detailed requirements.

#### User Stories

- **US05**: As a **system**, I need to **generate COBOL code using AI**, so that **the code includes specified features and business logic**.
- **US06**: As a **developer**, I want to **ensure code is syntactically correct**, so that **it can be compiled and tested**.

#### Tasks

- **Integration with AI Models**:
  - Set up API calls to generate COBOL code from requirements.
- **Prompt Refinement**:
  - Optimize prompts to guide the AI in generating accurate code.
- **Code Generation Script**:
  - Implement a script to automate code generation for each requirement.
- **Initial Validation**:
  - Compile generated COBOL code using a COBOL compiler (e.g., GnuCOBOL).
  - Fix any syntax errors by adjusting prompts or post-processing code.
- **Testing on Sample Requirements**:
  - Generate code for a subset of requirements and validate results.
- **Documentation**:
  - Document the code generation process and prompt guidelines.

#### Deliverables

- AI-Assisted Code Generation Module script.
- Sample generated COBOL programs.
- Documentation on code generation and prompt engineering.

---

### Sprint 4: Validation and Quality Assurance Layer

**Duration**: Weeks 7-8

#### Sprint Goal

Implement automated validation processes to ensure syntactic and functional correctness of the generated COBOL code.

#### User Stories

- **US07**: As a **QA engineer**, I want to **automate syntactic validation**, so that **we can quickly identify and fix code issues**.
- **US08**: As a **developer**, I need to **implement functional testing**, so that **the code performs as intended**.

#### Tasks

- **Automated Syntactic Validation**:
  - Develop scripts to batch compile COBOL programs and log errors.
- **Functional Testing Framework**:
  - Design a testing framework for executing programs with test data.
  - Create test data sets for sample programs.
- **Error Handling and Reporting**:
  - Implement mechanisms to capture and report compilation and execution errors.
- **Human-in-the-Loop Review**:
  - Set up a process for manual review of a subset of programs.
- **Continuous Integration Setup**:
  - Configure CI tools (e.g., GitHub Actions) to automate validation on code updates.
- **Documentation**:
  - Document the validation processes and how to interpret reports.

#### Deliverables

- Validation scripts and tools.
- Functional testing framework with sample test cases.
- CI pipeline configured for automated validation.
- Documentation on validation procedures.

---

### Sprint 5: Documentation and Metadata Generator

**Duration**: Weeks 9-10

#### Sprint Goal

Develop tools to generate documentation and metadata for each program, detailing included features and usage instructions.

#### User Stories

- **US09**: As a **user**, I want **detailed metadata for each program**, so that **I understand what features are included**.
- **US10**: As a **developer**, I need to **automate documentation generation**, so that **it's consistent and up-to-date**.

#### Tasks

- **Metadata Schema Design**:
  - Define the structure of metadata for programs (e.g., features included, dependencies, instructions).
- **Documentation Templates**:
  - Create templates for program documentation.
- **Automation Scripts**:
  - Implement scripts to generate metadata and documentation based on the feature combinations and requirements.
- **Code Annotation**:
  - Insert comments or annotations within the code to highlight features.
- **Testing and Verification**:
  - Generate documentation for sample programs and verify accuracy.
- **Documentation**:
  - Document the metadata generation process and how to customize it.

#### Deliverables

- Metadata schema and documentation templates.
- Documentation and Metadata Generator scripts.
- Sample documentation and metadata files.
- Documentation on the generation process.

---

### Sprint 6: Dataset Assembly and Initial LLM Testing

**Duration**: Weeks 11-12

#### Sprint Goal

Assemble the generated programs and documentation into a structured dataset and perform initial testing with LLMs.

#### User Stories

- **US11**: As a **data scientist**, I want to **use the dataset for LLM training**, so that **I can evaluate model performance**.
- **US12**: As a **project manager**, I need to **ensure the dataset is well-organized**, so that **it's easily usable by others**.

#### Tasks

- **Dataset Structuring**:
  - Organize programs, metadata, and documentation into a coherent directory structure.
- **Data Packaging**:
  - Prepare the dataset for distribution (e.g., zipping files, creating manifests).
- **Initial LLM Training**:
  - Use the dataset to train or fine-tune an LLM for COBOL translation.
- **Performance Evaluation**:
  - Evaluate the LLM's performance on translating the generated programs.
  - Identify any issues or areas for improvement.
- **Feedback Incorporation**:
  - Use insights to refine generation processes or prompts.
- **Documentation**:
  - Document the dataset contents and usage instructions.

#### Deliverables

- Assembled dataset ready for use.
- Initial LLM performance report.
- Documentation on dataset structure and usage.

---

## Roles and Responsibilities

- **Product Owner**: Defines the vision, prioritizes the backlog, and accepts deliverables.
- **Scrum Master**: Facilitates the agile process, removes impediments, and ensures the team adheres to Scrum practices.
- **Development Team**: Responsible for implementing the tasks, including developers, QA engineers, and data scientists.
- **AI Specialist**: Focuses on AI model integration and prompt engineering.
- **Quality Assurance**: Ensures the quality of the generated code and documentation.

_(Note: Since you're working as a solopreneur, these roles may be combined or adjusted as needed.)_

## Communication and Collaboration

- **Daily Check-ins**: Personal review of progress and planning for the day.
- **Sprint Planning Meetings**: At the start of each sprint to define goals and tasks.
- **Sprint Reviews**: At the end of each sprint to assess achievements.
- **Sprint Retrospectives**: Reflect on what went well and what can be improved.
- **Tools**:
  - **Notion**: For backlog management and documentation.
  - **GitHub**: For version control and issue tracking.
  - **VSCode**: As the primary development environment.

## Tools and Technologies

- **Programming Languages**: Python for scripting and automation.
- **AI Models**: OpenAI GPT-4 for requirement and code generation.
- **COBOL Tools**: GnuCOBOL compiler for validation.
- **Testing Frameworks**: Custom scripts or pytest for validation processes.
- **Documentation Tools**: Markdown, Sphinx or MkDocs for generating documentation.
- **Version Control**: Git and GitHub for code management.
- **CI/CD**: GitHub Actions for continuous integration.

## Risk Management

- **Technical Risks**:
  - **AI Model Limitations**: Mitigate by refining prompts and providing more context.
  - **Validation Challenges**: Address by improving testing frameworks.
- **Resource Risks**:
  - **API Usage Limits**: Monitor usage and plan for potential costs.
  - **Time Constraints**: Prioritize tasks and adjust scope as needed.
- **Quality Risks**:
  - **Code Quality**: Implement thorough validation and testing.
  - **Dataset Utility**: Gather feedback from initial LLM testing to improve.

## Conclusion

This agile plan provides a roadmap for developing the MVP of the **COBOLGen Benchmark Pilot**. By focusing on iterative development and continuous improvement, we aim to build a robust system that meets the project's goals and provides valuable datasets for LLM training and testing.

---

## Appendix: User Stories

- **US01**: Create a comprehensive Feature Matrix.
- **US02**: Generate valid combinations of features.
- **US03**: Generate requirement templates.
- **US04**: Automate requirement generation using AI.
- **US05**: Generate COBOL code using AI.
- **US06**: Ensure generated code is syntactically correct.
- **US07**: Automate syntactic validation.
- **US08**: Implement functional testing.
- **US09**: Provide detailed metadata for each program.
- **US10**: Automate documentation generation.
- **US11**: Use the dataset for LLM training.
- **US12**: Ensure the dataset is well-organized.
