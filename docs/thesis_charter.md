# Thesis Charter

- Version: 0.1
- Date: 2026-09-01
- Target defense: 2029-05
- Target degree: 2029-08

## 1. Central question

Can a shared latent-state model explain the complete frequency-dependent
time courses of SV/glutamate and LDCV/peptide output, and can its remaining
mechanistic alternatives be prospectively distinguished ex vivo?

## 2. Outcome-independent thesis claim

Complete transmitter time courses, rather than frequency endpoints alone,
can constrain a functional release architecture, reveal its remaining
equivalence classes, and guide a prospective ex vivo validation experiment.

## 3. Minimum thesis contribution

1. Curated in vivo dataset and observation model
2. Shared-parameter C–R–L model across stimulation conditions
3. Structural, synthetic-recovery, and practical-identifiability analyses
4. Predictive distributions for candidate ex vivo protocols
5. Pre-specified held-out ex vivo validation
6. Final supported architecture or unresolved equivalence class

## 4. Conditional mechanistic claims

### If H1 is sufficient

Under the tested conditions, SV resource depletion/recovery and an
independent calcium-dependent LDCV recruitment process are sufficient
to reproduce the measured transmitter-output crossover.

### If H2 is required

The data require an additional activity-dependent availability or
feedback state beyond depletion alone.

### If H3 is required

A presynaptic LDCV-related process reshapes SV output beyond the
changes predicted from initial release probability and depletion.

### If the models remain indistinguishable

The available data constrain an equivalence class rather than a unique
mechanism. The thesis will report which predictions remain robust and
which additional measurement would be needed.

## 5. Explicit non-claims

- C is not claimed to be measured absolute calcium concentration.
- R is an effective SV resource, not a directly counted anatomical pool.
- L is LDCV recruitment/competence, not peptide concentration or
  necessarily the number of available LDCVs.
- Fluorescence is not equated directly with release without an
  observation model.
- “Switching” does not mean that one transmitter is completely off.
- Individual microscopic parameters need not be uniquely identifiable.
- Presynaptic competition will not be inferred from peptide-receptor
  blockade.
- Optical pulses will not be assumed to equal terminal spikes unless
  input fidelity is validated.
- Results will not be generalized beyond the tested terminal,
  preparation, stimulation range, and readouts.
- Behavioral consequences, other species, other circuits, AI and
  neuromorphic applications are outside the thesis scope.

## 6. Falsification criteria

The proposed architecture fails if it cannot reproduce held-out
time-course features under a shared parameter set, or if its locked
ex vivo prediction lies outside the pre-specified acceptance criterion.

## 7. Scope-change rule

A new state variable, perturbation, readout, species, or circuit can be
added only when:

1. an existing model fails a documented diagnostic test;
2. the new component resolves that specific failure;
3. the addition does not endanger the defense timeline; and
4. the decision is recorded in the decision log.
