# Contributing
If, for whatever reason, you are using my VS Codium profiles... thank you first of all, I guess...?

## Something doesn't work
If there are *any* problems with my profiles feel free to open an issue describing whatever bug you encountered, just make sure that the bug is **reproducible** and not a VS Codium bug in itself.

### Good Example
Suppose there is a Node.js profile that provides linting through ESLint and that formats the code using Prettier. Sometimes it may happen that Prettier, when formatting the code, breaks your linting your rules; since you don't want to change linting rules to comply with Prettier output, you decide to use [`prettier-eslint`](https://github.com/prettier/prettier-eslint) to format the code before linting it in order to make the final out compliant with your linting rules. 

Great, you've found a way to make your code the way you want it, but right now it's kinda tedious formatting the code as VS Codium doesn't know how to do it. To also address this issue, you decide to use this [*amazing extension*](https://github.com/idahogurl/vs-code-prettier-eslint) and everything works great.

Time passed and now various dependencies got new versions, including breaking changes ones. Anyway, you decide to create a new project, automatically you'll also get the most recent (hopefully) stable version of the dependencies. Among these updated dependencies, there is ESLint v9.x. Somehow the *amazing extension* mentioned earlier doesn't work anymore, you look at the output and find out that the issue is caused by `prettier-eslint` not supporting the new ESLint version (check out [this issue](https://github.com/idahogurl/vs-code-prettier-eslint/issues/236#issuecomment-2622311536) if you want to know more), this will break the *amazing extension* as it relies on that dependency thus breaking the VS Codium profile.

Unless `prettier-eslint` gets support for ESLint v9.x and the [maintainer](https://github.com/idahogurl "Rebecca Vest's GitHub profile") of the *amazing extension* also updates their extension, the VS Codium profiles as it is won't work anymore and thus this is the time when an issue *must* be opened to handle the breaking changes.

### Bad Example
Suppose you have to share your coding workspace with your buddy using Live Share. For some reason, the extension just *doesn't work*. You can't figure out why so you open an issue in this repository. 

The problem was that you were missing `icu69` and the issue wasn't in the VS Codium profile itself but in your system. There isn't much I can do about it except *trying* to point you towards a *possible* solution and closing the issue; please don't interpret this as being rude.