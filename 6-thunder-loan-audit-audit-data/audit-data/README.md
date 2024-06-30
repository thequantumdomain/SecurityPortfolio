# Tooling

## Solidity Metrics

We can use [cloc](https://www.geeksforgeeks.org/cloc-count-number-of-lines-of-code-in-file/) or [solidity-metrics](https://marketplace.visualstudio.com/items?itemName=tintinweb.solidity-metrics) to calculate number of lines of code. 

Puppy raffle stats:
```
nSLOC: 245
Complexity: 198
```

# Static Analysis

## Slither

We can use [slither](https://github.com/crytic/slither) on this repo. 

```
slither . --config-file slither.config.json --checklist
```

This will find a number of issues by itself. 

## Coverage Report

```
forge coverage --report debug > coverage_report.txt
```

## Gas Report

```
forge snapshot
```
