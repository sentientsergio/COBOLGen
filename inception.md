# Project Inception: Generating Synthetic Test Data for Benchmarking LLM Translation Performance

## 1. Project Overview

The aim of this project is to develop synthetic test data for benchmarking the performance of tools attempting to translate COBOL programs into modern language environments like Java or .NET. Given the critical role COBOL still plays in legacy systems, especially in finance and government sectors, translating COBOL code accurately and effectively is essential to modernizing IT infrastructure. Synthetic data generation will provide a variety of scenarios, edge cases, and nuanced patterns that real-world COBOL code often presents, offering a robust foundation for evaluating the performance of translation tools.

This project will leverage **Autogen**, a Python-based Agentic AI framework, to generate synthetic COBOL data, bypassing traditional grammar-based generation approaches. Autogen allows for the autonomous exploration and generation of COBOL programs with different levels of complexity, more closely simulating real-world problem-solving and intricate business logic scenarios. At inception, this synthetic COBOL data generation tool could be informed using **Retrieval-Augmented Generation (RAG)**, which would allow it to incorporate COBOL syntax and semantics comprehensively. This enables the tool to exercise all language features for completeness during generation. Additionally, the generated code will not only consist of individual COBOL sources but also projects comprising multiple COBOL sources and copybooks. The agent teams will receive initial input from human experts in the form of business requirements and specific COBOL features to be exercised. This input, provided in machine-readable formats like **JSON** or **YAML**, will guide the planning, design, and development of sources that fit cohesively into the planned project structure.

## 2. Problem Statement

COBOL remains one of the most pervasive programming languages for critical business systems, yet there is a shortage of skilled COBOL programmers, and the language itself is cumbersome for modern software development. Converting COBOL to modern programming languages manually is time-intensive, error-prone, and costly. While LLMs offer a promising solution for automating this translation, a significant challenge is the lack of diverse, complex, and annotated COBOL datasets for benchmarking these tools. Most publicly available test programs are small and simple, which limits the effectiveness of benchmarking efforts. This project aims to generate more complex examples that exercise a broader range of COBOL language features and involve greater complexity than the tiny publicly available library of examples provides.

## 3. Objectives

- Develop an automated pipeline leveraging Autogen to synthesize (generate) diverse COBOL code samples, including a range of business logic patterns.
- Use Retrieval-Augmented Generation (RAG) to inform the synthetic generation tool with COBOL syntax and semantics, ensuring completeness in exercising all language features.
- Develop COBOL projects consisting of multiple interrelated COBOL sources and copybooks, ensuring a comprehensive representation of realistic enterprise systems.
- Provide initial project requirements and specific COBOL features from human experts in machine-readable formats, guiding the generation of synthetic projects.
- Ensure the synthetic data covers typical COBOL application use cases and edge cases, enabling the synthetic programs to comprehensively benchmark translation performance of LLM tools being used to translate COBOL.

## 4. Key Considerations

- **Diversity in COBOL Code**: COBOL has numerous variations, including differences in syntax, structure, and style influenced by decades of practices. The synthetic data generation needs to incorporate these diverse aspects.
- **Complex Business Logic**: Real-world COBOL programs often include complex business logic for financial transactions, error handling, and system integration. The generated test data must mirror these characteristics.
- **Project-Level Complexity**: COBOL applications often consist of multiple programs and shared components, such as copybooks. The generated projects must reflect this level of complexity, ensuring the code samples are representative of typical enterprise COBOL systems.
- **Human-Guided Input**: Business requirements and specific features will be provided by experts and former COBOL programmers, ensuring that generated projects align with real-world scenarios and objectives.
- **Data Integrity and Annotation**: To effectively benchmark translation tools, synthetic datasets must be well-annotated, reflecting correct and incorrect translations, ensuring the tools can be rigorously evaluated for logic preservation and error avoidance.

## 5. Approach and Methodology

- **Data Generation Using Autogen**: Utilize Autogen, a Python-based agentic AI framework, to autonomously generate COBOL projects representing different business cases—ranging from simple payroll processes to complex insurance claim workflows. This approach moves away from grammar-based techniques and leverages LLMs to simulate realistic and intricate scenarios.
- **Retrieval-Augmented Generation (RAG)**: Leverage RAG to integrate COBOL syntax and semantics into the generation process, ensuring a thorough understanding and representation of language features. This approach will enhance the completeness and accuracy of the generated COBOL programs.
- **Input from Human Experts**: The process will start with input from human experts, including business requirements and specific COBOL features, provided in machine-readable formats (e.g., JSON/YAML). This guidance ensures that generated projects accurately reflect business needs.
- **Project-Level Synthesis**: Develop cohesive projects involving multiple COBOL sources and copybooks, ensuring they fit together to form realistic business applications. This will include planning, designing, and developing components that are interdependent.
- **Synthetic Code Generation**: Produce COBOL code samples of varying complexity to be used for benchmarking translation tools. The focus is on ensuring semantic correctness and clarity of logic, reflecting real-world scenarios.
- **Automated Evaluation**: Use automated testing and validation techniques to assess the quality of generated COBOL code, including unit tests to ensure correctness.
- **Benchmarking Translation Tools**: Utilize the generated datasets to benchmark the performance of various transformer-based models and tools in understanding and translating COBOL to modern languages.

## 6. Benefits

- **Scalable Data Generation**: A synthetic approach, driven by Autogen and RAG, allows the creation of vast amounts of diverse, customized data, which may not be available otherwise.
- **Accelerate Legacy Modernization**: By providing high-quality, complex benchmarking data, this project can significantly expedite legacy software modernization efforts by aiding in the development of more accurate COBOL translation tools.
- **Cost Efficiency**: Automated translation reduces reliance on the limited and often expensive pool of COBOL developers, leading to significant long-term cost savings.

## 7. Potential Challenges

- **Complexity of Business Logic**: Capturing the nuances of business-critical processes in synthetic COBOL can be challenging.
- **Generalization**: Ensuring that LLMs benchmarked on synthetic data generalize well to real-world, messy COBOL programs requires careful design and evaluation.
- **Validation**: Validating the semantic equivalence between COBOL and its translation is non-trivial, especially for complex systems.
- **Human-Agent Collaboration**: The quality of the initial human-provided requirements and specific COBOL features will be crucial for guiding the agent team effectively.

## 8. Next Steps

- Conduct a literature review to identify existing approaches to synthetic data generation for programming languages, with a focus on agentic AI techniques and RAG.
- Define specific use cases and business domains for the generated COBOL programs.
- Develop a proof of concept (POC) for generating a small set of synthetic COBOL-translation pairs using Autogen and RAG methodologies to test feasibility.
