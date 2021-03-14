# How to Write a Git Commit Message

*A project’s long-term success rests (among other things) on its maintainability, and a maintainer has few tools more powerful than his project’s log. It’s worth taking the time to learn how to care for one properly. What may be a hassle at first soon becomes habit, and eventually a source of pride and productivity for all involved.*

*In this post, I am addressing just the most basic element of keeping a healthy commit history: how to write an individual commit message. There are other important practices like commit squashing that I am not addressing here. Perhaps I’ll do that in a subsequent post.*

*Most programming languages have well-established conventions as to what constitutes idiomatic style, i.e. naming, formatting and so on. There are variations on these conventions, of course, but most developers agree that picking one and sticking to it is far better than the chaos that ensues when everybody does their own thing.*

### A team’s approach to its commit log should be no different. In order to create a useful revision history, teams should first agree on a commit message convention that defines at least the following three things:

1. Style: Markup syntax, wrap margins, grammar, capitalization, punctuation. Spell these things out, remove the guesswork, and make it all as simple as possible. The end result will be a remarkably consistent log that’s not only a pleasure to read but that actually does get read on a regular basis.

2. Content: What kind of information should the body of the commit message (if any) contain? What should it not contain?

3. Metadata: How should issue tracking IDs, pull request numbers, etc. be referenced?

*Fortunately, there are well-established conventions as to what makes an idiomatic Git commit message. Indeed, many of them are assumed in the way certain Git commands function. There’s nothing you need to re-invent. Just follow the seven rules below and you’re on your way to committing like a pro.*

### The seven rules of a great Git commit message

1. Keep in mind: This has all been said before.
2. Separate subject from body with a blank line.
3. Limit the subject line to 50 characters.
4. Capitalize the subject line.
5. Do not end the subject line with a period.
6. Use the imperative mood in the subject line.
Wrap the body at 72 characters.
7. Use the body to explain what and why vs.

*Before now, I only used git commit -m "Fix X to allow Y to use Z" on my personal projects with just a subject and no extra description. This is great for small and clear fixes like git commit -m "Fix typo in README.md, but in cases of more extensive changes, you would need to add some extra details.*

### Editor method

*Run git commit without a message or option and it'll open up your default text editor to write a commit message.*

#### To configure your "default" editor:

*git config --global core.editor nano
This would configure Git to use nano as your default editor. Replace "nano" with "emacs," "vim," or whatever your preference is.*

*In the opened editor, the first line is the subject (short description), leave a blank line after it, and everything else is the extended description (body).*


## How to write good commit messages

*There are several conventions used by different teams and developers to write good commit messages. I'll only outline some general rules and tips for writing commit messages–you have to decide what convention you want to follow. And if you work for a company or contribute to open source, you have to adapt to their convention :).*

*For consistency, you can use one convention for work and another for personal projects as you might change jobs sometime, and the convention might also change.*

*Be sure to check out this thread for some amazing commit message conventions or add yours to help someone make a decision.*

*Here's a great template of a good commit message originally written by Tim pope*

#### Looks great, right? Here's how you can make yours great too:

1. Specify the type of commit:

. feat: The new feature you're adding to a particular application.
. fix: A bug fix.
. style: Feature and updates related to styling.
. refactor: Refactoring a specific section of the codebase.
. test: Everything related to testing.
. docs: Everything related to documentation.
. chore: Regular code maintenance.[ You can also use emojis to represent commit types].

2. Separate the subject from the body with a blank line.
3. Your commit message should not contain any whitespace errors.
4. Remove unnecessary punctuation marks.
5. Do not end the subject line with a period.
6. Capitalize the subject line and each paragraph.
7. Use the imperative mood in the subject line.
8. Use the body to explain what changes you have made and why you made them.
9. Do not assume the reviewer understands what the original problem was, ensure you add it.
10. Do not think your code is self-explanatory.
11. Follow the commit convention defined by your team.