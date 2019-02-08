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
