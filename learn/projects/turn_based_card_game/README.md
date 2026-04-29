# Turn-Based Card Game

Purpose: learn turn order, state machines, hand/deck/discard logic, AI turns, and later networking-friendly deterministic rules.

Think of this as:
- card-shedding game
- color/number matching game
- action-card game
- UNO-like learning project without depending on brand-specific content

## What You Learn

1. turn state
2. deck / hand / discard piles
3. draw rules
4. playable card validation
5. AI turn logic
6. win condition
7. UI state and highlighting
8. deterministic rules for future networking

## Good Small First Version

Rules:
1. 2 players only
2. colors: red, blue, green, yellow
3. numbers: 0-4 only
4. match by color or number
5. if no card playable, draw 1
6. first empty hand wins

## Starter Controls

- `A` / Left: previous card
- `D` / Right: next card
- `Enter` / Space: play selected card
- `S` / Down: draw one card if no legal play
- `Tab`: reveal both hands
- `R`: reset game

## Files

- `main.odin`: playable hot-seat starter
- `build.sh`: run it

Run with:

```sh
zsh build.sh
```

Do not start with:
- wild cards
- stacking rules
- online play
- animations
- complicated AI

## Good Build Order

1. hardcode small deck
2. deal hands
3. top discard card visible
4. current player highlight
5. playable card validation
6. pass turn
7. draw when blocked
8. win check

## Good Upgrades

1. skip card
2. reverse card
3. draw-two card
4. simple CPU opponent
5. local multiplayer input
6. replay log
7. network-ready action messages

## Why This Is Useful

Turn-based card games teach:
- state machines very clearly
- data modeling
- UI feedback
- deterministic actions

That helps puzzle games, co-op games, and future networking too.
