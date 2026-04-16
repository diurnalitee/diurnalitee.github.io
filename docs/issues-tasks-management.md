## Issues & Task Management

To keep track of work, I usually use some kind of external task board or planning tool. This might be something like Trello, Miro, Milanote, or even Obsidian.

The exact tool does not really matter that much. What matters is that it works well for everyone in the team and does not become an obstacle in the workflow.

The entire point of this system is to support development, not to create extra annoying admin work for no reason. The issue system should not be a headache to make, maintain, or handle.

If creating or updating issues becomes overly annoying, then the system is starting to work against the team instead of for it.

When in doubt, [K.I.S.S.](https://en.wikipedia.org/wiki/KISS_principle)!

### General Approach

I usually prefer a Kanban-style approach, because it gives a simple overview of what still needs to be done, what is currently being worked on, and what is finished.

A very basic structure is usually enough:

```text
Backlog -> To Do -> In Progress -> Review -> Done
```

No need to overcomplicate it if a simple board does the job.

### About Issues

User stories, tasks, whatever you want to call them, from here on I will refer to them as **issues**.

Issues should be clear, manageable, and actually useful.

What I generally want from an issue:

* Clear requirements
* Clear steps or context, if needed
* A clearly defined **Definition of Done**
* A clear priority
* Small enough scope to finish in a few hours

If an issue is too large, it should probably be split into multiple smaller issues.

### Definition of Done

An issue should not just be "kind of worked on" or "mostly done probably". It should be clear when it is actually finished. This means the issue should define what needs to be true before it can be considered done.

Depending on the task, this might include things like:

* Feature is implemented
* Bug is fixed
* Tested and working
* Reviewed
* Documentation updated, if needed

Basically, make it clear what "done" actually means:

```text
Feature: Basic inventory system

Definition of Done:
- Player can open and close the inventory (e.g. with `E`)
- Items can be added to the inventory
- Items are displayed correctly in the UI
- No errors in the console during normal use
- Functionality tested in `TestScene`
- Code reviewed and approved
```

### Priorities

Issues should also have clear priorities. Not everything is equally urgent or important, and if priorities are unclear, people can easily end up working on the wrong thing first.

This does not need to be super complicated. Even something simple is fine, as long as it is obvious what should take priority.

### Issue Template & Example

```text
## Summary
Short explanation of the task / feature / bug.

## Context
(Optional) Why is this needed?
- What problem does this solve?
- Where does this fit in the project?

## Requirements
- Clear requirement 1
- Clear requirement 2
- Keep these actionable

## Tasks / Steps
(Optional, if helpful)
- Step 1
- Step 2
- Step 3

## Definition of Done
- What must be true for this to be considered finished?
- Feature works as expected
- No errors in console
- Tested in [scene / system]
- (Add anything relevant for this specific task)

## Priority
High / Medium / Low

## Notes
(Optional)
Anything extra that might help whoever picks this up.
```

```text
## Summary
Add basic inventory UI toggle

## Context
We need a way for the player to open and close the inventory.

## Requirements
- Pressing `E` opens the inventory
- Pressing `E` again closes it
- Inventory UI is visible when open

## Definition of Done
- Inventory toggles correctly with `E`
- UI appears and disappears as expected
- No console errors
- Tested in `TestScene`

## Priority
High
```