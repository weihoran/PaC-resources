# Benchmark Repository: CaC-to-PaC Illustrative Examples

This repository contains an illustrative example extracted from our benchmark dataset used in our study of continuous compliance pipelines. The benchmark demonstrates the translation of Compliance as Code (CaC) into executable Policy as Code (PaC) using Large Language Models (LLMs). Please note that the full benchmark dataset is under a non-disclosure agreement (NDA) and is not publicly available. The examples here are provided solely for demonstration purposes.

## Repository Contents

- **OSCAL.json**  
  An example input file in OSCAL-compliant JSON format. This file represents a typical component definition with embedded compliance rules, parameters, and control mappings.

- **policy_template.yaml**  
  A template file for Policy as Code, formatted for Kyverno. This template includes placeholders that are intended to be dynamically filled with parameters extracted from the OSCAL input.

- **deployable_policy.yaml**  
  The reference output file, which is a fully instantiated and deployable Policy as Code. This file demonstrates the final policy generated after processing the OSCAL input with the policy template.

## Benchmark Overview

The benchmark dataset comprises 70 paired examples of CaC inputs and their corresponding PaC outputs. These pairs cover key compliance scenarios across multiple domains, including infrastructure, Kubernetes, and application-level controls. The benchmark is used to evaluate our LLM-based approach in terms of accuracy, completeness, and usability in generating executable policies.

Due to confidentiality constraints, the full dataset is not available. Instead, this repository provides a subset of synthetic examples that closely mirror the structure and complexity of the complete benchmark.

## How to Use

1. **Review the OSCAL Input:**  
   Open `OSCAL.json` to understand the structure of the compliance requirements, including rule identifiers, descriptions, parameter details, and control mappings.

2. **Examine the Policy Template:**  
   Check `policy_template.yaml` to see the layout and placeholders used for generating Policy as Code. This template serves as the basis for transforming OSCAL inputs into executable policies.

3. **Compare with the Reference Output:**  
   Open `deployable_policy.yaml` to view the final, deployable policy. This file shows how the template has been filled with actual parameter values extracted from the OSCAL input.

4. **Experiment and Extend:**  
   Use these examples as a starting point to build or test your own compliance pipelines. They can serve as a guide for how to dynamically generate policies from structured compliance inputs.

## Disclaimer

These examples are for illustrative purposes only. The full benchmark dataset, which contains more extensive and diverse examples, is under NDA and is not available in this repository.

