TODO: check recommandations from previous years at OOPSLA/ECOOP/PLDI

# Advice for authors

Artifacts are self-contained packages that should contribute to making the experimental results of your paper reproducible. To that end, it is best to provide artifacts with:
- **No dependencies**. Use docker. Resort to Virtual machines otherwise (VMs are heavier, require manual installation, need user passwords and impose keyboard localization choice by default).
- **Have push-button evaluations**. We recommend to use scripts to generate data and experimental figures. This fully automated approach may be a bit more costly to setup, but you won't have any copy/pasting issue for your paper, and regenerating data is heavily simplified.

TODO: Double blind artifact evaluation is complicated...

# For authors: metadata to provide during artifact submission

## Hardware/software requirements
- OS and resource (CPU, memory, disk, GPU) used by the authors
- Required hardware resources for evaluation. In case the evaluation takes multiple days or requires huge resources, please provide a scaled-down evaluation.
- Potential compatibility issues (e.g. Docker on ARM)

TODO: How to handle exotic hardware requirements? Usenix proposes remote SSH accesses (strongly reduces anonymity)

## Description of the artefact

- Content of the artefact
- Description of the kick-the-tires test to run, and estimated running time (should be a few minutes maximum)
- List of experimental claims made by the paper, and how to reproduce each experimental claim, along with estimated running times.
- Licenses of software included in artifact.

# For reviewers: template for artefact evaluation

## Kick-the-tires

### Are there experimental claims made in the paper that are not documented in the artifact?
### Have you been able to run the artifact?
### Have you been able to run the kick-the-tires test?
### Do you expect to have sufficient resources to run the evaluation? Full or reduced if that applies?

## Functionality badge

### Are there experimental claims made in the paper that are not documented in the artifact?
### For each claim, have you been able to reproduce it? Reproduce in a smaller-scale evaluation proposed by the authors?
### Is the evaluation adequate and reliable?
Is the tool deterministic?
In particular, if execution times are measured, are there different trial runs to measure average performance? Do the execution significantly change?
### If there are comparisons with other tools, are their results reproduced as well? Are the comparisons fair?

TODO: Ask reviewers to upload produced figures/tables during their checking of the evaluation?

## Reusability badge

- Is the implementation open-source?
- Can you build the software again?
- (If relevant) Are the benchmarks used public and open-source?

# "Proof artifacts"

cf. https://proofartifacts.github.io/guidelines/
Check assumptions?


# Relevant resources:

- SIGPLAN's checklist https://www.sigplan.org/Resources/EmpiricalEvaluation/
- ACM's official page https://www.acm.org/publications/policies/artifact-review-and-badging-current
- ECOOP'23 call: https://2023.ecoop.org/track/ecoop-2023-artifacts#Call-for-Artifacts
- SPLASH'23 call: https://2023.splashcon.org/track/splash-2023-Artifacts#Call-for-Artifacts
- Other communities:
  + OSDI call for artifact: https://www.usenix.org/conference/osdi23/call-for-artifacts
  + Usenix https://www.usenix.org/conference/usenixsecurity22/artifact-appendix-guidelines
  
