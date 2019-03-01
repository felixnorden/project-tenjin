# Supervision

Date: 30-01-19

## Topics brought up

- Have some form of abstraction for the logic and proofing to always make sure that the proof holds or not, without annoying parsing
- Alternative visualisation of the game should be discussed further
- Linear logic - every proposition can only be used once
  - Has duplication using the `!`-modality to say what can be copied, and what cannot
  - `!` can only be eliminated, never introduced!
- Constructive logic - splitting conclusions into separate proofs for each algebraic clause
- Classical logic - also has negation
- Sequent Calculus vs Natural Deduction
  - Simply different syntax
  - **Note:** Cut rule in Sequent Calculus
- Focus on Propositional logic
- Points depending on how fast/efficiently the proofs are made
  - Deducted points for slower
- Meetings weekly to begin with
- Project goals
  - Formulate a thesis based on Computer Science
    - I.e based on model to product
    - E.g can we produce an intuitive visualisation?

### Constructive logic

Building up a proof along the way

- "Law of excluding middles" - Either A or ¬A
- ¬A = A → ⊥
- "False" implies anything, so anything goes from false assumptions

E.g

> A = A → ⊥
> ¬A
> –––
> C

⟶

> ⊥
> –––
> C

⟶

> C
> –––
> C
