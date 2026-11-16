# STEM learning guide — ecosystem-orchestrator

The ecosystem orchestrator installs and coordinates the machine learning platform pieces of the AZAZAEL tree — the part that decides what runs where.

This guide is for teachers, mentors, club leaders, parents and students who want to
use this repository as a vehicle for real STEM learning — in particular for girls and
other groups still under-represented in computing, engineering and mathematics. It
says what the project actually teaches, how to run a session with it, and what to
remove so that nobody is excluded by accident.

## What this project teaches

**Subject areas**

- installation automation
- orchestration
- configuration management
- failure recovery

**Skills practised**

- writing a repeatable setup
- distinguishing configuration from code
- making a failure recoverable instead of fatal

## Prerequisites

Python 3.13. A shell. Nothing needs to be installed globally for the entry exercise, which reads configuration rather than applying it.

Nothing else is assumed for the entry-level activity below: no prior programming
experience, no particular hardware, and no home internet connection.

## Six practices this repository is set up to support

These follow the published guidance on gender-equitable STEM education — connect the
work to learners' lives, let them investigate real problems, treat struggle as part of
the work, name and challenge stereotypes, make the work collaborative, and put
learners in front of diverse role models.

1. **Connect it to their lives.** the same problem as setting up 30 identical laptops before a lesson — do it by hand once, then automate it
2. **Let them investigate.** ask learners to write the instructions they would give a classmate, then compare with what the orchestrator does
3. **Make struggle normal.** Build the session so that the first attempt is *expected*
   to fail. Say out loud that debugging is the subject, not a penalty. Ask "what did
   that error tell you?" before offering the answer.
4. **Challenge the stereotype.** Name who does this work and why it is not a gendered
   skill. Praise the method ("you isolated the variable"), not the person ("you're a
   natural") — the second kind of praise teaches learners that ability is fixed.
5. **Make it social.** groups of three split into 'write the steps', 'find the missing step', and 'test it on a clean machine'
6. **Show diverse role models.** site-reliability engineers, and the people who maintain the installers behind scientific software

## A 90-minute session

1. *(15 min)* Read the configuration and draw the target machine.
2. *(25 min)* Find one step that is not idempotent and explain the damage it could do.
3. *(35 min)* Rewrite it to be safe to run twice.
4. *(15 min)* Test on a clean copy; report what broke.

## Vocabulary to define before the session

Specialist vocabulary is a hidden entry test if nobody explains it. Define each of
these the first time it appears, in one sentence, in the learners' own words:

1. **orchestration** — deciding what runs where, and in what order.
2. **idempotent** — running it twice leaves the same result.
3. **manifest** — the file that declares the desired state.

## Accessibility

Read [ACCESSIBILITY.md](ACCESSIBILITY.md) before running a session. Two rules matter
most in a mixed-ability room:

- Every activity must be completable with a keyboard alone, with a visible focus ring.
- Every instruction names the control or the heading ("the **Run** button in the
  toolbar"), never a colour or a position.

Pair learners rather than singling anyone out, and always offer a text-only route for
a visual step.

## Contributing as a learner

Small, well-scoped contributions are the point, not a consolation prize:

- Browse issues labelled
  [`good first issue`](https://github.com/myzticalbabe/ecosystem-orchestrator/labels/good%20first%20issue).
- Read [CONTRIBUTING.md](CONTRIBUTING.md) — it has a section written for first-time
  contributors.
- Ask in [SUPPORT.md](SUPPORT.md) if anything is unclear. Asking is expected here; it
  is not a failure.

## Licence and classroom reuse

Classroom, club and workshop use is welcome. See `LICENSE` for the exact terms, and
check whether your institution requires a separate agreement before redistributing
modified copies.
