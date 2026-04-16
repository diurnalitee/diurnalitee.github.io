## Commit Guidelines

Each commit should be similar to an individual step in a cooking recipe, not the entire recipe!

### General Habits

Generally, I try to commit frequently but logically. Each commit should represent a meaningful step. Whenever a component of a system is completed, commit. If you've half-finished a function and the program doesn't even compile, maybe don't commit.  
I am guilty of forgetting to commit while I'm in the flow state. Whenever this happens I try to retroactively make several commits instead of just dumping everything into one giant commit.

**Good examples:**

* one feature split into logical milestones
* separate commits for refactors, fixes, and new features

**Bad examples:**

* `stuff`
* `updates`
* one massive commit touching half the project without any provided context

### Commit Message Format

I use this format:

```text
type: short description
```

Types I tend to use:

* `feat`     new feature
* `fix`      bug fix
* `refactor` code changes without behavior change
* `docs`     documentation changes
* `style`    formatting only, no logic change

Examples:

```text
feat: add basic dialogue system
fix: prevent crash when inventory is empty
refactor: simplify input parsing logic
docs: add workflow documentation
```

If something needs more context, I use the expanded commmit message, usually in bullet points:

```text
type: short description

- Optional longer explanation if needed.
- Like this so it shows up concise and easy to skim on GitHub!
```

### Frequency

I generally think it is a good time to commit when:

* a small feature is complete
* a bug is fixed
* a logical chunk of work is finished
* the project has reached a stable checkpoint

I usually avoid waiting until everything is done, because that tends to create messy history and harder reviews.

For **pushing**, I usually push at the end of a workday or when, like with a commit, the project/system I'm working on has reached a stable checkpoint.
