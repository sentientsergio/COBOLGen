# COBOLGen Benchmark Pilot

## Overview

![Corpus Callosum](./banner.png)

The **COBOLGen Benchmark Pilot** aims to develop synthetic COBOL datasets that benchmark the performance of large language models (LLMs) in translating COBOL programs to modern environments like Java or .NET. The project seeks to address the challenges posed by a scarcity of complex, diverse, and high-quality COBOL datasets by creating comprehensive synthetic examples that fully represent the nuances and complexities of real-world COBOL systems.

The project leverages **Autogen**, a Python-based Agentic AI framework, and **Retrieval-Augmented Generation (RAG)**, combining autonomous AI-driven generation with context-rich guidance to create realistic COBOL code and projects. These synthetic datasets will be used for benchmarking LLM tools in terms of their translation accuracy and efficiency.

This README provides a high-level description of the project and links to the core documents that have been developed so far.

## Documents

### 1. [Project Inception - COBOLGen Benchmark Pilot](./inception.md)

This document details the initial project vision, including:

- The motivation behind developing synthetic COBOL datasets.
- A problem statement that addresses the limitations of current COBOL data resources.
- The high-level objectives of creating a benchmarking dataset for evaluating LLM translation tools.

### 2. [Literature Review - Techniques for Synthetic Data Generation and COBOL Translation](./research.md)

This literature review explores:

- Techniques for generating synthetic data and how they can be used for COBOL translation.
- The use of Agentic AI and RAG to generate and enhance COBOL data.
- Related works in legacy language translation and the role of synthetic data in benchmarking.

### 3. [COBOLGen Benchmark Pilot Architecture Document](./architecture.md)

This architecture document provides a comprehensive overview of the system design and technology stack for the COBOLGen Benchmark Pilot. It covers:

- Key architectural components, including the Autogen framework, Retrieval-Augmented Generation (RAG), and cloud-based infrastructure.
- The integration of large language models (LLMs) and how they support the project's objectives.
- Details on the development environment, tools, and technologies used to facilitate agile development and rapid iteration.
- Architectural workflows and data flow diagrams that illustrate system interactions and processes.

### 4. [COBOLGen Benchmark Pilot Agile Planning Document](./plans/agile.md)

This agile planning document outlines the iterative approach for implementing the COBOLGen Benchmark Pilot. It covers:

- Sprint cycles, starting from project kickoff and setup to continuous improvement and feedback integration.
- Details on setting up development environments, creating a GitHub repository, collaborating with COBOL experts, and building the synthetic COBOL datasets.
- Sprints include initial setup, Autogen agent development, LLM integration, RAG implementation, and MVP release.
- Each sprint focuses on delivering a potentially shippable product increment, with regular reviews and retrospectives to adapt and refine the process.

## Key Technologies

- **Autogen**: The agentic AI framework responsible for autonomous decision-making and generation of COBOL projects, helping simulate real-world complexity.
- **Reflection**: Agents reflecting on intermediate results, providing feedback for iterative improvement to ensure high-quality output and alignment with business requirements.
- **Retrieval-Augmented Generation (RAG)**: Enhances the generation process with context from existing COBOL codebases, manuals, and domain-specific knowledge.
- **OpenAI o1-preview**: Used for generating and managing agent-based tasks effectively in synthetic data generation.
- **GPT-4o**: Provides the backbone for complex language generation tasks, helping create realistic COBOL code samples.
- **Anthropic Claude GPT 3.5**: Assists in understanding and refining generated COBOL data, ensuring semantic correctness and enhanced translation quality.

## Next Steps

- Finalize the proof of concept (POC) for generating synthetic COBOL-translation pairs.
- Continue refining the Autogen and RAG configurations to enhance the quality of generated datasets.
- Collaborate with stakeholders to iteratively improve the generated code based on real-world feedback.

## How to Contribute

If you’re interested in contributing to this project, please review the existing documents (linked above) and provide suggestions, code contributions, or feedback. All contributions are welcome, particularly in the areas of expanding dataset diversity, improving generation accuracy, and extending benchmarking coverage.
