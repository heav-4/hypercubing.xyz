---
title: Rules
---

# Hypercubing Leaderboard Submission Rules

These rules are not written in legalese. Please don't try to exploit them. Ask in the Hypercubers Discord if you have any questions, comments, or concerns about these rules.

These rules may be flexible, especially for new categories. For example, if you're speedsolving a really big puzzle that no one's done before, it might be reasonable to allow macros for it.

## General rules

- [These programs](/software#recommended-hypercubing-software) are recommended for speedsolving. If using a program not listed here, you should ask on the Discord first.
- The puzzle must be solved from a full scramble.
- Spectators may commentate, but must not help the solver.
- Algorithm reference sheets are strongly discouraged.[^algsheets]
- Using software to compute a solution to the puzzle state is not allowed (except for computer-assisted FMC).
- Reversing the scramble is not allowed; the solution must be novel.

## Speedsolving rules

These rules apply generally to speedsolving submissions unless the category has specific rules.

- Macros are **not** allowed.
- Piece filters are allowed.
- All speedsolves require video evidence, such as a screen recording.
    - A timer must be visible on the screen during the solve. Timers built into the puzzle software are preferred.
- If using keyboard controls:
    - If possible, a keybinds reference must be visible during the solve.[^keybinds-ref]
    - The keybinds should not be hyperoptimized for specific algorithms.[^alg-keybinds]
- Log file is not required, but you should still save your PBs!

### Blindsolving rules

- Macros are allowed during solving.
- Piece filters are allowed during memorization but not during solving.
- All blindsolves require video evidence of the solver that clearly shows the screen and that they are not cheating by using some external reference.
- The solver does not need to be blindfolded, but the colors on the puzzle must be invisible during the solve.
- Besides those rules, typical blindsolving rules apply:
    - Final time = memorization time + solving time.
    - Writing anything down isn't allowed.

### Physical rules

!!! info
    See [Canonical Moves](/puzzles/physical/2x2x2x2/canonical-moves) for more details.

- All physical solves require physical evidence that shows the puzzle fully in frame throughout the solve and shows the entire scrambling and solving process as well as the timer.
- Allowed moves for physical 2x2x2x2 events are limited to 2 categories, the canonical moveset originally made by the hypercubing mailing list as well as a few additional moves:
    - Canonical moves:
        - All R and L cell rotations
        - U/D y2
        - F/B z2
        - I/O x* (aka axial twist)
        - Any of many equivalent gyro algorithms
    - Additional moves:
        - U/D x2/z2
        - F/B x2/y2
        - I y2/z2
- Scrambles should be generated by [this page](/puzzles/physical/2x2x2x2/scramble-generator) or any equivalent scramble generator.
- Any full puzzle rotation that doesn't change the state (including the Gyro) may be applied to the puzzle during inspection; other moves may not.

## Fewest-moves solving rules

- Log files are required for submission.
- Video evidence is not required.
- Collaboration is allowed; each collaborator must be given the option to be credited for the solve, and should be credited if their contributions were significant.

### Computer-assisted fewest-moves solving rules

- Fewest-moves solving rules apply, except that using software to compute a partial or full solution is allowed.

## Principles when writing new speedsolving software

If you're thinking of writing a new program for speedsolving or suggesting a new feature for Hyperspeedcube, here are some principles we try to follow:

- No more than one move per keypress.
- If your program has keybinds (especially customizable ones), add some reference that shows what keys are being pressed and what they're doing.
- New features should hopefully make solving strategy more interesting. Some examples:
    - Macros on the 3^4^ encourage commutator spam, which is very boring compared to layer-by-layer or F2L methods, so they are not allowed for speedsolves.
    - Piece filters reduce time spent looking for pieces, which is boring to do and boring to watch. There's a trade-off there: piece filters encourage a stricter solving order, which is less interesting in a way, but this also enables [3-Block](/methods/3x3x3x3/3block), a very interesting method.
- New features should ideally have some justification based on 3D speedsolving. For example, multiple keybind sets is analogous to different grips on a 3D puzzle.[^grip]

[^algsheets]: We can't stop you from using an algorithm reference, but it's not in the spirit of the competition and it'll probably slow you down.
[^keybinds-ref]: If the program doesn't have a built-in keybinds reference (such as akkei's physical 3^4^ simulator) then you probably don't need one.
[^alg-keybinds]: In particular, you should not be able to execute a meaningful algorithm by pressing a sequence of keys in a line on the keyboard. Keybinds should be laid out in a way that makes sense moreso than a way that is useful for an algorithm. A keybind set optimized for general RKT is fine. If you have a question about this, ask on the Discord.
[^grip]: You might hold a 3^3^ differently to execute `<M,U>` moves more efficiently compared to `<R,U,F>` moves. Similarly, a 4D creature might have a specialized grip on the 3^4^ for RKT compared to general moves.
