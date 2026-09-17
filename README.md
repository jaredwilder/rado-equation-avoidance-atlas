# Rado equation avoidance atlas

For integers `a,b,c` and `n>=1`, let

\[
f(a,b,c;n)
\]

be the maximum size of a subset of `[n]={1,...,n}` containing no solution in **distinct** elements `x,y,z` to

\[
ax+by=cz.
\]

This repository collects exact finite extremal data for that problem family.

## Recovered atlas

The source audit records:

- **11 solver-optimal sequences**;
- **839 exact values** in total;
- six of seven sampled tables independently re-derived by brute force for `n=3..20`;
- 10 of the 11 sequences absent from the OEIS search performed during the original audit.

The original machine-readable 839-value table has not yet been recovered into this repository, so only the values actually present in the surviving source are displayed here.

## `x+2y=3z`

The recovered optimal sequence runs through `n=63` and begins

```text
3,3,3,4,4,4,5,6,7,7,7,7,7,8,9,9,9,9,9,10,...,19
```

The surviving summary abbreviates the middle terms; this repository does not interpolate them.

## `x+3y=4z`

The exact plateau recorded in the source is

\[
f(1,3,4;n)=20\qquad(46\le n\le64),
\]

followed by

\[
f(1,3,4;65)=21.
\]

A periodic construction uses the residue pattern

```text
{0,1,3,5,6} mod 13.
```

A proposed extension of the same mechanism to `x+4y=5z` failed: the measured plateau value was 20 rather than the predicted 12.

## Conventions matter

Repeated variables are excluded in the definition above. This differs from Schur-type formulations that allow `x=y`; those variants should not be mixed with this table.

## Data status

The mathematical definition, the concrete lines above, and the source audit are present. Still missing are the complete 839-value table and the solver certificates for every row. Those are source-recovery tasks, not gaps to fill by extrapolation.

The earlier mixed source is [`jaredwilder/relation-family-atlas`](https://github.com/jaredwilder/relation-family-atlas).

Author: Jared Wilder.
