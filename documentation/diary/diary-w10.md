# Diary Week 10

## Work tasks

This week, things went quite well and we managed to do a majority of the set out tasks. However, we did find it hard to get all of the necessary hours in due to both being a bit tired from last week's exams and our other courses having compuslory lectures and assignments.

Tasks:

- Finish the logic module for iteration one (C#).
- Update UML Class diagram for the implementation, and add necessary classes.
- Begin connecting the logic module to a Unity frontend.
- Do as many User tests as possible.
- Begin writing on report
  - Background
  - Theory
  - Method

### Finished tasks

- Finish the logic module for iteration one (C#).
- Do as many User tests as possible.
- Begin writing on report
  - Background
  - Theory
  - Method

### Unfinished tasks

- Update UML Class diagram for the implementation, and add necessary classes.
- Begin connecting the logic module to a Unity frontend.

## Problems

- The game proof structure is naturally represented by a tree that grows as new subproofs are created from the proving process. However, right now the module is represented as a list due to `C#` not having a native tree data structure. 

### Suggested solutions (with reflections)

- As things are looking right now, we have two options to go with:
  - Choose an existing third party library from nuget.
  - Create our own simplified version designed after our needs.

Choosing an existing library is useful as we save time and avoid reinventing the wheel, but it also requires us to understand the library's codebase.

Creating our own data structure could take more time, but we can tailor it to our needs and always extend it if the requirements change. It also makes it possible for us to understand the underlying code from the beginning, as we are the ones writing it.

#### Solution (if chosen)

After a bit of research on nuget, we have decided on looking at our own solution, as we could not find a recommended library that we could fully understand due to our lack of knowledge in `C#`.

## Meetings

- [Meeting March 26 2019](../meetings/meeting-26-03-19.md)
