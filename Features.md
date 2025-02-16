# Feature comparison of Smalltalk Web frameworks

## Abstract

So frameworks where you can develop in Smalltalk (ST) and run your code in JavaScript (JS),\
in the front-end (browsers, Electron, etc.) and the back-end (Node.js, Deno, Bun, ...).

Currenty these ST to JS frameworks are compared in the tables below:\
CodeParadise (CP), PharoJS including WebST (PJS), SmallJS (SJS)

TODO: Complete CP en PJS parts.\
TODO: More featues of CP and PJS?\
TODO: Detail pages for subjects like debugging, async.

## Feature tables

### Architecture

| Feature | CP | PJS | SJS | Remarks |
| :--- | :---: | :---: | :---: | :--- |
| JS Runtime | bytecode | JS code | JS code |  |
| Modular image |  |  | - |  |
| JS low-level performance | - | +? | - |  |

### Smalltalk core library

| Feature | CP | PJS | SJS | Remarks |
| :--- | :---: | :---: | :---: | :--- |
| ST number hierarchy |  |  | + | Including: LargeInteger, Float, Fraction |
| JS or ST library standard |  |  | JS |  Uses JS or ST 'standard' classes and method names  |
| Single framework (no bridges) |  |  | + |  |
| async / await |  |  | + |  |
| GUI model | MVP |  | MVC |  |
| HTML component framework | Shoelace(1) |  | plain HTML | Shoelace is based on Web Components |
| HTML generate or DOM link |  | generate | link |  |

### Front-end environments / frameworks

| Feature | CP | PJS | SJS | Remarks |
| :--- | :---: | :---: | :---: | :--- |
| Browser support:  |  |  | C,F | Chromium, Firefox, Safari |
| Desktop support |  |  | E,N | Electron, NodeGui |

### Back-end environments / frameworks

| Feature | CP | PJS | SJS | Remarks |
| :--- | :---: | :---: | :---: | :--- |
| Node.js |  |  | + |  |
| Deno |  |  | ? | ? = untested |
| Bun |  |  | ? | ? = untested |
| HTTP server |  | Zinc | Http-sever |  |
| App server |  | Seaside? | ExpressJS |  |
| Database support |  |  | S,P,M | SQLite, Postgres, MySQL / MariaDB  |
| AI support  |  |  |  | Soon: OpenAI, DeepSeek |

### Development

| Feature | CP | PJS | SJS | Remarks |
| :--- | :---: | :---: | :---: | :--- |
| IDE | Pharo | Pharo | VSCode |  |
| Live image | + | + | - |  |
| Image or File based | Image | Image | File |  |
| Separate HTML / CSS files (tooling) |  |  | + |  |
| Playground |  |  | + |  |
| Standalone deployment | +(1) | + | + | (1) MPV apps need server |
| Git tools | Metacello | Metacello | all file based |  |
| JS / TS source-level integration |  |  | + |  |

### Debugging

| Feature | CP | PJS | SJS | Remarks |
| :--- | :---: | :---: | :---: | :--- |
| ST source debugging |  |  | + | SJS through source map |
| ST step debugging |  |  | + |  SJS shows ST wrappers in JS (1) |
| JS source debugging |  |  | + |  |
| JS runtime debugging |  |  | + |  |
| async debugging |  |  | + |  |

(1) Would need VSCode Language server prevent, but that's a lot of effort
and would hide the JS running underneath.


