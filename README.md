Advice for authors:
- Use docker when possible, resort to VMs otherwise
- Full automation to generate data & experimental figures

TODO: Double blind artifact evaluation is... complicated...

# For authors: metadata to provide during artifact submission

## Hardware/software requirements
- OS and resource (CPU, memory, disk, GPU) used by the authors
- Required hardware resources for (reduced) evaluation:
- Potential compatibility issues: (eg Docker on ARM, ...)

TODO: How to handle exotic hardware requirements? Usenix proposes remote accesses (strongly reduces anonymity)

## Description of the artefact

- Content of the artifact
- Quick kick-the-tires test
- List of experimental claims made by the paper, and how to reproduce each experimental claim
- Licenses?

# For reviewers: template for artefact evaluation

## Kick-the-tires

### Are there experimental claims made in the paper that are not documented in the artifact?
### Have you been able to run the artifact?
### Have you been able to run the kick-the-tires test?
### Do you expect to have sufficient resources to run the reduced evaluation ? Full evaluation ?

## Functionality badge

### Are there experimental claims made in the paper that are not documented in the artifact?

### For each claim, have you been able to reproduce it? Reproduce in a smaller-scale evaluation proposed by the authors?
Number of trials/summary statistics/data distribution

### If there are comparisons with other tools, are their results reproduced as well? Are the comparisons fair?

TODO: Ask reviewers to upload produced figures/tables during their checking of the evaluation?

## Reusability badge

- Is the implementation open-source?
- Can you build the software again?
- (If relevant) Are the benchmarks used public and open-source?

// - Are the benchmarks well-chosen to evaluate? Would other benchmarks be relevant?


# "Proof artifacts"

cf. https://proofartifacts.github.io/guidelines/
Check assumptions?
