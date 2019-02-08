# Intermediate proofs

## Or condition proof 

```hs
Premises:
 (A | B) & C
 B -> C

Conclusion : B | C

----------------
1.  (A | B) & C      -- Premise
3.  B -> C           -- Premise
4.  A | B            -- 1.&E
5.  C                -- 1.&E
    ___
6.   A               -- Supp
7.   B | C           -- 5.|I
    ___
8.   B               -- Supp
9.   B | C           -- 8.|I
    ___
10. B | C            -- 6-7,8-9,CP
```
