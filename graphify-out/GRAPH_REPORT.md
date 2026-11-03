# Graph Report - Mern-Template  (2026-11-03)

## Corpus Check
- 46 files · ~5,794 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 283 nodes · 403 edges · 19 communities (14 shown, 4 thin omitted)
- Extraction: 99% EXTRACTED · 1% INFERRED · 0% AMBIGUOUS · INFERRED: 3 edges (avg confidence: 0.85)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `cb11a4e3`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- App.tsx
- profile/index.mjs
- client/package.json
- server/package.json
- compilerOptions
- compilerOptions
- compilerOptions
- devDependencies
- dependencies
- package.json
- dependencies
- vercel.json
- Getting Started
- server/vercel.json
- vite-env.d.ts
- tsconfig.json
- client/vercel.json
- server/README.md

## God Nodes (most connected - your core abstractions)
1. `compilerOptions` - 20 edges
2. `compilerOptions` - 18 edges
3. `compilerOptions` - 15 edges
4. `store` - 13 edges
5. `react` - 12 edges
6. `react-router-dom` - 9 edges
7. `axios` - 7 edges
8. `BackendUrl` - 7 edges
9. `scripts` - 7 edges
10. `Button()` - 6 edges

## Surprising Connections (you probably didn't know these)
- `App()` --calls--> `store`  [EXTRACTED]
  client/src/App.tsx → client/src/store/states.ts
- `Navbar()` --calls--> `store`  [EXTRACTED]
  client/src/components/Navbar.tsx → client/src/store/states.ts
- `Home()` --calls--> `store`  [EXTRACTED]
  client/src/pages/Home.tsx → client/src/store/states.ts
- `Login()` --calls--> `store`  [EXTRACTED]
  client/src/pages/Login.tsx → client/src/store/states.ts
- `Profile()` --calls--> `store`  [EXTRACTED]
  client/src/pages/Profile.tsx → client/src/store/states.ts

## Import Cycles
- None detected.

## Communities (19 total, 4 thin omitted)

### Community 0 - "App.tsx"
Cohesion: 0.13
Nodes (25): App(), Button(), ButtonProps, FormProps, ButtonProps, Input(), SpinnerLoader(), Navbar() (+17 more)

### Community 1 - "profile/index.mjs"
Cohesion: 0.14
Nodes (19): bcryptjs, cors, express, jsonwebtoken, mongoose, multer, connect_db(), handleMulterError() (+11 more)

### Community 2 - "client/package.json"
Cohesion: 0.08
Nodes (28): @types/bun, typescript, name, private, scripts, build, dev, lint (+20 more)

### Community 3 - "server/package.json"
Cohesion: 0.07
Nodes (30): cloudinary, dotenv, express-rate-limit, morgan, nodemailer, nodemon, sharp, streamifier (+22 more)

### Community 4 - "compilerOptions"
Cohesion: 0.10
Nodes (20): compilerOptions, allowImportingTsExtensions, allowJs, jsx, lib, module, moduleDetection, moduleResolution (+12 more)

### Community 5 - "compilerOptions"
Cohesion: 0.10
Nodes (19): compilerOptions, allowArbitraryExtensions, allowImportingTsExtensions, erasableSyntaxOnly, jsx, lib, module, moduleDetection (+11 more)

### Community 6 - "compilerOptions"
Cohesion: 0.12
Nodes (16): compilerOptions, allowImportingTsExtensions, erasableSyntaxOnly, lib, module, moduleDetection, noEmit, noFallthroughCasesInSwitch (+8 more)

### Community 7 - "devDependencies"
Cohesion: 0.14
Nodes (14): devDependencies, eslint, @eslint/js, eslint-plugin-react-hooks, eslint-plugin-react-refresh, globals, @types/bun, @types/node (+6 more)

### Community 8 - "dependencies"
Cohesion: 0.14
Nodes (14): dependencies, bcryptjs, cloudinary, cors, dotenv, express, express-rate-limit, jsonwebtoken (+6 more)

### Community 9 - "package.json"
Cohesion: 0.12
Nodes (15): dependencies, client, server, name, private, scripts, build, dev (+7 more)

### Community 10 - "dependencies"
Cohesion: 0.20
Nodes (10): dependencies, axios, react, react-dom, react-icons, react-otp-input, react-router-dom, tailwindcss (+2 more)

### Community 11 - "vercel.json"
Cohesion: 0.20
Nodes (9): framework, root, rewrites, $schema, framework, root, services, client (+1 more)

### Community 12 - "Getting Started"
Cohesion: 0.25
Nodes (7): Features, Getting Started, Installation, MERN Starter Template, Prerequisites, Running Development Servers, Tech Stack

### Community 13 - "server/vercel.json"
Cohesion: 0.50
Nodes (3): builds, routes, version

## Knowledge Gaps
- **170 isolated node(s):** `name`, `private`, `version`, `type`, `dev` (+165 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 177 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **4 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `devDependencies` connect `devDependencies` to `client/package.json`?**
  _High betweenness centrality (0.030) - this node is a cross-community bridge._
- **Why does `react` connect `App.tsx` to `client/package.json`?**
  _High betweenness centrality (0.026) - this node is a cross-community bridge._
- **Why does `dependencies` connect `dependencies` to `server/package.json`?**
  _High betweenness centrality (0.023) - this node is a cross-community bridge._
- **What connects `name`, `private`, `version` to the rest of the system?**
  _170 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `App.tsx` be split into smaller, more focused modules?**
  _Cohesion score 0.12896405919661733 - nodes in this community are weakly interconnected._
- **Should `profile/index.mjs` be split into smaller, more focused modules?**
  _Cohesion score 0.14408602150537633 - nodes in this community are weakly interconnected._
- **Should `client/package.json` be split into smaller, more focused modules?**
  _Cohesion score 0.07741935483870968 - nodes in this community are weakly interconnected._