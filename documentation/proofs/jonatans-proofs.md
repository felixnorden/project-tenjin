# 3+1 propositional statements and their proofs

## 1. Simple: Implies elimination

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

## 2. Intermediate: Or elimination 

```hs
Premises:
 A
 (A & C) | C

Conclusion: C

---------------
1. A            -- Premise
2. (A & C) | C  -- Premise
___
3. C            -- Assumption
___
___
4. (A & C)      -- Assumption
5. C            -- &E(1, 4)
___
6. C            -- |E(3, 4-5)
```

## 3. Advanced: Conjuction of disjunctions

```hs
Premises:
 (A & ~B) 
 (D | (D & C))
 D -> C
 ~B -> (A | C)
 

Conclusion: 
 (A | C) & (D & C) 

---------------
1. (A & ~B)           -- Premise
2. (D | (D & C))      -- Premise
3. D -> C             -- Premise
4. ~B -> (A | C)      -- Premise
5. ~B                 -- &E(1)
6. (A | C)            -- ->E(4)
___
7. D                  -- Assumption
8. C                  -- ->E(3, 7)
9. (D & C)            -- &I(7, 8)
___
10. (D & C)           -- Assumption
___
11. (D & C)           -- |E(7-9, 10)
12. (A | C) & (D & C) -- &I(6, 11)

```

## Bonus: Contradiction

```hs
Premises:
 A | B
 A -> ~C

Conclusion : 
 C -> B

---------------
1. A | B         -- Premise
2. A -> ~C       -- Premise
___
3. C             -- Assumption
   ___
   4. A             -- Assumption
   5. ~C            -- ->E, (2, 4)
   6. ⊥             -- (3, 5)
   7. B             -- ⊥E(6, B)
   ___
   8. B             -- Assumption
   ___
9. B              -- |E(4-7, 8)
___
10. C -> B        -- ->I(3-9)
