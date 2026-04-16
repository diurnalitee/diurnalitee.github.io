## Pull Request (PR) Etiquette

Pull requests should be clear, focused, and easy to review. Here is my approach!

### Title Format

```text
[type] short description
```

Examples:

```text
[feat] add inventory system
[fix] resolve null reference in input handler
[refactor] simplify manager logic
[docs] update workflow notes
```

### Description Template

When opening a PR, I include enough context that someone can quickly understand what changed, why it changed, and how to test it.

```text
## Summary
Brief explanation of what this PR does.

## Changes
- List of key changes
- Keep it concise

## Why
Explain the reasoning behind the change.

## Validation / Testing Instructions
Explain how to check that the change works.

For Unity project specifically, I include things like:
- which scene to open
- which prefab or object to use
- which buttons to press
- what behavior is expected
- any setup required before testing

Example:
- Open `Scenes/TestScene`
- Select the `InventoryTester` prefab
- Press Play
- Press `E` to open the inventory
- Add an item through the test button in the inspector
- Confirm the item appears correctly in the UI

## Notes
Optional: anything reviewers should pay attention to.
```

### Before Opening a PR

Before I open a PR, I check the following:

1. Does the code run?
2. Does the code follow coding/naming conventions?
3. Good file separation? File structure good?
4. Did I leave in any unnecessary debug logs, test objects, or temporary hacks?
   1. If yes, get rid of them first
5. Recheck everything I've changed just in case. Maybe even twice

### Review Behavior

When reviewing PRs or receiving review feedback, I keep a few things in mind:

* Keep it constructive; provide feedback that is actually helpful.
* Be direct; express concerns and problems clearly.
* Is this important or a [nit](https://stackoverflow.com/questions/27810522/what-does-nit-mean-in-hacker-speak)?
  * Is the nit too nitty? Should I include it??? Be reasonable!
* For receiving feedback, remember that critique is (almost always) impersonal, and the best thing to do is to look at it with the aim to improve :)
* It is, however, important to not just blindly agree with critique, use yer brain! If unsure, ask a third party!
