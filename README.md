# smart-contract-security-research
Analysis of automated smart contract security tools and their failure in cross-contract and logic-based exploits

This repository contains a practical research study on the limitations of automated smart contract security tools such as Slither and Mythril.

## Overview

Automated tools are widely used in smart contract development, but real-world exploits continue to bypass them. This research evaluates how well these tools perform across different vulnerability classes.

## What is included

- Analysis of 4 vulnerability classes:
  - Classic reentrancy
  - Cross-contract reentrancy (ERC777 / Lendf.Me)
  - Access control failures
  - Logic bugs (Nomad bridge)

- Tool evaluation:
  - Slither (static analysis)
  - Mythril (symbolic execution)

- Quantitative metrics:
  - Precision
  - Recall
  - F1 score

## Key Findings

- High precision for known vulnerability patterns
- Near-zero recall for:
  - Cross-contract interactions
  - Callback-based exploits
  - Logic-level vulnerabilities

- 100% of interaction-based and logic bugs were missed by tools in this study

## Why it matters

Modern DeFi exploits increasingly rely on complex interactions rather than isolated bugs. This makes automated tools insufficient as a standalone security solution.

## Conclusion

Security requires a layered approach:
- Static analysis
- Symbolic execution
- Manual auditing
- System-level reasoning

## Full Research

See the full report here:

👉 [research.md](./research.md)
