# AI Red Teaming Guidelines and Best Practices

## Overview

This repository provides guidelines, best practices, and references for professional red teaming of generative AI systems, including large language models (LLMs), image, video, and audio generation models. The focus is on systematic, ethical, and impactful red teaming—beyond surface-level automation—drawing from leading industry and research resources.

Red teaming is not just adversarial testing or a technical exercise. As highlighted by the AVID blog, it is a critical thinking and collaborative process that challenges assumptions, governance, and organizational processes. Effective red teaming should:
- Be applied throughout the development lifecycle, not just post-deployment
- Involve both technical and non-technical stakeholders
- Foster blameless transparency about blind spots and vulnerabilities
- Include a feedback loop for tracking, prioritizing, and mitigating issues
- Require ongoing monitoring and adaptation as threats and user behaviors evolve

The GenAI Red Teaming Guide emphasizes a structured approach to identifying vulnerabilities and mitigating risks across AI systems. It highlights key risks such as prompt injection, toxic outputs, model extraction, bias, and hallucinations. The guide outlines a holistic methodology that includes model evaluation, implementation testing, infrastructure assessment, and runtime behavior analysis. It also stresses the importance of continuous monitoring and cross-functional collaboration to address evolving threats.

For further insight into the evolution and impact of AI red teaming, see [Microsoft AI Red Team: Building the future of safer AI](https://www.microsoft.com/en-us/security/blog/2023/08/07/microsoft-ai-red-team-building-future-of-safer-ai/).

## What is AI Red Teaming?

AI red teaming is the practice of systematically probing AI systems to identify vulnerabilities, risks, and failure modes. It helps organizations:
- Discover novel and emergent risks
- Stress-test mitigations and safety controls
- Improve safety metrics and risk assessments
- Build public trust in AI deployments

## The Value of Red Teaming

AI red teaming is a critical practice for ensuring the safety, security, and trustworthiness of generative AI systems. By simulating adversarial behaviors and probing for vulnerabilities, red teaming helps organizations:
- Identify and mitigate risks such as prompt injection, data leakage, and bias.
- Stress-test safety controls and alignment mechanisms.
- Build public trust by demonstrating a commitment to responsible AI practices.
- Enhance system resilience against evolving threats.

## Emerging Methods for Red Teaming

Emerging methods in AI red teaming include:
- **Adversarial Prompt Engineering**: Crafting prompts to test model robustness and alignment.
- **Scenario-Based Testing**: Simulating real-world misuse cases to uncover vulnerabilities.
- **Automated Tooling**: Leveraging tools like PyRIT for efficient risk detection and evaluation.
- **Multi-Turn Attacks**: Engaging models in conversational flows to identify weaknesses.
- **Ethical and Bias Evaluation**: Systematically testing for biases and ethical concerns in model outputs.

## Internal vs External Red Teaming

- **Internal Red Teaming**:
  - Conducted by in-house teams with deep knowledge of the system.
  - Allows for continuous testing and integration into the development lifecycle.
  - May lack the objectivity and diverse perspectives of external teams.

- **External Red Teaming**:
  - Involves third-party experts to provide an unbiased evaluation.
  - Brings diverse skill sets and fresh perspectives to the assessment.
  - Often used for high-stakes systems or regulatory compliance.

## Designing a Red Teaming Campaign or Assessment

Designing an effective red teaming campaign involves:
1. **Defining Objectives and Scope**:
   - Identify critical use cases and high-risk areas.
   - Align objectives with organizational goals and regulatory requirements.

2. **Assembling the Team**:
   - Include AI engineers, cybersecurity experts, and ethics specialists.
   - Ensure diversity in skill sets and perspectives.

3. **Threat Modeling**:
   - Analyze potential attack vectors and adversarial scenarios.
   - Use frameworks like MITRE ATLAS and NIST AI RMF for guidance.

4. **Executing the Assessment**:
   - Conduct tests across the four phases: model, implementation, system, and runtime.
   - Use a combination of manual and automated techniques.

5. **Documenting Findings**:
   - Record vulnerabilities, exploit scenarios, and remediation steps.
   - Provide actionable recommendations for improvement.

6. **Continuous Improvement**:
   - Re-test after implementing fixes and integrate periodic checks.
   - Adapt methodologies to address emerging threats and technologies.

## Red Teaming Report Structure

A professional AI red teaming report should be objective, evidence-based, and actionable. The following structure is recommended:

### 1. Executive Summary
- Key findings and severity ratings
- Overall system evaluation
- Critical recommendations

### 2. Methodology
- Testing approach and frameworks used
- Tools and techniques employed
- Testing environment and parameters
- Scope and limitations

### 3. Findings and Vulnerabilities
- Detailed description of each issue
- Severity classification (e.g., Critical, High, Medium, Low)
- Reproducibility steps
- Supporting evidence (examples, screenshots, outputs)

### 4. Risk Assessment
- Potential impact analysis
- Likelihood of exploitation
- User groups potentially affected

### 5. Recommendations
- Specific mitigation strategies
- Prioritized action items
- Long-term defense strategies

### 6. Appendices
- Raw test data
- Technical details for developers
- Testing scripts and prompts used

## Assessment Phases

The GenAI Red Teaming Guide outlines a structured approach to evaluating generative AI systems, dividing the assessment into four distinct phases:

1. **Model Evaluation**:
   - Focuses on the AI model itself, assessing its alignment, robustness, and bias.
   - Includes testing for adversarial robustness, ethical risks (e.g., bias, toxicity), and technical weaknesses (e.g., model provenance, data pipeline security).

2. **Implementation Evaluation**:
   - Examines the deployment stack, including guardrails, prompts, and filters.
   - Tests for bypassing safety controls, poisoning data used in grounding, and evaluating model firewalls or proxies.

3. **System Evaluation**:
   - Evaluates the broader system, including infrastructure, integration points, and supply chain vulnerabilities.
   - Assesses interactions between the model and other components, such as APIs and storage systems.

4. **Runtime / Human & Agentic Interaction**:
   - Focuses on real-time interactions and human-AI collaboration.
   - Identifies vulnerabilities in business processes, over-reliance on AI, and social engineering risks.

Each phase is designed to address specific risks and ensure a comprehensive evaluation of the generative AI system.

## Visual Representation

![AI Red Teaming Phases](https://www.microsoft.com/en-us/security/blog/wp-content/uploads/2023/08/Fig2-AI-red-team.webp)

This image from the Microsoft blog illustrates the structured approach to AI red teaming, emphasizing the importance of systematic evaluation across different phases.


### Concepts from GenAI Red Teaming Guide
- **Key Risks**: Prompt injection, toxic outputs, model extraction, bias, hallucinations, and data leakage.
- **Holistic Methodology**: Includes model evaluation, implementation testing, infrastructure assessment, and runtime behavior analysis.
- **Blueprint Phases**: Structured into model, implementation, system, and runtime evaluations.
- **Essential Techniques**: Adversarial prompt engineering, dataset manipulation, stress testing, and ethical bias evaluation.
- **Continuous Monitoring**: Emphasizes the need for ongoing risk assessment and adaptation to evolving threats.

### Concepts from AVID Blog
- Red teaming is a critical thinking and collaborative exercise, not just adversarial testing.
- Goes beyond technical vulnerabilities to challenge assumptions, governance, and organizational processes.
- Should be applied throughout the development lifecycle, not just post-deployment.
- Effective red teaming requires a feedback loop: tracking, prioritizing, and mitigating issues, then verifying fixes.
- Red teaming is similar to research and acceptance testing: iterative, blameless, and focused on surfacing blind spots and real-world failure modes.
- Ongoing monitoring and adaptive response are essential, as threats and user behaviors evolve after deployment.

## Key Resources

- [OWASP GenAI Red Teaming Guide](https://genai.owasp.org/resource/genai-red-teaming-guide/)
- [AI Safety Institute Red Teaming Framework (AISI)](https://aisi.go.jp/assets/pdf/ai_safety_RT_v1.00_en.pdf)
- [OpenAI’s Approach to External Red Teaming (arXiv:2503.16431)](https://www.arxiv.org/abs/2503.16431)
- [Microsoft Learn: AI Red Team](https://learn.microsoft.com/en-us/security/ai-red-team/)
- [Red Teaming is a Critical Thinking Exercise: Part 1 (AVID Blog)](https://avidml.org/blog/red-teaming-1/)
- [GenAI Red Teaming Guide (OWASP)](https://genai.owasp.org/resource/genai-red-teaming-guide/)
- [MITRE ATLAS Framework](https://atlas.mitre.org/): A comprehensive repository for adversarial threat modeling in AI systems.
- [MIT AI Risk Database](https://airisk.mit.edu/): A database for understanding and mitigating AI risks.
---

This document is a starting point. For detailed methodologies and the latest best practices, consult the resources above.
