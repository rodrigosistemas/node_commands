## Node Principal Commands

<img src="https://github.com/rodrigosistemas/node_commands/blob/main/img/nodejs.png" alt="nmap" width="300"/>

### Create a New Node.js Project

```bash
npm init
```

*Interactively create a `package.json`* for your project, prompting you for metadata (name, version, entry point, etc.).

### Run Your Project in Development Mode

```bash
npm run dev
```

*Execute the “dev” script* defined in your `package.json` (often starts a watcher or nodemon to auto-reload on changes).

```bash
npm start
```

*Run the “start” script*—the conventional way to launch your application in production mode.

```bash
npm run build
```

*Execute the “build” script*—typically compiles/transpiles your source (e.g. Babel, Webpack, TypeScript) into a distributable format.

### Install Dependencies

#### Globally

```bash
npm install -g <package_name>
```

*Make a package available system-wide*, so you can run its CLI from any directory.

#### Locally (per project)

```bash
npm install <package_name>
```

*Add a runtime dependency* to your project (saved under `dependencies` in `package.json`).

#### For Development Only

```bash
npm install --save-dev <package_name>
```

*Add a build/test tool* (e.g. linters, transpilers) under `devDependencies`, not required in production.

### View Installed Packages

```bash
npm list
```

*Show the dependency tree* of all packages installed in the current project.

### Remove Packages

```bash
npm uninstall <package_name>
```

*Remove a local dependency* from your project and `package.json`.

```bash
npm uninstall -g <package_name>
```

*Remove a globally installed package*.
   You can specify a package version inline (e.g. `npx create-next-app@12.0.0`), so you always get the exact toolchain you need.

4. **Zero-Install Scripting**
   Great for quick tasks or one-off scripts—no need to modify your `package.json` or maintain global installs.

By leveraging `npx`, you keep your environment clean, guarantee you’re running the correct version of a tool, and save the step of globally installing CLIs you only need occasionally.
