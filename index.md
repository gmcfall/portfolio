## [react-firebase-state](https://github.com/gmcfall/react-firebase-state)
A state management library for Firebase in React apps. This library helps
you manage server-side data from *Firebase Auth* and *Firestore*, plus
client-side state that you control.

React, Redux, and Firebase had been my preferred front-end stack for years.
But the combination of Firebase with Redux has some pain points. Compared 
to other frameworks, it requires more effort to implement new features, 
even when streamlined with Redux-Toolkit.  Furthermore, the typical design
pattern involves calling `useEffect` to fetch data when a component mounts.
This pattern runs afoul of the React roadmap. Future releases of React will, 
under certain circumstances, unmount and remount components in quick succession. 
This impending design change will cause lots of unnecessary data fetching at 
great expense for components that load data from inside the `useEffect` hook.

I considered switching from Redux to React-Query (now renamed *TanStack Query*).
But it's not a great fit because TanStack Query's sweet spot is pulling data 
from the server, not receiving data pushed from the server as Firestore does 
when using listeners. In the end, I decided to build a state management library 
from the ground-up tailored to Firebase's unique features.

## [yjs-firestore-provider](https://github.com/gmcfall/yjs-firestore-provider)
It is notoriously difficult to build collaborative applications like Google Docs 
where various users make concurrent changes to the same rich-text document or 
some other complex data structure.

[Yjs](https://docs.yjs.dev/) is a library of modular building blocks that 
simplifies the development of such collaborative applications. It includes a 
variety of *providers* that set up the communication between clients, manage
awareness information, and store shared data. Unfortunately, Yjs does not
include a provider that uses Google Firestore as the backend.

The `yjs-firestore-provider` module fills that gap.

## [flashcards](https://github.com/gmcfall/flashcards)

A reference application illustrating the use of `react-firebase-state` and 
`yjs-firestore-provider`.

The application allows students and teachers to create and share smart flashcards.

This application is a work-in-progress.

### Features:
- Robust User Management including workflows for registration, sign in, sign out, 
  updating a user profile, and deleting a user account.
- Search for existing flashcard decks.
- An editor for concurrent editing of flashcard decks by multiple collaborators.
- A personal library of favorite decks.
- A sharing workflow similar to Google Docs.

## [Konig Semantic Toolkit](https://github.com/konigio)

A suite of tools for creating applications that leverage semantic web standards.

As a Principal Architect at Pearson Education, I designed these tools and led
a team of software engineers who did most of the coding, though I made contributions 
to the code base, too. Pearson was generous enough to release these 
tools to the open source community.

The main thrust of this project was to build low-code (and even no-code) solutions for
ETL into a data warehouse.

## [Learning Tools Interoperability (LTI)](https://www.imsglobal.org/activity/learning-tools-interoperability)

I served as the co-chair of a working group that developed an international standard for linking
together cross-domain learning tools, under the auspices of the IMS Global Learning Consortium 
(now rebranded as *1EdTech*).

As of March 2023, there are 176 learning tools that leverage this standard, benefitting millions 
of instructors and students.


