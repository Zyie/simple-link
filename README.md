# Simple Links
Provides a simpler way to link local projects together instead of using npm link.

## Installation

```sh
npm install -g simple-links
```

Alternatively, you can use npx to run the command without installing it globally.

```sh
npx simple-links
```

## Usage

There are two aliases for the command, `sl` and `simple-link`.

```sh
sl ../path/to/some-package ./node_modules/some-package
```

You can also watch for changes and it will automatically update the link.
```sh
sl ../path/to/some-package ./node_modules/some-package -w
```

## Limitations
Simple links will not copy over `node_modules` therefore if you are working on an unreleased repo, or have added a new module to an existing one, you will run into issues of missing modules.
