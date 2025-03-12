# VS Codium Profiles
A collection of (opinionated) VS Codium profiles for various development environments.

Unfortunately `.code-profile` files don't self-reference themselves; this means that, when updating a profile that is being extended, the update will propagate to all profiles that extend it resulting in a kinda redundant version control. Unfortunately can't do much about it without making some over-engineered stuff that doesn't need to exist.

## Profiles
Currently, there aren't many profiles, this list will grow as I have to work with various environments. Anyway, these are the respective profile scopes
- [`default`](#default), contains extensions used in everyday development like a theme, *all* profiles must extend this.
- [`angular`](#angular), contains extensions used for Angular development.

### `default`
Includes the following extensions
- **GitHub Theme** (`github.github-vscode-theme`) with **GitHub Dark Default** because it doesn't look like a burned dark theme to me.
- **GitHub Copilot** (`github.copilot`), for when you are doing repetitive stuff that an AI can easily automate; please don't depend and neither reply on this for generating *actual* code, save yourself.
- **GitHub Copilot Chat** (`github.copilot-chat`) (comes with "GitHub Copilot" extension pack), use this before querying your (meta)search engine, *may* give some pointers on what to look for when doing the actual search; don't rely on informationg given by the LLM, **always** (and I mean *always*) educate yourself about whatever you are querying, don't be an AI relay.
- **Live Share** (`ms-vsliveshare.vsliveshare`), basically an interactive way for screensharing code when you are with your buddy on Discord.
- **vscode-pdf** (`tomoki1207.pdf`), for opening PDF inside VS Codium. This is a *lot* useful if you need to implement something that has to be compliant with some standard; code on the left, specifications on the right.
- **Remote - SSH** (`ms-vscode-remote.remote-ssh`), because sometime you have to do a quick patch on your production server.
- **Remote - SSH: Editing Configuration Files** (`ms-vscode-remote.remote-ssh-edit`), comes with the "Remote - SSH" extension pack, don't know what purpose this serves.
- **Remote Explorer** (`ms-vscode.remote-explorer`), comes with the "Remote - SSH" extension pack, don't know what purpose this serves.

### `angular`
Extends the [`default`](#default) profile.

Includes the following extensions
- **Angular Language Service** (`angular.ng-template`), language server for Angular templates (I think so).
- **ESLint** (`dbaeumer.vscode-eslint`), because linting (and formatting) your code is **essential**.
- **Sass (.sass only)** (`syler.sass-indented`), for hightling, autocompleting and formatting your Sass files.