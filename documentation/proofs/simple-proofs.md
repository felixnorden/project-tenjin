# Simple proofs

## And elimination and Modus Ponens

### Natural deduction

```hs
Premises:
 A & B
 B -> C

Conclusion : C

---------------
1. A & B    -- Premise
2. B -> C   -- Premise
3. B        -- 1,&E
4. C        -- 2,3,MP
```

### Sequent calculus

``` hs
A & B, B -> C ⊢ C
->
A, B, B -> C ⊢ C    -- &L
->
A, C ⊢ C □          -- MP

```

## Implies elimination

```hs
Premises:
 A
 A -> B

Conclusion: B

---------------
1. A        -- Premise
2. A -> B   -- Premise
3. B        -- ->E(1, 2)
```