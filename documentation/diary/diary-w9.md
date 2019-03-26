# Diary Week 9

## Work tasks

- Continue on implementation of iteration one's C# module.
- Create the paper prototype.
- Design the user test

### Finished tasks

- Create the paper prototype.
- Design the user test

### Unfinished tasks

- Continue on implementation of iteration one's C# module.

## Problems

- Some development problems have occurred, e.g. we do check the lists of clauses of a proof unnecessarily at times. It would be preferable if we could avoid this without needing the information of where the clause to modify was chosen.

### Suggested solutions (with reflections)

- One possible solution is to merge the two lists `Premises` and `Conclusions` into one single list, where we keep track of where the turnstile (⊢) is positioned. This way, we always iterate over the same list.

#### Solution (if chosen)

- We have decided to only go with the suggested solution if we see that the code base becomes too complex with the current solution after some refactoring.

## Meetings

- [Meeting March 22, 2019](../meetings/meeting-22-03-19.md)
