# Advanced proofs

## Or elimination and Or-And conclusion

```hs
Premises:
 (A | B) -> C
 C -> B
 D | A
 D & B

Conclusion: (C | A) & B

------------------------
1. (A | B) -> C       -- Premise
2. C -> B             -- Premise
3. D | A              -- Premise
4. D & B              -- Premise
5. D                  -- 4.&E
6. B                  -- 4.&E
   ___
7.  A                 -- Supp
8.  C | A             -- 7.|I
9.  (C | A) & B       -- 8,6.&I
   ___
   ___
10. ~A                -- Supp
11. A | B             -- 6.|I
12. C                 -- 11,1.MP
13. C | A             -- 12.|I
14. (C | A) & B       -- 13,6.&I
   ___
15. (C | A) & B       -- 7-9,10-14.CP 
``` 

## Conjuction of a disjunction and a conjunction

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

## Assumption contradiction

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
