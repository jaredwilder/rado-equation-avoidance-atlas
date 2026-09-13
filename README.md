# Rado Equation Avoidance Atlas

**Author:** Jared Wilder  
**Public subject home created:** 2026-09-13

This repository is the focused home for a finite exact-extremal program that was previously buried inside the mixed `relation-family-atlas` release.

## Problem family

For integers `a,b,c` and `n >= 1`, let

\[
f(a,b,c;n)
\]

denote the maximum cardinality of a subset of `[n]={1,...,n}` containing **no solution in distinct elements** `x,y,z` to

\[
ax+by=cz.
\]

The distinctness convention is load-bearing. This repository must not silently mix it with Schur-style variants that permit repeated variables.

## Recovered exact atlas

The source sweep reports an exact atlas consisting of:

- **11 complete solver-optimal sequences**;
- **839 exact values** in total;
- **10 of the 11 sequences reported absent from OEIS** at the time of the sweep;
- six of seven sampled tables independently re-derived by brute force on `n=3..20`;
- the seventh sample being Schur's equation under the separate convention permitting `x=y`, giving `ceil(n/2)`.

Those are source-reported audit facts. The original machine-readable 839-value atlas has **not yet been recovered into this repository**, so this front door does not pretend the full table bytes are present.

## Concrete recovered lines

### `x + 2y = 3z`

The source records a solver-optimal sequence through `n=63`, beginning

```text
3,3,3,4,4,4,5,6,7,7,7,7,7,8,9,9,9,9,9,10,...,19
```

The public mixed-source summary abbreviates the middle of this sequence. Until the original table bytes are recovered, this repository will not manufacture the omitted entries.

### `x + 3y = 4z`

The source reports the exact plateau

\[
f(1,3,4;n)=20\qquad(46\le n\le64),
\]

followed by

\[
f(1,3,4;65)=21.
\]

The associated construction is described as periodic with residue pattern

```text
{0,1,3,5,6} mod 13
```

and the source identifies a finite-reach mechanism behind the 19-value plateau.

A preregistered generalization from that mechanism did **not** survive measurement: the predicted rule for `x+4y=5z` missed, with the measured plateau value reported as 20 rather than 12. That failed prediction is part of the research record and is preserved rather than erased.

## What this repository claims

This is an **exact finite-computation / extremal-sequence research program**, not a claim of a new general theorem in Rado theory.

The source itself describes these results as new exact values in a natural specialization of a classical framework, and explicitly warns that structural constructions may have classical antecedents. Historical novelty/priority is therefore **not upgraded here** merely because the numbers were absent from the source's OEIS check.

## Authority boundary

Current static authority in this repository is:

1. the mathematical definition and conventions above;
2. the recovered audit statements copied from the public source summary;
3. explicit publication/recovery debt below.

Not yet present here:

- the complete 839-value machine-readable atlas;
- the full 11 sequence tables;
- solver certificates/receipts for every row;
- a fresh literature/OEIS collision audit performed from this repository.

Those are recovery tasks, not license to interpolate missing data.

## Provenance

Primary public source before promotion:

- `jaredwilder/relation-family-atlas`
- README section **"Exact values that survive the collision"**

The mixed source remains valuable provenance, but this focused repository is now the canonical public subject home for the Rado-equation avoidance atlas.

## Status

**PROGRAM PUBLIC / FULL DATA RECOVERY INCOMPLETE.**

The exact finite results reported above are preserved with their original scope. Missing source bytes are named explicitly instead of reconstructed from guesswork.
