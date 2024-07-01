# AI-Arena-Audit
https://hackmd.io/@dO4PKW54RVa8wuwmVLvKWQ/BJ-RM0JPA

```uint256 newDna = fighterType == 0 ? dna : uint256(fighterType);```

`newDna` being directly set to the fighterType when `fighterType != 0 `might lead to confusion and misuse. `newDna` is typically expected to be a derived large number or unique identifier based on complex calculations, not a small constant value.

An attacker might exploit the predictable nature of newDna by setting fighterType to non-zero value.
