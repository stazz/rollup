# rollup changelog

## 4.46.0

_2025-07-27_

### Features

- Optimize `in` checks on namespaces to keep them treeshake-able (#6029)

### Pull Requests

- [#5991](https://github.com/rollup/rollup/pull/5991): feat: update linux-loongarch64-gnu (@wojiushixiaobai, @lukastaegert)
- [#6029](https://github.com/rollup/rollup/pull/6029): feat: optimize `in` checks on namespaces to keep them treeshake-able (@cyyynthia, @lukastaegert)
- [#6033](https://github.com/rollup/rollup/pull/6033): fix(deps): update swc monorepo (major) (@renovate[bot], @lukastaegert)

## 4.45.3

_2025-07-26_

### Bug Fixes

- Do not fail build if a const is reassigned but warn instead (#6020)
- Fail with a helpful error message if an exported binding is not defined (#6023)

### Pull Requests

- [#6014](https://github.com/rollup/rollup/pull/6014): chore(deps): update dependency @vue/language-server to v3 (@renovate[bot])
- [#6015](https://github.com/rollup/rollup/pull/6015): chore(deps): update dependency vue-tsc to v3 (@renovate[bot], @lukastaegert)
- [#6016](https://github.com/rollup/rollup/pull/6016): fix(deps): update swc monorepo (major) (@renovate[bot], @lukastaegert)
- [#6017](https://github.com/rollup/rollup/pull/6017): fix(deps): lock file maintenance minor/patch updates (@renovate[bot], @lukastaegert)
- [#6020](https://github.com/rollup/rollup/pull/6020): Make const reassignments only a warning (@lukastaegert)
- [#6023](https://github.com/rollup/rollup/pull/6023): Throw descriptive error message for used export is not defined (@TrickyPi)
- [#6027](https://github.com/rollup/rollup/pull/6027): feat: upgrade to NAPI-RS 3 stable (@Brooooooklyn)
- [#6028](https://github.com/rollup/rollup/pull/6028): Update eslint-plugin-unicorn to resolve vulnerability (@lukastaegert)
- [#6034](https://github.com/rollup/rollup/pull/6034): fix(deps): lock file maintenance minor/patch updates (@renovate[bot], @lukastaegert)

## 4.45.1

_2025-07-15_

### Bug Fixes

- Resolve crash when using certain conditional expressions (#6009)

### Pull Requests

- [#6009](https://github.com/rollup/rollup/pull/6009): Add hasDeoptimizedCache flag for ConditionalExpression (@TrickyPi)

## 4.45.0

_2025-07-12_

### Features

- Improve tree-shaking when both branches of a conditional expression return the same boolean value (#6000)
- In environments that support both CJS and ESM, prefer the ESM build of Rollup (#6005)

### Bug Fixes

- Ensure static blocks do not prevent tree-shaking if they access `this` (#6001)

### Pull Requests

- [#6000](https://github.com/rollup/rollup/pull/6000): feat: improve get literal value for conditional expression (@ahabhgk, @lukastaegert)
- [#6001](https://github.com/rollup/rollup/pull/6001): Correct the parent scope for static blocks (@TrickyPi, @lukastaegert)
- [#6005](https://github.com/rollup/rollup/pull/6005): fix: export field order prefer esm (@DylanPiercey)

## 4.44.2

_2025-07-04_

### Bug Fixes

- Correctly handle `@__PURE__` annotations after `new` keyword (#5998)
- Generate correct source mapping for closing braces of block statements (#5999)

### Pull Requests

- [#5998](https://github.com/rollup/rollup/pull/5998): Support `@__PURE__` when nested after new in constructor invocations (@TrickyPi)
- [#5999](https://github.com/rollup/rollup/pull/5999): Add location info for closing brace of block statement (@TrickyPi)
- [#6002](https://github.com/rollup/rollup/pull/6002): chore(deps): update dependency vite to v7 (@renovate[bot], @lukastaegert)
- [#6004](https://github.com/rollup/rollup/pull/6004): fix(deps): lock file maintenance minor/patch updates (@renovate[bot], @lukastaegert)

## 4.44.1

_2025-06-26_

### Bug Fixes

- Reinstate maxParallelFileOps limit of 1000 to resolve the issue for some (#5992)

### Pull Requests

- [#5988](https://github.com/rollup/rollup/pull/5988): fix(deps): lock file maintenance minor/patch updates (@renovate[bot], @lukastaegert)
- [#5992](https://github.com/rollup/rollup/pull/5992): Set maxParallelFileOps to 1000 (@lukastaegert)

## 4.44.0

_2025-06-19_

### Features

- Remove limit on `maxParallelFileOps` as this could break watch mode with the commonjs plugin (#5986)

### Bug Fixes

- Provide better source mappings when coarse intermediate maps are used (#5985)

### Pull Requests

- [#5984](https://github.com/rollup/rollup/pull/5984): fix(deps): lock file maintenance minor/patch updates (@renovate[bot], @lukastaegert)
- [#5985](https://github.com/rollup/rollup/pull/5985): Improve approximation of coarse sourcemap segments (@TrickyPi)
- [#5986](https://github.com/rollup/rollup/pull/5986): Remove limit on max parallel file ops (@lukastaegert)

## 4.43.0

_2025-06-11_

### Features

- Provide new `fs` option and `this.fs` API to replace file system (#5944)

### Pull Requests

- [#5944](https://github.com/rollup/rollup/pull/5944): feat(options): Add an option for overriding the file system module in the JS API (@EggDice, @lukastaegert)

## 4.42.0

_2025-06-06_

### Features

- Add option to allow the input to be located in the output in watch mode (#5966)

### Pull Requests

- [#5966](https://github.com/rollup/rollup/pull/5966): feat: watch mode add `allowInputInsideOutputPath` option (@btea, @lukastaegert)

## 4.41.2

_2025-06-06_

### Bug Fixes

- Detect named export usages in dynamic imports with `then` and non-arrow function expressions (#5977)
- Do not replace usages of constant variables with their values for readability (#5968)

### Pull Requests

- [#5968](https://github.com/rollup/rollup/pull/5968): fix: preserve constant identifiers in unary expressions instead of magic numbers (@OmkarJ13, @lukastaegert)
- [#5969](https://github.com/rollup/rollup/pull/5969): chore(deps): update dependency yargs-parser to v22 (@renovate[bot], @lukastaegert)
- [#5970](https://github.com/rollup/rollup/pull/5970): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5971](https://github.com/rollup/rollup/pull/5971): chore(deps): lock file maintenance (@renovate[bot])
- [#5976](https://github.com/rollup/rollup/pull/5976): Update README.md (@ftlno, @lukastaegert)
- [#5977](https://github.com/rollup/rollup/pull/5977): fix: consider function expression in thenable when tree-shaking dynamic imports (@TrickyPi)
- [#5981](https://github.com/rollup/rollup/pull/5981): fix(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5982](https://github.com/rollup/rollup/pull/5982): Debug/fix watch pipeline (@lukastaegert)

## 4.41.1

_2025-05-24_

### Bug Fixes

- If a plugin calls `this.resolve` with `skipSelf: true`, subsequent calls when handling this by the same plugin with same parameters will return `null` to avoid infinite recursions (#5945)

### Pull Requests

- [#5945](https://github.com/rollup/rollup/pull/5945): Avoid recursively calling a plugin's resolveId hook with same id and importer (@younggglcy, @lukastaegert)
- [#5963](https://github.com/rollup/rollup/pull/5963): fix(deps): update swc monorepo (major) (@renovate[bot])
- [#5964](https://github.com/rollup/rollup/pull/5964): fix(deps): lock file maintenance minor/patch updates (@renovate[bot])

## 4.41.0

_2025-05-18_

### Features

- Detect named exports in more dynamic import scenarios (#5954)

### Pull Requests

- [#5949](https://github.com/rollup/rollup/pull/5949): ci: use node 24 (@btea, @lukastaegert)
- [#5951](https://github.com/rollup/rollup/pull/5951): chore(deps): update dependency pretty-bytes to v7 (@renovate[bot])
- [#5952](https://github.com/rollup/rollup/pull/5952): fix(deps): update swc monorepo (major) (@renovate[bot], @lukastaegert)
- [#5953](https://github.com/rollup/rollup/pull/5953): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5954](https://github.com/rollup/rollup/pull/5954): enhance tree-shaking for dynamic imports (@TrickyPi, @renovate[bot], @lukastaegert)
- [#5957](https://github.com/rollup/rollup/pull/5957): chore(deps): update dependency lint-staged to v16 (@renovate[bot], @lukastaegert)
- [#5958](https://github.com/rollup/rollup/pull/5958): fix(deps): update rust crate swc_compiler_base to v20 (@renovate[bot], @lukastaegert)
- [#5959](https://github.com/rollup/rollup/pull/5959): fix(deps): lock file maintenance minor/patch updates (@renovate[bot], @lukastaegert)
- [#5960](https://github.com/rollup/rollup/pull/5960): Use spawn to run CLI tests (@lukastaegert)

## 4.40.2

_2025-05-06_

### Bug Fixes

- Create correct IIFE/AMD/UMD bundles when using a mutable default export (#5934)
- Fix execution order when using top-level await for dynamic imports with inlineDynamicImports (#5937)
- Throw when the output is watched in watch mode (#5939)

### Pull Requests

- [#5934](https://github.com/rollup/rollup/pull/5934): fix(exports): avoid "exports is not defined" `ReferenceError` (@dasa)
- [#5937](https://github.com/rollup/rollup/pull/5937): consider TLA imports have higher execution priority (@TrickyPi)
- [#5939](https://github.com/rollup/rollup/pull/5939): fix: watch mode input should not be an output subpath (@btea)
- [#5940](https://github.com/rollup/rollup/pull/5940): chore(deps): update dependency vite to v6.3.4 [security] (@renovate[bot])
- [#5941](https://github.com/rollup/rollup/pull/5941): chore(deps): update dependency eslint-plugin-unicorn to v59 (@renovate[bot])
- [#5942](https://github.com/rollup/rollup/pull/5942): fix(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5943](https://github.com/rollup/rollup/pull/5943): fix(deps): lock file maintenance minor/patch updates (@renovate[bot])

## 4.40.1

_2025-04-28_

### Bug Fixes

- Limit hash size for asset file names to the supported 21 (#5921)
- Do not inline user-defined entry chunks or chunks with explicit file name (#5923)
- Avoid top-level-await cycles when non-entry chunks use top-level await (#5930)
- Expose package.json via exports (#5931)

### Pull Requests

- [#5921](https://github.com/rollup/rollup/pull/5921): fix(assetFileNames): reduce max hash size to 21 (@shulaoda)
- [#5923](https://github.com/rollup/rollup/pull/5923): fix: generate the separate chunk for the entry module with explicated chunk filename or name (@TrickyPi)
- [#5926](https://github.com/rollup/rollup/pull/5926): fix(deps): update rust crate swc_compiler_base to v18 (@renovate[bot])
- [#5927](https://github.com/rollup/rollup/pull/5927): fix(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5928](https://github.com/rollup/rollup/pull/5928): fix(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5930](https://github.com/rollup/rollup/pull/5930): Avoid chunks TLA dynamic import circular when TLA dynamic import used in non-entry modules (@TrickyPi)
- [#5931](https://github.com/rollup/rollup/pull/5931): chore: add new `./package.json` entry (@JounQin, @lukastaegert)
- [#5936](https://github.com/rollup/rollup/pull/5936): fix(deps): lock file maintenance minor/patch updates (@renovate[bot])

## 4.40.0

_2025-04-12_

### Features

- Only show `eval` warnings on first render and only when the call is not tree-shaken (#5892)
- Tree-shake non-included dynamic import members when the handler just maps to one named export (#5898)

### Bug Fixes

- Consider dynamic imports nested within top-level-awaited dynamic import expressions to be awaited as well (#5900)
- Fix namespace rendering when tree-shaking is disabled (#5908)
- When using multiple transform hook filters, all of them need to be satisfied together (#5909)

### Pull Requests

- [#5892](https://github.com/rollup/rollup/pull/5892): Warn when eval or namespace calls are rendered, not when they are parsed (@SunsetFi, @lukastaegert)
- [#5898](https://github.com/rollup/rollup/pull/5898): feat: treeshake dynamic import chained member expression (@privatenumber, @lukastaegert)
- [#5900](https://github.com/rollup/rollup/pull/5900): consider the dynamic import within a TLA call expression as a TLA import (@TrickyPi)
- [#5904](https://github.com/rollup/rollup/pull/5904): fix(deps): update swc monorepo (major) (@renovate[bot])
- [#5905](https://github.com/rollup/rollup/pull/5905): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5908](https://github.com/rollup/rollup/pull/5908): Fix `treeshake: false` breaking destructured namespace imports (@Skn0tt)
- [#5909](https://github.com/rollup/rollup/pull/5909): Correct the behavior when multiple transform filter options are specified (@sapphi-red)
- [#5915](https://github.com/rollup/rollup/pull/5915): chore(deps): update dependency @types/picomatch to v4 (@renovate[bot])
- [#5916](https://github.com/rollup/rollup/pull/5916): fix(deps): update rust crate swc_compiler_base to v17 (@renovate[bot])
- [#5917](https://github.com/rollup/rollup/pull/5917): chore(deps): lock file maintenance minor/patch updates (@renovate[bot], @lukastaegert)
- [#5918](https://github.com/rollup/rollup/pull/5918): chore(deps): update dependency vite to v6.2.6 [security] (@renovate[bot], @lukastaegert)

## 4.39.0

_2025-04-02_

### Features

- Do not create separate facade chunks if a chunk would contain several entry modules that allow export extension if there are no export name conflicts (#5891)

### Bug Fixes

- Mark the `id` property as optional in the filter for the `resolveId` hook (#5896)

### Pull Requests

- [#5891](https://github.com/rollup/rollup/pull/5891): chunk: merge allow-extension modules (@wmertens, @lukastaegert)
- [#5893](https://github.com/rollup/rollup/pull/5893): chore(deps): update dependency vite to v6.2.4 [security] (@renovate[bot])
- [#5896](https://github.com/rollup/rollup/pull/5896): fix: resolveId id filter is optional (@sapphi-red)

## 4.38.0

_2025-03-29_

### Features

- Support `.filter` option in `resolveId`, `load` and `transform` hooks (#5882)

### Pull Requests

- [#5882](https://github.com/rollup/rollup/pull/5882): Add support for hook filters (@sapphi-red)
- [#5894](https://github.com/rollup/rollup/pull/5894): fix(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5895](https://github.com/rollup/rollup/pull/5895): chore(deps): update dependency eslint-plugin-unicorn to v58 (@renovate[bot])

## 4.37.0

_2025-03-23_

### Features

- Support Musl Linux on Riscv64 architectures (#5726)
- Handles class decorators placed before the `export` keyword (#5871)

### Bug Fixes

- Log Rust panic messages to the console when using the WASM build (#5875)

### Pull Requests

- [#5726](https://github.com/rollup/rollup/pull/5726): Add support for linux riscv64 musl (@fossdd, @leso-kn)
- [#5871](https://github.com/rollup/rollup/pull/5871): feat: support decorators before or after export (@TrickyPi)
- [#5875](https://github.com/rollup/rollup/pull/5875): capture Rust panic messages and output them to the console. (@luyahan, @lukastaegert)
- [#5883](https://github.com/rollup/rollup/pull/5883): Pin digest of 3rd party actions (@re-taro)
- [#5885](https://github.com/rollup/rollup/pull/5885): fix(deps): lock file maintenance minor/patch updates (@renovate[bot])

## 4.36.0

_2025-03-17_

### Features

- Extend `renderDynamicImport` hook to provide information about static dependencies of the imported module (#5870)
- Export several additional types used by Vite (#5879)

### Bug Fixes

- Do not merge chunks if that would create a top-level await cycle between chunks (#5843)

### Pull Requests

- [#5843](https://github.com/rollup/rollup/pull/5843): avoiding top level await circular (@TrickyPi, @lukastaegert)
- [#5870](https://github.com/rollup/rollup/pull/5870): draft for extended renderDynamicImport hook (@iczero, @lukastaegert)
- [#5876](https://github.com/rollup/rollup/pull/5876): Update axios overrides to 1.8.2 (@vadym-khodak)
- [#5877](https://github.com/rollup/rollup/pull/5877): chore(deps): update dependency eslint-plugin-vue to v10 (@renovate[bot])
- [#5878](https://github.com/rollup/rollup/pull/5878): fix(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5879](https://github.com/rollup/rollup/pull/5879): fix: export types (@sxzz)

## 4.35.0

_2025-03-08_

### Features

- Pass build errors to the closeBundle hook (#5867)

### Pull Requests

- [#5852](https://github.com/rollup/rollup/pull/5852): chore(deps): update dependency eslint-plugin-unicorn to v57 (@renovate[bot], @lukastaegert)
- [#5862](https://github.com/rollup/rollup/pull/5862): fix(deps): update swc monorepo (major) (@renovate[bot], @lukastaegert)
- [#5867](https://github.com/rollup/rollup/pull/5867): feat(5858): make closeBundle hook receive the last error (@GauBen)
- [#5872](https://github.com/rollup/rollup/pull/5872): chore(deps): update dependency builtin-modules to v5 (@renovate[bot])
- [#5873](https://github.com/rollup/rollup/pull/5873): chore(deps): update uraimo/run-on-arch-action action to v3 (@renovate[bot])
- [#5874](https://github.com/rollup/rollup/pull/5874): fix(deps): lock file maintenance minor/patch updates (@renovate[bot])

## 4.34.9

_2025-03-01_

### Bug Fixes

- Support JSX modes in WASM (#5866)
- Allow the CustomPluginOptions to be extended (#5850)

### Pull Requests

- [#5850](https://github.com/rollup/rollup/pull/5850): Revert CustomPluginOptions to be an interface (@sapphi-red, @lukastaegert)
- [#5851](https://github.com/rollup/rollup/pull/5851): Javascript to JavaScript (@dasa, @lukastaegert)
- [#5853](https://github.com/rollup/rollup/pull/5853): chore(deps): update dependency pinia to v3 (@renovate[bot])
- [#5854](https://github.com/rollup/rollup/pull/5854): fix(deps): update swc monorepo (major) (@renovate[bot])
- [#5855](https://github.com/rollup/rollup/pull/5855): fix(deps): lock file maintenance minor/patch updates (@renovate[bot], @lukastaegert)
- [#5860](https://github.com/rollup/rollup/pull/5860): chore(deps): update dependency @shikijs/vitepress-twoslash to v3 (@renovate[bot])
- [#5861](https://github.com/rollup/rollup/pull/5861): chore(deps): update dependency globals to v16 (@renovate[bot])
- [#5863](https://github.com/rollup/rollup/pull/5863): fix(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5864](https://github.com/rollup/rollup/pull/5864): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5866](https://github.com/rollup/rollup/pull/5866): Add jsx parameter to parseAsync in native.wasm.js (@TrickyPi)

## 4.34.8

_2025-02-17_

### Bug Fixes

- Do not make assumptions about the value of nested paths in logical expressions if the expression cannot be simplified (#5846)

### Pull Requests

- [#5846](https://github.com/rollup/rollup/pull/5846): return UnknownValue if the usedbranch is unkown and the path is not empty (@TrickyPi)

## 4.34.7

_2025-02-14_

### Bug Fixes

- Ensure that calls to parameters are included correctly when using try-catch deoptimization (#5842)

### Pull Requests

- [#5840](https://github.com/rollup/rollup/pull/5840): fix(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5842](https://github.com/rollup/rollup/pull/5842): Fix prop inclusion with try-catch-deoptimization (@lukastaegert)

## 4.34.6

_2025-02-07_

### Bug Fixes

- Retain "void 0" in the output for smaller output and fewer surprises (#5838)

### Pull Requests

- [#5835](https://github.com/rollup/rollup/pull/5835): fix(deps): update swc monorepo (major) (@renovate[bot], @lukastaegert)
- [#5838](https://github.com/rollup/rollup/pull/5838): replace undefined with void 0 for operator void (@TrickyPi)

## 4.34.5

_2025-02-07_

### Bug Fixes

- Ensure namespace reexports always include all properties of all exports (#5837)

### Pull Requests

- [#5836](https://github.com/rollup/rollup/pull/5836): fix(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5837](https://github.com/rollup/rollup/pull/5837): Include all paths of reexports if namespace is used (@lukastaegert)

## 4.34.4

_2025-02-05_

### Bug Fixes

- Do not tree-shake properties if a rest element is used in destructuring (#5833)

### Pull Requests

- [#5833](https://github.com/rollup/rollup/pull/5833): include all properties if a rest element is destructed (@TrickyPi)

## 4.34.3

_2025-02-05_

### Bug Fixes

- Ensure properties of "this" are included in getters (#5831)

### Pull Requests

- [#5831](https://github.com/rollup/rollup/pull/5831): include the properties that accessed by this (@TrickyPi)

## 4.34.2

_2025-02-04_

### Bug Fixes

- Fix an issue where not all usages of a function were properly detected (#5827)

### Pull Requests

- [#5827](https://github.com/rollup/rollup/pull/5827): Ensure that functions provided to a constructor are properly deoptimized (@lukastaegert)

## 4.34.1

_2025-02-03_

### Bug Fixes

- Ensure throwing objects includes the entire object (#5825)

### Pull Requests

- [#5825](https://github.com/rollup/rollup/pull/5825): Ensure that all properties of throw statements are included (@lukastaegert)

## 4.34.0

_2025-02-01_

### Features

- Tree-shake unused properties in object literals (re-implements #5420) (#5737)

### Pull Requests

- [#5737](https://github.com/rollup/rollup/pull/5737): Reapply object tree-shaking (@lukastaegert, @TrickyPi)

## 4.33.0

_2025-02-01_

### Features

- Correctly detect literal value of more negated expressions (#5812)

### Bug Fixes

- Use the correct with/assert attribute key in dynamic imports (#5818)
- Fix an issue where logical expressions were considered to have the wrong value (#5819)

### Pull Requests

- [#5812](https://github.com/rollup/rollup/pull/5812): feat: optimize the literal value of unary expressions (@TrickyPi)
- [#5816](https://github.com/rollup/rollup/pull/5816): fix(deps): update swc monorepo (major) (@renovate[bot], @lukastaegert)
- [#5817](https://github.com/rollup/rollup/pull/5817): fix(deps): lock file maintenance minor/patch updates (@renovate[bot], @lukastaegert)
- [#5818](https://github.com/rollup/rollup/pull/5818): support for changing the attributes key for dynamic imports (@TrickyPi)
- [#5819](https://github.com/rollup/rollup/pull/5819): Return UnknownValue if getLiteralValueAtPath is called recursively within logical expressions (@TrickyPi)
- [#5820](https://github.com/rollup/rollup/pull/5820): return null (@kingma-sbw)

## 4.32.1

_2025-01-28_

### Bug Fixes

- Fix possible crash when optimizing logical expressions (#5804)

### Pull Requests

- [#5804](https://github.com/rollup/rollup/pull/5804): fix: set hasDeoptimizedCache to true as early as possible (@TrickyPi)
- [#5813](https://github.com/rollup/rollup/pull/5813): Fix typo (@kantuni)

## 4.32.0

_2025-01-24_

### Features

- Add watch.onInvalidate option to trigger actions immediately when a file is changed (#5799)

### Bug Fixes

- Fix incorrect urls in CLI warnings (#5809)

### Pull Requests

- [#5799](https://github.com/rollup/rollup/pull/5799): Feature/watch on invalidate (@drebrez, @lukastaegert)
- [#5808](https://github.com/rollup/rollup/pull/5808): chore(deps): update dependency vite to v6.0.9 [security] (@renovate[bot])
- [#5809](https://github.com/rollup/rollup/pull/5809): fix: avoid duplicate rollupjs.org prefix (@GauBen, @lukastaegert)
- [#5810](https://github.com/rollup/rollup/pull/5810): chore(deps): update dependency @shikijs/vitepress-twoslash to v2 (@renovate[bot])
- [#5811](https://github.com/rollup/rollup/pull/5811): fix(deps): lock file maintenance minor/patch updates (@renovate[bot])

## 4.31.0

_2025-01-19_

### Features

- Do not immediately quit when trying to use watch mode from within non-TTY environments (#5803)

### Bug Fixes

- Handle files with more than one UTF-8 BOM header (#5806)

### Pull Requests

- [#5792](https://github.com/rollup/rollup/pull/5792): fix(deps): update rust crate swc_compiler_base to v8 (@renovate[bot])
- [#5793](https://github.com/rollup/rollup/pull/5793): fix(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5794](https://github.com/rollup/rollup/pull/5794): chore(deps): lock file maintenance (@renovate[bot])
- [#5801](https://github.com/rollup/rollup/pull/5801): chore(deps): update dependency eslint-config-prettier to v10 (@renovate[bot])
- [#5802](https://github.com/rollup/rollup/pull/5802): fix(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5803](https://github.com/rollup/rollup/pull/5803): Support watch mode in yarn, gradle and containers (@lukastaegert)
- [#5806](https://github.com/rollup/rollup/pull/5806): fix: strip all BOMs (@TrickyPi)

## 4.30.1

_2025-01-07_

### Bug Fixes

- Prevent invalid code when simplifying unary expressions in switch cases (#5786)

### Pull Requests

- [#5786](https://github.com/rollup/rollup/pull/5786): fix: consider that literals cannot following switch case. (@TrickyPi)

## 4.30.0

_2025-01-06_

### Features

- Inline values of resolvable unary expressions for improved tree-shaking (#5775)

### Pull Requests

- [#5775](https://github.com/rollup/rollup/pull/5775): feat: enhance the treehshaking for unary expression (@TrickyPi)
- [#5783](https://github.com/rollup/rollup/pull/5783): Improve CI caching for node_modules (@lukastaegert)

## 4.29.2

_2025-01-05_

### Bug Fixes

- Keep import attributes when using dynamic ESM `import()` expressions from CommonJS (#5781)

### Pull Requests

- [#5772](https://github.com/rollup/rollup/pull/5772): Improve caching on CI (@lukastaegert)
- [#5773](https://github.com/rollup/rollup/pull/5773): fix(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5780](https://github.com/rollup/rollup/pull/5780): feat: use picocolors instead of colorette (@re-taro)
- [#5781](https://github.com/rollup/rollup/pull/5781): fix: keep import attributes for cjs format (@TrickyPi)

## 4.29.1

_2024-12-21_

### Bug Fixes

- Fix crash from deoptimized logical expressions (#5771)

### Pull Requests

- [#5769](https://github.com/rollup/rollup/pull/5769): Remove unnecessary lifetimes (@lukastaegert)
- [#5771](https://github.com/rollup/rollup/pull/5771): fix: do not optimize the literal value if the cache is deoptimized (@TrickyPi)

## 4.29.0

_2024-12-20_

### Features

- Treat objects as truthy and always check second argument to better simplify logical expressions (#5763)

### Pull Requests

- [#5759](https://github.com/rollup/rollup/pull/5759): docs: add utf-8 encoding to JSON file reading (@chouchouji)
- [#5760](https://github.com/rollup/rollup/pull/5760): fix(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5763](https://github.com/rollup/rollup/pull/5763): fix: introduce UnknownFalsyValue for enhancing if statement tree-shaking (@TrickyPi)
- [#5766](https://github.com/rollup/rollup/pull/5766): chore(deps): update dependency @rollup/plugin-node-resolve to v16 (@renovate[bot])
- [#5767](https://github.com/rollup/rollup/pull/5767): fix(deps): lock file maintenance minor/patch updates (@renovate[bot])

## 4.28.1

_2024-12-06_

### Bug Fixes

- Support running Rollup natively on LoongArch (#5749)
- Add optional `debugId` to `SourceMap` types (#5751)

### Pull Requests

- [#5749](https://github.com/rollup/rollup/pull/5749): feat: add support for LoongArch (@darkyzhou)
- [#5751](https://github.com/rollup/rollup/pull/5751): feat: Add `debugId` to `SourceMap` types (@timfish, @lukastaegert)
- [#5752](https://github.com/rollup/rollup/pull/5752): chore(deps): update dependency mocha to v11 (@renovate[bot])
- [#5753](https://github.com/rollup/rollup/pull/5753): chore(deps): update dependency vite to v6 (@renovate[bot])
- [#5754](https://github.com/rollup/rollup/pull/5754): fix(deps): update swc monorepo (major) (@renovate[bot])
- [#5755](https://github.com/rollup/rollup/pull/5755): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5756](https://github.com/rollup/rollup/pull/5756): Test if saving the Cargo cache can speed up FreeBSD (@lukastaegert)

## 4.28.0

_2024-11-30_

### Features

- Allow to specify how to handle import attributes when transpiling Rollup config files (#5743)

### Pull Requests

- [#5743](https://github.com/rollup/rollup/pull/5743): fix: supports modify the import attributes key in the config file (@TrickyPi, @lukastaegert)
- [#5747](https://github.com/rollup/rollup/pull/5747): chore(deps): update codecov/codecov-action action to v5 (@renovate[bot])
- [#5748](https://github.com/rollup/rollup/pull/5748): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])

## 4.27.4

_2024-11-23_

### Bug Fixes

- Update bundled magic-string to support sourcemap debug ids (#5740)

### Pull Requests

- [#5740](https://github.com/rollup/rollup/pull/5740): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])

## 4.27.3

_2024-11-18_

### Bug Fixes

- Revert object property tree-shaking for now (#5736)

### Pull Requests

- [#5736](https://github.com/rollup/rollup/pull/5736): Revert object tree-shaking until some issues have been resolved (@lukastaegert)

## 4.27.2

_2024-11-15_

### Bug Fixes

- Ensure unused variables in patterns are always deconflicted if rendered (#5728)

### Pull Requests

- [#5728](https://github.com/rollup/rollup/pull/5728): Fix more variable deconflicting issues (@lukastaegert)

## 4.27.1

_2024-11-15_

### Bug Fixes

- Fix some situations where parameter declarations could put Rollup into an infinite loop (#5727)

### Pull Requests

- [#5727](https://github.com/rollup/rollup/pull/5727): Debug out-of-memory issues with Rollup v4.27.0 (@lukastaegert)

## 4.27.0

_2024-11-15_

### Features

- Tree-shake unused properties in object literals (#5420)

### Bug Fixes

- Change hash length limit to 21 to avoid inconsistent hash length (#5423)

### Pull Requests

- [#5420](https://github.com/rollup/rollup/pull/5420): feat: implement object tree-shaking (@TrickyPi, @lukastaegert)
- [#5723](https://github.com/rollup/rollup/pull/5723): Reduce max hash size to 21 (@lukastaegert)
- [#5724](https://github.com/rollup/rollup/pull/5724): fix(deps): update swc monorepo (major) (@renovate[bot])
- [#5725](https://github.com/rollup/rollup/pull/5725): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])

## 4.26.0

_2024-11-13_

### Features

- Allow to avoid `await bundle.close()` via explicit resource management in TypeScript (#5721)

### Pull Requests

- [#5721](https://github.com/rollup/rollup/pull/5721): feat: support `using` for `RollupBuild` (@shulaoda)

## 4.25.0

_2024-11-09_

### Features

- Add `output.sourcemapDebugIds` option to add matching debug ids to sourcemaps and code for tools like Sentry or Rollbar (#5712)

### Bug Fixes

- Make it easier to manually reproduce base16 hashes by using a more standard base16 conversion algorithm (#5719)

### Pull Requests

- [#5712](https://github.com/rollup/rollup/pull/5712): feat: Add support for injecting Debug IDs (@timfish)
- [#5717](https://github.com/rollup/rollup/pull/5717): fix(deps): update swc monorepo (major) (@renovate[bot])
- [#5718](https://github.com/rollup/rollup/pull/5718): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5719](https://github.com/rollup/rollup/pull/5719): Use a less surprising base-16 encoding (@lukastaegert)

## 4.24.4

_2024-11-04_

### Bug Fixes

- Ensure mutations by handlers in Proxy definitions are always respected when tree-shaking (#5713)

### Pull Requests

- [#5708](https://github.com/rollup/rollup/pull/5708): Update configuration-options document (@sacru2red, @lukastaegert)
- [#5711](https://github.com/rollup/rollup/pull/5711): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5713](https://github.com/rollup/rollup/pull/5713): fix: Deoptimize the proxied object if its property is reassigned in the handler functions (@TrickyPi)

## 4.24.3

_2024-10-29_

### Bug Fixes

- Slightly reduce memory consumption by specifying fixed array sizes where possible (#5703)

### Pull Requests

- [#5703](https://github.com/rollup/rollup/pull/5703): perf: use pre-allocated arrays for known result sizes (@GalacticHypernova)

## 4.24.2

_2024-10-27_

### Bug Fixes

- Add missing build dependency (#5705)

### Pull Requests

- [#5705](https://github.com/rollup/rollup/pull/5705): Fix "Couldn't find package" error when installing rollup using yarn (@tagattie)

## 4.24.1

_2024-10-27_

### Bug Fixes

- Support running Rollup natively on FreeBSD (#5698)

### Pull Requests

- [#5689](https://github.com/rollup/rollup/pull/5689): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5690](https://github.com/rollup/rollup/pull/5690): chore(deps): update dependency @inquirer/prompts to v7 (@renovate[bot])
- [#5691](https://github.com/rollup/rollup/pull/5691): chore(deps): update dependency eslint-plugin-unicorn to v56 (@renovate[bot])
- [#5692](https://github.com/rollup/rollup/pull/5692): chore(deps): lock file maintenance minor/patch updates (@renovate[bot], @lukastaegert)
- [#5695](https://github.com/rollup/rollup/pull/5695): fix(deps): update swc monorepo (major) (@renovate[bot])
- [#5696](https://github.com/rollup/rollup/pull/5696): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5698](https://github.com/rollup/rollup/pull/5698): Add support for FreeBSD (x64 and arm64) (@tagattie, @lukastaegert)

## 4.24.0

_2024-10-02_

### Features

- Support preserving and transpiling JSX syntax (#5668)

### Pull Requests

- [#5668](https://github.com/rollup/rollup/pull/5668): Introduce JSX support (@lukastaegert, @Martin-Idel, @felixhuttmann, @AlexDroll, @tiptr)

## 4.23.0

_2024-10-01_

### Features

- Collect all emitted names and originalFileNames for assets (#5686)

### Pull Requests

- [#5686](https://github.com/rollup/rollup/pull/5686): Add names and originalFileNames to assets (@lukastaegert)

## 4.22.5

_2024-09-27_

### Bug Fixes

- Allow parsing of certain unicode characters again (#5674)

### Pull Requests

- [#5674](https://github.com/rollup/rollup/pull/5674): Fix panic with unicode characters (@sapphi-red, @lukastaegert)
- [#5675](https://github.com/rollup/rollup/pull/5675): chore(deps): update dependency rollup to v4.22.4 [security] (@renovate[bot])
- [#5680](https://github.com/rollup/rollup/pull/5680): chore(deps): update dependency @rollup/plugin-commonjs to v28 (@renovate[bot], @lukastaegert)
- [#5681](https://github.com/rollup/rollup/pull/5681): chore(deps): update dependency @rollup/plugin-replace to v6 (@renovate[bot])
- [#5682](https://github.com/rollup/rollup/pull/5682): chore(deps): update dependency @rollup/plugin-typescript to v12 (@renovate[bot])
- [#5684](https://github.com/rollup/rollup/pull/5684): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])

## 2.79.2

_2024-09-26_

### Bug Fixes

- Fix a vulnerability in generated code that affects IIFE, UMD and CJS bundles when run in a browser context (#5671)

### Pull Requests

- [#5671](https://github.com/rollup/rollup/pull/5671): Fix DOM Clobbering CVE (@lukastaegert)

## 3.29.5

_2024-09-21_

### Bug Fixes

- Fix a vulnerability in generated code that affects IIFE, UMD and CJS bundles when run in a browser context (#5671)

### Pull Requests

- [#5671](https://github.com/rollup/rollup/pull/5671): Fix DOM Clobbering CVE (@lukastaegert)

## 4.22.4

_2024-09-21_

### Bug Fixes

- Fix a vulnerability in generated code that affects IIFE, UMD and CJS bundles when run in a browser context (#5671)

### Pull Requests

- [#5670](https://github.com/rollup/rollup/pull/5670): refactor: Use object.prototype to check for reserved properties (@YuHyeonWook)
- [#5671](https://github.com/rollup/rollup/pull/5671): Fix DOM Clobbering CVE (@lukastaegert)

## 4.22.3

_2024-09-21_

### Bug Fixes

- Ensure that mutations in modules without side effects are observed while properly handling transitive dependencies (#5669)

### Pull Requests

- [#5669](https://github.com/rollup/rollup/pull/5669): Ensure impure dependencies of pure modules are added (@lukastaegert)

## 4.22.2

_2024-09-20_

### Bug Fixes

- Revert fix for side effect free modules until other issues are investigated (#5667)

### Pull Requests

- [#5667](https://github.com/rollup/rollup/pull/5667): Partially revert #5658 and re-apply #5644 (@lukastaegert)

## 4.22.1

_2024-09-20_

### Bug Fixes

- Revert #5644 "stable chunk hashes" while issues are being investigated

### Pull Requests

- [#5663](https://github.com/rollup/rollup/pull/5663): chore(deps): update dependency inquirer to v11 (@renovate[bot], @lukastaegert)
- [#5664](https://github.com/rollup/rollup/pull/5664): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5665](https://github.com/rollup/rollup/pull/5665): fix: type in CI file (@YuHyeonWook)
- [#5666](https://github.com/rollup/rollup/pull/5666): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])

## 4.22.0

_2024-09-19_

### Features

- Add additional known global values to avoid access side effects (#5651)

### Bug Fixes

- Ensure deterministic chunk hash generation despite async renderChunk hook (#5644)
- Improve side effect detection when using "smallest" treeshaking preset when imports are optimized away (#5658)

### Pull Requests

- [#5644](https://github.com/rollup/rollup/pull/5644): fix: apply final hashes deterministically with stable placeholders set (@mattkubej, @lukastaegert)
- [#5646](https://github.com/rollup/rollup/pull/5646): chore(deps): update dependency @mermaid-js/mermaid-cli to v11 (@renovate[bot])
- [#5647](https://github.com/rollup/rollup/pull/5647): chore(deps): update dependency concurrently to v9 (@renovate[bot])
- [#5648](https://github.com/rollup/rollup/pull/5648): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5651](https://github.com/rollup/rollup/pull/5651): feat: add `AggregateError`, `FinalizationRegistry`, `WeakRef` to knownGlobals (@re-taro)
- [#5653](https://github.com/rollup/rollup/pull/5653): Fix example selection in REPL (@lukastaegert)
- [#5657](https://github.com/rollup/rollup/pull/5657): chore(deps): update dependency vite to v5.4.6 [security] (@renovate[bot])
- [#5658](https://github.com/rollup/rollup/pull/5658): Detect variable reassignments in modules without side effects (@lukastaegert)

## 4.21.3

_2024-09-12_

### Bug Fixes

- Always respect side effects in left-hand side of optional chain (#5642)
- Update stack trace for augmented errors to not hide relevant information (#5640)

### Pull Requests

- [#5636](https://github.com/rollup/rollup/pull/5636): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5637](https://github.com/rollup/rollup/pull/5637): chore(deps): lock file maintenance (@renovate[bot])
- [#5640](https://github.com/rollup/rollup/pull/5640): fix: keep the message of stack up-to-date (@TrickyPi)
- [#5642](https://github.com/rollup/rollup/pull/5642): fix: include left-side effect of optional chaining in the end of hasEffectsAsChainElement (@TrickyPi)

## 4.21.2

_2024-08-30_

### Bug Fixes

- Handle IIFE/UMD namespace definitions conflicting with a builtin property (#5605)

### Pull Requests

- [#5605](https://github.com/rollup/rollup/pull/5605): fix: Wrong namespace property definition (@thirumurugan-git, @lukastaegert)
- [#5630](https://github.com/rollup/rollup/pull/5630): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5631](https://github.com/rollup/rollup/pull/5631): chore(deps): lock file maintenance (@renovate[bot])
- [#5632](https://github.com/rollup/rollup/pull/5632): chore(deps): lock file maintenance (@renovate[bot])

## 4.21.1

_2024-08-26_

### Bug Fixes

- Ensure `closeWatcher` hook is called when watch mode is aborted via Ctrl+C (#5618)
- Do not produce invalid code for `import.meta.url` in compact mode (#5624)
- Do not throw when generating chunk names when preserving modules in Windows (#5625)

### Pull Requests

- [#5591](https://github.com/rollup/rollup/pull/5591): chore(deps): update dependency @types/eslint to v9 (@renovate[bot], @lukastaegert)
- [#5618](https://github.com/rollup/rollup/pull/5618): preload the WASM file even though the version is undefined. (@TrickyPi)
- [#5619](https://github.com/rollup/rollup/pull/5619): Call and await closeWatcher hooks on exit signals (@lukastaegert)
- [#5622](https://github.com/rollup/rollup/pull/5622): chore(deps): lock file maintenance minor/patch updates (@renovate[bot], @lukastaegert)
- [#5624](https://github.com/rollup/rollup/pull/5624): fix: add space for DOCUMENT_CURRENT_SCRIPT template (@TrickyPi)
- [#5625](https://github.com/rollup/rollup/pull/5625): fix: get the right chunk name for preserve modules in Windows (@TrickyPi, @lukastaegert)

## 4.21.0

_2024-08-18_

### Features

- Add option to configure directory for virtual modules when preserving modules (#5602)

### Pull Requests

- [#5602](https://github.com/rollup/rollup/pull/5602): feat: introduce the virtualDirname option to customize the virtual directory name (@TrickyPi)
- [#5607](https://github.com/rollup/rollup/pull/5607): chore(deps): update typescript-eslint monorepo to v8 (major) (@renovate[bot], @lukastaegert)
- [#5608](https://github.com/rollup/rollup/pull/5608): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5611](https://github.com/rollup/rollup/pull/5611): chore: fix the `noConflict` option in REPL. (@7086cmd)
- [#5613](https://github.com/rollup/rollup/pull/5613): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5614](https://github.com/rollup/rollup/pull/5614): chore(deps): lock file maintenance (@renovate[bot])

## 4.20.0

_2024-08-03_

### Features

- Allow plugins to specify the original file name when emitting assets (#5596)

### Pull Requests

- [#5596](https://github.com/rollup/rollup/pull/5596): Add originalFIleName property to emitted assets (@lukastaegert)
- [#5599](https://github.com/rollup/rollup/pull/5599): chore(deps): update dependency eslint-plugin-unicorn to v55 (@renovate[bot], @lukastaegert)
- [#5600](https://github.com/rollup/rollup/pull/5600): chore(deps): lock file maintenance minor/patch updates (@renovate[bot], @lukastaegert)

## 4.19.2

_2024-08-01_

### Bug Fixes

- Avoid "cannot get value of null" error when using optional chaining with namespaces (#5597)

### Pull Requests

- [#5597](https://github.com/rollup/rollup/pull/5597): Fix retrieval of literal values for chained namespaces (@lukastaegert)

## 4.19.1

_2024-07-27_

### Bug Fixes

- Do not remove parantheses when tree-shaking logical expressions (#5584)
- Do not ignore side effects in calls left of an optional chaining operator (#5589)

### Pull Requests

- [#5584](https://github.com/rollup/rollup/pull/5584): fix: find whitespace from operator position to start (@TrickyPi)
- [#5587](https://github.com/rollup/rollup/pull/5587): docs: improve command by code-group (@thinkasany, @lukastaegert)
- [#5589](https://github.com/rollup/rollup/pull/5589): Fix side effect detection in optional chains (@lukastaegert)
- [#5592](https://github.com/rollup/rollup/pull/5592): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5593](https://github.com/rollup/rollup/pull/5593): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5594](https://github.com/rollup/rollup/pull/5594): chore(deps): lock file maintenance (@renovate[bot])
- [#5595](https://github.com/rollup/rollup/pull/5595): chore(deps): lock file maintenance (@renovate[bot])

## 4.19.0

_2024-07-20_

### Features

- Implement support for decorators (#5562)

### Bug Fixes

- Improve soucemap generation when tree-shaking logical expressions (#5581)

### Pull Requests

- [#5562](https://github.com/rollup/rollup/pull/5562): feat: implementing decorator support (@TrickyPi, @lukastaegert)
- [#5570](https://github.com/rollup/rollup/pull/5570): refactor(finalisers): condition branch (@Simon-He95, @zhangmo8)
- [#5572](https://github.com/rollup/rollup/pull/5572): Improve chunk and asset type information in docs (@lukastaegert)
- [#5573](https://github.com/rollup/rollup/pull/5573): Switch to audit resolver to ignore requirejs vulnerability (@lukastaegert)
- [#5575](https://github.com/rollup/rollup/pull/5575): chore(deps): update dependency inquirer to v10 (@renovate[bot], @lukastaegert)
- [#5576](https://github.com/rollup/rollup/pull/5576): chore(deps): lock file maintenance minor/patch updates (@renovate[bot], @lukastaegert)
- [#5580](https://github.com/rollup/rollup/pull/5580): chore(deps): lock file maintenance minor/patch updates (@renovate[bot], @lukastaegert)
- [#5581](https://github.com/rollup/rollup/pull/5581): When tree-shaking logical expression, make sure to remove all trailing white-space. (@lukastaegert)

## 4.18.1

_2024-07-08_

### Bug Fixes

- Prevent "%" in generated file names to ensure imports resolve (#5535)

### Pull Requests

- [#5524](https://github.com/rollup/rollup/pull/5524): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5525](https://github.com/rollup/rollup/pull/5525): chore(deps): lock file maintenance (@renovate[bot])
- [#5526](https://github.com/rollup/rollup/pull/5526): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5527](https://github.com/rollup/rollup/pull/5527): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5529](https://github.com/rollup/rollup/pull/5529): Use Spanned trait to simplify logic (@lukastaegert)
- [#5530](https://github.com/rollup/rollup/pull/5530): Fix typos in ARCHITECTURE.md (@younggglcy)
- [#5532](https://github.com/rollup/rollup/pull/5532): Use Rust macros for converters where possible (@lukastaegert)
- [#5535](https://github.com/rollup/rollup/pull/5535): fix: escape `%` if URI malformed (@baseballyama, @lukastaegert)
- [#5536](https://github.com/rollup/rollup/pull/5536): chore(deps): lock file maintenance minor/patch updates (@renovate[bot], @lukastaegert)
- [#5541](https://github.com/rollup/rollup/pull/5541): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5542](https://github.com/rollup/rollup/pull/5542): chore(deps): lock file maintenance (@renovate[bot])
- [#5543](https://github.com/rollup/rollup/pull/5543): Watch rust files and rebuild during dev (@lukastaegert)
- [#5544](https://github.com/rollup/rollup/pull/5544): Refactor AST converters (@lukastaegert)
- [#5545](https://github.com/rollup/rollup/pull/5545): chore(deps): update dependency @rollup/plugin-commonjs to v26 (@renovate[bot])
- [#5546](https://github.com/rollup/rollup/pull/5546): chore(deps): update dependency nyc to v17 (@renovate[bot])
- [#5547](https://github.com/rollup/rollup/pull/5547): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5548](https://github.com/rollup/rollup/pull/5548): chore(deps): lock file maintenance (@renovate[bot])
- [#5549](https://github.com/rollup/rollup/pull/5549): chore(deps): lock file maintenance (@renovate[bot])
- [#5550](https://github.com/rollup/rollup/pull/5550): chore(deps): update dependency eslint-plugin-unicorn to v54 (@renovate[bot], @lukastaegert)
- [#5551](https://github.com/rollup/rollup/pull/5551): chore(deps): lock file maintenance minor/patch updates (@renovate[bot], @lukastaegert)
- [#5555](https://github.com/rollup/rollup/pull/5555): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5556](https://github.com/rollup/rollup/pull/5556): chore(deps): lock file maintenance (@renovate[bot])
- [#5558](https://github.com/rollup/rollup/pull/5558): Consider that the body of ClassBody might be of type StaticBlock (@TrickyPi)
- [#5565](https://github.com/rollup/rollup/pull/5565): refactor(ast): conditional branch (@Simon-He95)
- [#5566](https://github.com/rollup/rollup/pull/5566): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5567](https://github.com/rollup/rollup/pull/5567): chore(deps): lock file maintenance (@renovate[bot])

## 4.18.0

_2024-05-22_

### Features

- Resolve import.meta.filename and .dirname in transpiled plugins (#5520)

### Pull Requests

- [#5504](https://github.com/rollup/rollup/pull/5504): Auto generate node index (@lukastaegert)
- [#5507](https://github.com/rollup/rollup/pull/5507): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5508](https://github.com/rollup/rollup/pull/5508): chore(deps): lock file maintenance (@renovate[bot])
- [#5510](https://github.com/rollup/rollup/pull/5510): Split up converter.rs into AST nodes (@lukastaegert)
- [#5512](https://github.com/rollup/rollup/pull/5512): chore(deps): update dependency builtin-modules to v4 (@renovate[bot], @lukastaegert)
- [#5514](https://github.com/rollup/rollup/pull/5514): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5518](https://github.com/rollup/rollup/pull/5518): chore(deps): update dependency eslint-plugin-unicorn to v53 (@renovate[bot], @lukastaegert)
- [#5519](https://github.com/rollup/rollup/pull/5519): chore(deps): lock file maintenance minor/patch updates (@renovate[bot], @lukastaegert)
- [#5520](https://github.com/rollup/rollup/pull/5520): Resolve import.meta.{filename,dirname} in files imported from config (@BPScott)
- [#5521](https://github.com/rollup/rollup/pull/5521): docs: correct base32 to base36 in documentation (@highcastlee)

## 4.17.2

_2024-04-30_

### Bug Fixes

- Fix tree-shaking problems when using spread arguments (#5503)

### Pull Requests

- [#5501](https://github.com/rollup/rollup/pull/5501): Slightly improve perf report (@lukastaegert)
- [#5503](https://github.com/rollup/rollup/pull/5503): fix: rest element should deoptimize parameter values (@liuly0322)

## 4.17.1

_2024-04-29_

### Bug Fixes

- Prevent infinite recursions for certain constructor invocations (#5500)

### Pull Requests

- [#5500](https://github.com/rollup/rollup/pull/5500): fix: parameter variable infinite recursion error (@liuly0322)

## 4.17.0

_2024-04-27_

### Features

- Track function call arguments to optimize functions only called once or with the same literal values (re-release from 4.16.0) (#5483)

### Bug Fixes

- Reduce browser WASM size to a fraction by changing optimization settings (#5494)

### Pull Requests

- [#5483](https://github.com/rollup/rollup/pull/5483): feature(fix): function parameter tracking (@liuly0322)
- [#5488](https://github.com/rollup/rollup/pull/5488): Report performance in CI (@TrickyPi)
- [#5489](https://github.com/rollup/rollup/pull/5489): Create FUNDING.json (@BenJam)
- [#5492](https://github.com/rollup/rollup/pull/5492): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5493](https://github.com/rollup/rollup/pull/5493): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5494](https://github.com/rollup/rollup/pull/5494): Use opt-level=z for browser wasm (@sapphi-red)

## 4.16.4

_2024-04-23_

### Bug Fixes

- Revert function parameter tracking logic introduced in 4.16.0 to work on some remaining issues (#5487)

### Pull Requests

- [#5487](https://github.com/rollup/rollup/pull/5487): Revert function parameter tracking logic for now (@lukastaegert)

## 4.16.3

_2024-04-23_

### Bug Fixes

- Do not optimize IIFEs that have a name and are again referenced inside their definition (#5486)

### Pull Requests

- [#5486](https://github.com/rollup/rollup/pull/5486): fix: only optimize annoymous iife (@liuly0322)

## 4.16.2

_2024-04-22_

### Bug Fixes

- Resolve a situation condition where reassignments of function parameters were not tracked properly (#5482)
- Make sure that for armv7 packages, only one package is downloaded for the user (musl or gnu) (#5479)

### Pull Requests

- [#5479](https://github.com/rollup/rollup/pull/5479): Add libc field to armv7 packages (@sapphi-red)
- [#5482](https://github.com/rollup/rollup/pull/5482): fix: function parameter reassigned update (@liuly0322)

## 4.16.1

_2024-04-21_

### Bug Fixes

- Fix crash when rendering logical or conditional expressions (#5481)

### Pull Requests

- [#5481](https://github.com/rollup/rollup/pull/5481): fix: conditional/logical expression should request a new tree-shaking (@liuly0322)

## 4.16.0

_2024-04-21_

### Features

- Track function call arguments to optimize functions only called once or with the same literal values (#5443)

### Pull Requests

- [#5443](https://github.com/rollup/rollup/pull/5443): feat: improve tree-shaking by propagate const parameter (@liuly0322, @lukastaegert)

## 4.15.0

_2024-04-20_

### Features

- Add output.importAttributesKey option to select whether to use "with" or "assert" for import attributes (#5474)

### Pull Requests

- [#5474](https://github.com/rollup/rollup/pull/5474): Add ImportAttributesKey to choose keyword ("with" | "assert") (@doubleaa93, @lukastaegert)
- [#5475](https://github.com/rollup/rollup/pull/5475): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5477](https://github.com/rollup/rollup/pull/5477): Try to run emulated smoke tests for Linux environments (@lukastaegert)

## 4.14.3

_2024-04-15_

### Bug Fixes

- Support Alpine Linux and other MUSL builds on ARM (#5471)

### Pull Requests

- [#5471](https://github.com/rollup/rollup/pull/5471): Add linux arm musl build (@sapphi-red)

## 4.14.2

_2024-04-12_

### Bug Fixes

- Do not create invalid code when reexporting both a namespace and the default export from that namespace (#5466)
- Ensure ppc64 platform is properly detected (#5460)

### Pull Requests

- [#5456](https://github.com/rollup/rollup/pull/5456): Add high-level architecture documentation (@lukastaegert)
- [#5460](https://github.com/rollup/rollup/pull/5460): Fix ppc64le target (@lukastaegert)
- [#5463](https://github.com/rollup/rollup/pull/5463): chore: tweak the comment about files should not be edited (@TrickyPi)
- [#5466](https://github.com/rollup/rollup/pull/5466): Ensure reexported namespaces do not prevent creation of default export helpers (@lukastaegert)
- [#5468](https://github.com/rollup/rollup/pull/5468): chore(deps): update dependency eslint-plugin-unicorn to v52 (@renovate[bot], @lukastaegert)
- [#5469](https://github.com/rollup/rollup/pull/5469): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5470](https://github.com/rollup/rollup/pull/5470): chore(deps): lock file maintenance (@renovate[bot])

## 4.14.1

_2024-04-07_

### Bug Fixes

- Show better error when running on musl Linux where the musl build is not supported (#5454)

### Pull Requests

- [#5451](https://github.com/rollup/rollup/pull/5451): chore: generate string constants from config (@TrickyPi)
- [#5452](https://github.com/rollup/rollup/pull/5452): chore(deps): lock file maintenance minor/patch updates (@renovate[bot])
- [#5453](https://github.com/rollup/rollup/pull/5453): chore(deps): lock file maintenance (@renovate[bot])
- [#5454](https://github.com/rollup/rollup/pull/5454): Improve error message when running on unsupported MUSL Linux (@lukastaegert)
- [#5455](https://github.com/rollup/rollup/pull/5455): Remove inlining logic in AST (de-)serializer (@lukastaegert)

## 4.14.0

_2024-04-03_

### Features

- Display error causes in Rollup CLI (#5422)
- Add basic support for explicit resource management via "using" and "await using" (#5423)

### Pull Requests

- [#5422](https://github.com/rollup/rollup/pull/5422): feat: show all cause in Error (@devohda, @lukastaegert)
- [#5444](https://github.com/rollup/rollup/pull/5444): feat: support explicit-resource-management (@TrickyPi)
- [#5445](https://github.com/rollup/rollup/pull/5445): docs: add `@shikiji/vitepress-twoslash` (@sapphi-red)
- [#5447](https://github.com/rollup/rollup/pull/5447): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5448](https://github.com/rollup/rollup/pull/5448): chore(deps): lock file maintenance (@renovate[bot])

## 4.13.2

_2024-03-28_

### Bug Fixes

- Ensure accessing module info is cached after the build phase for improved performance (#5438)
- Support powerpc64le CPUs (#5350)

### Pull Requests

- [#5350](https://github.com/rollup/rollup/pull/5350): Add support for ppc64le (@pavolloffay, @lukastaegert)
- [#5438](https://github.com/rollup/rollup/pull/5438): Cache module info getters before output generation (@bluwy, @lukastaegert)

## 4.13.1

_2024-03-27_

### Bug Fixes

- Add new linux-s390x-gnu native binary package (#5346)

### Pull Requests

- [#5346](https://github.com/rollup/rollup/pull/5346): Add support for linux s390x gnu (@edlerd)
- [#5430](https://github.com/rollup/rollup/pull/5430): chore(deps): update dependency @vue/eslint-config-typescript to v13 (@renovate[bot], @lukastaegert)
- [#5431](https://github.com/rollup/rollup/pull/5431): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5432](https://github.com/rollup/rollup/pull/5432): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5436](https://github.com/rollup/rollup/pull/5436): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5437](https://github.com/rollup/rollup/pull/5437): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])

## 4.13.0

_2024-03-12_

### Features

- Ensure that the location of parse errors and other logs is encoded in the error message as well (#5424)

### Pull Requests

- [#5417](https://github.com/rollup/rollup/pull/5417): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5418](https://github.com/rollup/rollup/pull/5418): chore(deps): lock file maintenance (@renovate[bot])
- [#5419](https://github.com/rollup/rollup/pull/5419): chore: fix typo (@OnlyWick)
- [#5424](https://github.com/rollup/rollup/pull/5424): Add locations to logs, warnings and error messages ( @lukastaegert)

## 4.12.1

_2024-03-06_

### Bug Fixes

- Escape special characters in file references (#5404)

### Pull Requests

- [#5398](https://github.com/rollup/rollup/pull/5398): Rename `getRollupEror` to `getRollupError` (@MrRefactoring)
- [#5399](https://github.com/rollup/rollup/pull/5399): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5404](https://github.com/rollup/rollup/pull/5404): fix: escape ids in `import.meta.ROLLUP_FILE_URL_referenceId` correctly (@sapphi-red)
- [#5406](https://github.com/rollup/rollup/pull/5406): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5407](https://github.com/rollup/rollup/pull/5407): chore(deps): lock file maintenance (@renovate[bot])
- [#5411](https://github.com/rollup/rollup/pull/5411): Chunk assignment - Fix comment line breaks and typo (@yoavweiss, @lukastaegert)

## 4.12.0

_2024-02-16_

### Features

- Improve raw bundling performance by 10-15% when not using the cache or plugins that return an AST (#5391)

### Pull Requests

- [#5391](https://github.com/rollup/rollup/pull/5391): Improve performance by directly constructing AST from buffer ( @lukastaegert)
- [#5393](https://github.com/rollup/rollup/pull/5393): chore(deps): update dependency eslint-plugin-unicorn to v51 ( @renovate[bot])
- [#5394](https://github.com/rollup/rollup/pull/5394): chore(deps): update typescript-eslint monorepo to v7 (major) ( @renovate[bot])
- [#5395](https://github.com/rollup/rollup/pull/5395): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])

## 4.11.0

_2024-02-15_

### Features

- Add `output.reexportProtoFromExternal` option to disable special code for handling `__proto__` reexports (#5380)

### Bug Fixes

- Ensure namespace reexport code can be parsed by cjs-module-lexer (#5380)
- Throw when trying to reassing `const` variables (#5388)

### Pull Requests

- [#5380](https://github.com/rollup/rollup/pull/5380): fix: separately export `__proto__` for compatibility with CJS Transpiler Re-exports (@TrickyPi)
- [#5388](https://github.com/rollup/rollup/pull/5388): Add const reassign rule (@TrickyPi)

## 4.10.0

_2024-02-10_

### Features

- Support base-36 and base-16 hashes again via new `output.hashCharacters` option (#5371)

### Bug Fixes

- Do not crash process for panics in native code but throw them as JavaScript errors (#5383)

### Pull Requests

- [#5359](https://github.com/rollup/rollup/pull/5359): chore(deps): update actions/cache action to v4 (@renovate[bot])
- [#5360](https://github.com/rollup/rollup/pull/5360): chore(deps): update dependency pretty-ms to v9 (@renovate[bot])
- [#5366](https://github.com/rollup/rollup/pull/5366): chore(deps): update dependency husky to v9 (@renovate[bot])
- [#5367](https://github.com/rollup/rollup/pull/5367): chore(deps): update peter-evans/create-or-update-comment action to v4 (@renovate[bot])
- [#5368](https://github.com/rollup/rollup/pull/5368): chore(deps): update peter-evans/find-comment action to v3 ( @renovate[bot])
- [#5369](https://github.com/rollup/rollup/pull/5369): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5370](https://github.com/rollup/rollup/pull/5370): Fix dependency range for Node types (@lukastaegert)
- [#5371](https://github.com/rollup/rollup/pull/5371): Implement "output.hashCharacters" option to define character set for file hashes (@lukastaegert)
- [#5372](https://github.com/rollup/rollup/pull/5372): Roll back vitepress as 1.0.0-rc.40 breaks the development build ( @lukastaegert)
- [#5382](https://github.com/rollup/rollup/pull/5382): Update documentation (@TrickyPi)
- [#5383](https://github.com/rollup/rollup/pull/5383): Catch Rust panics and then throw them in JS (@TrickyPi)
- [#5384](https://github.com/rollup/rollup/pull/5384): chore(deps): update codecov/codecov-action action to v4 ( @renovate[bot])
- [#5385](https://github.com/rollup/rollup/pull/5385): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5386](https://github.com/rollup/rollup/pull/5386): Resolve all rollup imports to node_modules to avoid type conflict (@TrickyPi)

## 4.9.6

_2024-01-21_

### Bug Fixes

- Detect side effects when an element that was pushed into an array is modified via the array (#5352)

### Pull Requests

- [#5337](https://github.com/rollup/rollup/pull/5337): Generate AST transformers from config (@lukastaegert)
- [#5340](https://github.com/rollup/rollup/pull/5340): Also type-check d.ts files (@lukastaegert)
- [#5348](https://github.com/rollup/rollup/pull/5348): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5351](https://github.com/rollup/rollup/pull/5351): chore(deps): update dependency vite to v5.0.12 [security] ( @renovate[bot])
- [#5352](https://github.com/rollup/rollup/pull/5352): Track mutations of elements pushed into arrays (@lukastaegert)

## 4.9.5

_2024-01-12_

### Bug Fixes

- Fix issue where on Windows, Rollup would not load due to problems with the MSVC executable (#5335)

### Pull Requests

- [#5334](https://github.com/rollup/rollup/pull/5334): Fix typo in commondir.ts (@akiomik)
- [#5335](https://github.com/rollup/rollup/pull/5335): build: static link msvc runtime on Windows x64 platform ( @Brooooooklyn)
- [#5338](https://github.com/rollup/rollup/pull/5338): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])

## 4.9.4

_2024-01-06_

### Bug Fixes

- Use quotes for keys in namespaces that are only numbers but are not valid integers (#5328)
- Allow to have comments between pure annotations and the annoted node (#5332)

### Pull Requests

- [#5328](https://github.com/rollup/rollup/pull/5328): Correctly handling number key (@LongTengDao)
- [#5332](https://github.com/rollup/rollup/pull/5332): Handle pure annotations that are separated by a comment ( @lukastaegert)

## 4.9.3

_2024-01-05_

### Bug Fixes

- Support `__proto__` as export/import name (#5313)
- Use ESTree AST type over custom type in user-facing types (#5323)

### Pull Requests

- [#5313](https://github.com/rollup/rollup/pull/5313): Correctly handling **proto** export as module object key ( @LongTengDao)
- [#5323](https://github.com/rollup/rollup/pull/5323): fix: Add estree.Program type to rollup.d.ts (@TrickyPi)
- [#5326](https://github.com/rollup/rollup/pull/5326): docs: fix grammar (@gigabites19)
- [#5329](https://github.com/rollup/rollup/pull/5329): chore(deps): update dependency @vue/eslint-config-prettier to v9 (@renovate[bot])
- [#5330](https://github.com/rollup/rollup/pull/5330): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])

## 4.9.2

_2023-12-30_

### Bug Fixes

- Extend support for arbitrary namespace identifiers in SystemJS (#5321)
- Do not wrongly flag functions without side effects as side effects if moduleSideEffects is false (#5322)

### Pull Requests

- [#5305](https://github.com/rollup/rollup/pull/5305): Add JSDoc types to internal scripts (@lukastaegert)
- [#5309](https://github.com/rollup/rollup/pull/5309): chore(deps): update actions/download-artifact action to v4 ( @renovate[bot])
- [#5311](https://github.com/rollup/rollup/pull/5311): chode: add node badge (@btea)
- [#5312](https://github.com/rollup/rollup/pull/5312): Remove rollup-plugin-thatworks from devDeps (@TrickyPi)
- [#5318](https://github.com/rollup/rollup/pull/5318): chore(deps): update dependency eslint-plugin-unicorn to v50 ( @renovate[bot])
- [#5319](https://github.com/rollup/rollup/pull/5319): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5321](https://github.com/rollup/rollup/pull/5321): Handle arbitrary namespace identifiers in some SystemJS scenarios (@lukastaegert)
- [#5322](https://github.com/rollup/rollup/pull/5322): Do not handle declarations in modules without side effects as TDZ (@lukastaegert)

## 4.9.1

_2023-12-17_

### Bug Fixes

- Fix an issue where break statements could include the wrong label (#5297)

### Pull Requests

- [#5297](https://github.com/rollup/rollup/pull/5297): fix: use a new includedLabels in the body of the LabeledStatement (@TrickyPi)
- [#5300](https://github.com/rollup/rollup/pull/5300): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])

## 4.9.0

_2023-12-13_

### Features

- Fully support arbitrary strings as import and export identifiers (#5298)

### Pull Requests

- [#5296](https://github.com/rollup/rollup/pull/5296): Do not assume setTimeout return type (@kapouer)
- [#5298](https://github.com/rollup/rollup/pull/5298): Fully support arbitrary module namespace identifiers for all formats (@lukastaegert)

## 4.8.0

_2023-12-11_

### Features

- Improve `experimentalMinChunkSize` to take already loaded modules from dynamic imports into account (#5294)

### Pull Requests

- [#5294](https://github.com/rollup/rollup/pull/5294): Find more merge targets for experimentalMinChunkSize ( @lukastaegert)

## 4.7.0

_2023-12-08_

### Features

- Add build for Linux riscv64 architecture (#5288)

### Bug Fixes

- Improve error message when native Windows build does not start (#5284)

### Pull Requests

- [#5278](https://github.com/rollup/rollup/pull/5278): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5281](https://github.com/rollup/rollup/pull/5281): Add logs and experimentalLogSideEffects to REPL (@lukastaegert)
- [#5284](https://github.com/rollup/rollup/pull/5284): Add friendly error for missing MSVC redistributable (@sapphi-red)
- [#5285](https://github.com/rollup/rollup/pull/5285): chore(deps): update dependency vite to v5.0.5 [security] ( @renovate[bot])
- [#5288](https://github.com/rollup/rollup/pull/5288): Add support for linux riscv64 gnu (@kxxt)
- [#5290](https://github.com/rollup/rollup/pull/5290): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])

## 4.6.1

_2023-11-30_

### Bug Fixes

- Resolve a situation where declaring the same `var` several times was considered a conflict (#5276)

### Pull Requests

- [#5275](https://github.com/rollup/rollup/pull/5275): Add TNG as special sponsor (@lukastaegert)
- [#5276](https://github.com/rollup/rollup/pull/5276): Allow to redeclare parameters multiple times in nested scopes ( @lukastaegert)

## 4.6.0

_2023-11-26_

### Features

- Allow `this.addWatchFile` in all plugin hooks (#5270)

### Bug Fixes

- Show helpful error when native binaries are not installed due to an `npm` issue (#5267)
- Do not access `this` context in `this.addWatchFile` so it does not need to be bound when passed around (#5270)

### Pull Requests

- [#5267](https://github.com/rollup/rollup/pull/5267): Add friendly error for npm bug (@sapphi-red)
- [#5270](https://github.com/rollup/rollup/pull/5270): Allow this.addWatchFile in all hooks (@lukastaegert)
- [#5272](https://github.com/rollup/rollup/pull/5272): Debug deployed graphs (@lukastaegert)

## 4.5.2

_2023-11-24_

### Bug Fixes

- Handle files with UTF-8 BOM when using the commonjs plugin (#5268)

### Pull Requests

- [#5268](https://github.com/rollup/rollup/pull/5268): fix: strip BOM before calling transform hook (@TrickyPi)
- [#5269](https://github.com/rollup/rollup/pull/5269): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])

## 4.5.1

_2023-11-21_

### Bug Fixes

- Do not error when a function expression uses the same name for a parameter and its id (#5262)

### Pull Requests

- [#5257](https://github.com/rollup/rollup/pull/5257): Fix graphs in docs, improve REPL colors (@lukastaegert)
- [#5262](https://github.com/rollup/rollup/pull/5262): Allow function expression parameters to shadow the function id ( @lukastaegert)

## 4.5.0

_2023-11-18_

### Bug Fixes

- Show a proper error when using native Rollup on armv7 musl Linux (#5255)

### Pull Requests

- [#5251](https://github.com/rollup/rollup/pull/5251): doc fix import assertions to attributes in API plugin development page (@lhapaipai)
- [#5253](https://github.com/rollup/rollup/pull/5253): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5255](https://github.com/rollup/rollup/pull/5255): Error for armv7 musl build (@lukastaegert)

## 4.4.1

_2023-11-14_

### Bug Fixes

- Do not flag duplicate function declarations in function scopes as syntax errors (#5248)

### Pull Requests

- [#5248](https://github.com/rollup/rollup/pull/5248): Allow functions to redeclare vars and functions in function scopes (@lukastaegert)

## 4.4.0

_2023-11-12_

### Features

- Replace SWC linting with faster internal linting to error on duplicate declarations etc. (#5207)

### Bug Fixes

- Show proper error when an entry exports non-existing bindings (#5207)

### Pull Requests

- [#5207](https://github.com/rollup/rollup/pull/5207): perf: run lint while constructing nodes (@sapphi-red)

## 4.3.1

_2023-11-11_

### Bug Fixes

- Fix rename error when handling errors in watch mode (#5240)
- Prevent warning when using `--forceExit` (#5245)

### Pull Requests

- [#5240](https://github.com/rollup/rollup/pull/5240): fix: allow the name of Rollup Error to be modified (@TrickyPi)
- [#5243](https://github.com/rollup/rollup/pull/5243): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5245](https://github.com/rollup/rollup/pull/5245): Ensure --forceExit works without warning (@lukastaegert)

## 4.3.0

_2023-11-03_

### Features

- Add `forceExit` CLI flag for situations where the CLI does not exit gracefully (#5195)

### Bug Fixes

- Properly catch errors when removing a temporary config file fails (#5198)

### Pull Requests

- [#5195](https://github.com/rollup/rollup/pull/5195): Add `forceExit` CLI flag (@raphael-theriault-swi)
- [#5198](https://github.com/rollup/rollup/pull/5198): fix: prevent `ENOENT` error on temp config removal (@jzempel)
- [#5237](https://github.com/rollup/rollup/pull/5237): chore: remove unused files and deps (@TrickyPi)
- [#5238](https://github.com/rollup/rollup/pull/5238): chore(deps): update dependency eslint-plugin-unicorn to v49 ( @renovate[bot])
- [#5239](https://github.com/rollup/rollup/pull/5239): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])

## 4.2.0

_2023-10-31_

### Features

- Run parsing in multiple threads and introduce `parseAstAsync` helper function (#5202)

### Pull Requests

- [#5202](https://github.com/rollup/rollup/pull/5202): perf: introduce `parseAstAsync` and parallelize parsing AST ( @sapphi-red)

## 4.1.6

_2023-10-31_

### Bug Fixes

- Fix a bug where emtpy block comments in certain positions could freeze Rollup (#5231)

### Pull Requests

- [#5228](https://github.com/rollup/rollup/pull/5228): build: ensure rust toolchain components for linting are installed (@jerome-benoit)
- [#5231](https://github.com/rollup/rollup/pull/5231): Render emtpy block comments after tree-shaken statements ( @lukastaegert)
- [#5232](https://github.com/rollup/rollup/pull/5232): Revert specifying rustfmt and clippy in toolchain file as it breaks REPL build (@lukastaegert)

## 4.1.5

_2023-10-28_

### Bug Fixes

- Fix an issue where actual entries that were also implicit entries could remain implicit (#5220)

### Pull Requests

- [#5209](https://github.com/rollup/rollup/pull/5209): Document Vite workaround for browser build (@curran)
- [#5215](https://github.com/rollup/rollup/pull/5215): chore(deps): update dependency lint-staged to v15 ( @renovate[bot])
- [#5216](https://github.com/rollup/rollup/pull/5216): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5218](https://github.com/rollup/rollup/pull/5218): Update license plugin (@lukastaegert)
- [#5219](https://github.com/rollup/rollup/pull/5219): Fix error highlight in REPL (@lukastaegert)
- [#5220](https://github.com/rollup/rollup/pull/5220): Fix race condition when emitting implicitly dependent entries ( @lukastaegert)
- [#5224](https://github.com/rollup/rollup/pull/5224): chore(deps): update actions/setup-node action to v4 ( @renovate[bot])
- [#5225](https://github.com/rollup/rollup/pull/5225): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])

## 4.1.4

_2023-10-16_

### Bug Fixes

- Reduce sizes @rollup/browser and @rollup/wasm-node WASM artifacts (#5204)

### Pull Requests

- [#5204](https://github.com/rollup/rollup/pull/5204): perf: shrink wasm size by avoid importing browserslist ( @sapphi-red)

## 4.1.3

_2023-10-15_

### Bug Fixes

- Fix WASM build as hash function was not exported (#5203)

### Pull Requests

- [#5203](https://github.com/rollup/rollup/pull/5203): fix: export xxhashBase64Url from wasm (@sapphi-red)

## 4.1.2

_2023-10-15_

_Release did not finish successfully_

## 4.1.1

_2023-10-15_

### Bug Fixes

- Improve Node parsing performance (#5201)

### Pull Requests

- [#5201](https://github.com/rollup/rollup/pull/5201): perf: use mimalloc for bindings_napi (@sapphi-red)

## 4.1.0

_2023-10-14_

### Features

- Reduce memory usage of Rollup builds (#5133)

### Pull Requests

- [#5133](https://github.com/rollup/rollup/pull/5133): perf: reducing ast node memory overhead (@thebanjomatic)
- [#5177](https://github.com/rollup/rollup/pull/5177): chore: explicitly set rust toolchain channel (@cijiugechu)
- [#5179](https://github.com/rollup/rollup/pull/5179): Update migration guide for Rollup 4 (@lukastaegert)
- [#5180](https://github.com/rollup/rollup/pull/5180): Resolve clippy errors (@cijiugechu)
- [#5183](https://github.com/rollup/rollup/pull/5183): Add clippy to pipeline and fix remaining issues (@lukastaegert)
- [#5184](https://github.com/rollup/rollup/pull/5184): docs: fix code example for `onLog` (@tjenkinson)
- [#5186](https://github.com/rollup/rollup/pull/5186): Improve wording for native artifacts in migration guide ( @lukastaegert)
- [#5190](https://github.com/rollup/rollup/pull/5190): test: add verifyAst type (@TrickyPi)
- [#5196](https://github.com/rollup/rollup/pull/5196): chore(deps): update dependency rollup to v4 (@renovate[bot])
- [#5197](https://github.com/rollup/rollup/pull/5197): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])

## 4.0.2

_2023-10-06_

### Bug Fixes

- Fix annotation detection logic to not fail when a non-ASCII character precedes a double underscore (#5178)

### Pull Requests

- [#5178](https://github.com/rollup/rollup/pull/5178): Handle special characters before double underscores ( @lukastaegert)

## 4.0.1

_2023-10-06_

### Bug Fixes

- Do not panic on trailing semicolons after class methods (#5173)
- Add artifact for arm64 linux musl target (#5176)

### Pull Requests

- [#5172](https://github.com/rollup/rollup/pull/5172): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5173](https://github.com/rollup/rollup/pull/5173): fix: ignores empty statements in class body that is returned by SWC parser (@TrickyPi)
- [#5176](https://github.com/rollup/rollup/pull/5176): Fix linux arm musl build (@lukastaegert)

## 4.0.0

_2023-10-05_

### BREAKING CHANGES

#### General Changes

- The minimal required Node version is now 18.0.0 (#5142)
- The browser build now relies on a WASM artifact that needs to be provided as well (#5073)
- The NodeJS build now relies on an optional native binary; for unsupported platforms, users can use the `@rollup/wasm-node` package that has the same interface as Rollup but relies on WASM artifacts (#5073)
- The `INVALID_IMPORT_ASSERTION` error code has been replaced with `INVALID_IMPORT_ATTRIBUTE` (#5073)
- Rollup will now warn for `@__PURE__` and `@__NO_SIDE_EFFECTS__` annotations in invalid locations (#5165)
- If an entry module starts with a shebang comment `#!...`, this comment will be prepended to the output for `es` and `cjs` formats (#5163)
- File hashes will now use url-safe base64 encoded hashes (#5155)
- The maximum hash length has been reduced to 22 characters (#5155)
- The `RollupWarning` type has been removed in favor of the `RollupLog` type (#5147)

#### Changes to Rollup Options

- Acorn plugins are no longer supported, the `acornInjectPlugins` option has been removed (#5073)
- The `acorn` option has been removed (#5073)
- `output.externalImportAssertions` has been deprecated in favor of `output.externalImportAttributes` (#5073)
- `inlineDynamicImports`, `manualChunks` and `preserveModules` have been removed on input option level: Please use the corresponding output options of the same names (#5143)
- Removed output options (#5143):
  - `output.experimentalDeepDynamicChunkOptimization`: This option is no longer needed as Rollup now always runs the full chunking algorithm
  - `output.dynamicImportFunction`: Use the `renderDynamicImport` plugin hook instead
  - `output.namespaceToStringTag`: Use `output.generatedCode.symbols` instead
  - `output.preferConst`: Use `output.generatedCode.constBindings` instead

#### Plugin API Changes

- For `this.resolve`, the default of the `skipSelf` option is now `true` (#5142)
- `this.parse` now only supports the `allowReturnOutsideFunction` option for now (#5073)
- Import assertions now use the [new import attribute AST structure](https://github.com/estree/estree/blob/master/experimental/import-attributes.md) ( #5073)
- "assertions" have been replaced with "attributes" in various places of the plugin interface (#5073)
- If the import of a module id is handled by the `load` hook of a plugin, `rollup.watch` no longer watches the actual file if the module id corresponds to a real path; if this is intended, then the plugin is responsible for calling `this.addWatchFile` for any dependency files (#5150)
- The normalized input options provided by `buildStart` and other hooks no longer contain an `onwarn` handler; plugins should use `onLog` instead (#5147)
- `this.moduleIds` has been removed from the plugin context: Use `this.getModuleIds()` instead (#5143)
- The `hasModuleSideEffects` flag has been removed from the `ModuleInfo` returned by `this.getModuleInfo()`: Use `moduleSideEffects` on the `ModuleInfo` instead (#5143)

### Features

- Improve parsing speed by switching to a native SWC-based parser (#5073)
- Rollup will now warn for `@__PURE__` and `@__NO_SIDE_EFFECTS__` annotations in invalid locations (#5165)
- The parser is now exposed as a separate export `parseAst` (#5169)

### Bug Fixes

- Rollup no longer tries to watch virtual files if their name corresponds to an actual file name; instead, plugins handle watching via `this.addWatchFile()` (#5150)

### Pull Requests

- [#5073](https://github.com/rollup/rollup/pull/5073): [v4.0] Switch parser to SWC and introduce native/WASM code ( @lukastaegert)
- [#5142](https://github.com/rollup/rollup/pull/5142): [v4.0] Set the default of skipSelf to true (@TrickyPi)
- [#5143](https://github.com/rollup/rollup/pull/5143): [v4.0] Remove deprecated features (@lukastaegert)
- [#5144](https://github.com/rollup/rollup/pull/5144): [v4.0] Imporve the performance of generating ast and rollup ast nodes (@TrickyPi)
- [#5147](https://github.com/rollup/rollup/pull/5147): [v4.0] Remove onwarn from normalized input options ( @lukastaegert)
- [#5150](https://github.com/rollup/rollup/pull/5150): [v4.0] feat: Do not watch files anymore if their content is returned by the load hook (@TrickyPi)
- [#5154](https://github.com/rollup/rollup/pull/5154): [v4.0] Add parse option to allow return outside function ( @lukastaegert)
- [#5155](https://github.com/rollup/rollup/pull/5155): [v4.0] feat: implement hashing content in Rust (@TrickyPi)
- [#5157](https://github.com/rollup/rollup/pull/5157): [v4.0] Handle empty exports (@lukastaegert)
- [#5160](https://github.com/rollup/rollup/pull/5160): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5163](https://github.com/rollup/rollup/pull/5163): [v4.0] feat: preserve shebang in entry module for CJS and ESM outputs (@TrickyPi)
- [#5164](https://github.com/rollup/rollup/pull/5164): [v4.0] fix: also strip BOM from code strings in JS (@TrickyPi)
- [#5165](https://github.com/rollup/rollup/pull/5165): [v4.0] warn for invalid annotations (@lukastaegert)
- [#5168](https://github.com/rollup/rollup/pull/5168): [v4.0] Ensure we support new import attribute "with" syntax ( @lukastaegert)
- [#5169](https://github.com/rollup/rollup/pull/5169): [v4.0] Expose parser (@lukastaegert)

## 3.29.4

_2023-09-28_

### Bug Fixes

- Fix static analysis when an exported function uses callbacks (#5158)

### Pull Requests

- [#5158](https://github.com/rollup/rollup/pull/5158): Deoptimize all parameters when losing track of a function ( @lukastaegert)

## 3.29.3

_2023-09-24_

### Bug Fixes

- Fix a bug where code was wrongly tree-shaken after mutating function parameters (#5153)

### Pull Requests

- [#5145](https://github.com/rollup/rollup/pull/5145): docs: improve the docs repl appearance in the light mode ( @TrickyPi)
- [#5148](https://github.com/rollup/rollup/pull/5148): chore(deps): update dependency @vue/eslint-config-typescript to v12 (@renovate[bot])
- [#5149](https://github.com/rollup/rollup/pull/5149): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5153](https://github.com/rollup/rollup/pull/5153): Fully deoptimize first level path when deoptimizing nested parameter paths (@lukastaegert)

## 3.29.2

_2023-09-15_

### Bug Fixes

- Export `TreeshakingPreset` type (#5131)

### Pull Requests

- [#5131](https://github.com/rollup/rollup/pull/5131): fix: exports `TreeshakingPreset` (@moltar)
- [#5134](https://github.com/rollup/rollup/pull/5134): docs: steps to enable symlinks on windows (@thebanjomatic)
- [#5137](https://github.com/rollup/rollup/pull/5137): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])

## 3.29.1

_2023-09-10_

### Bug Fixes

- Fix time measurement of plugin hooks in watch mode (#5114)
- Ensure accessing document.currentScript in import.meta.url returns correct results (#5118)

### Pull Requests

- [#5114](https://github.com/rollup/rollup/pull/5114): fix(perf): avoid superfluous timer wrappings in watch mode ( @ZhengLiu2825)
- [#5118](https://github.com/rollup/rollup/pull/5118): fix: access document.currentScript at the top level (@TrickyPi)
- [#5125](https://github.com/rollup/rollup/pull/5125): chore(deps): update actions/checkout action to v4 ( @renovate[bot])
- [#5126](https://github.com/rollup/rollup/pull/5126): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5129](https://github.com/rollup/rollup/pull/5129): re-enbale repl-artefacts workflow for rollup-swc branch ( @TrickyPi)

## 3.29.0

_2023-09-06_

### Features

- Add output.sourcemapFileNames option (#5105)
- Add generic type parameter for `api` to Plugin type (#5112)

### Bug Fixes

- Ensure mutations of CustomEvent details are tracked (#5123)

### Pull Requests

- [#5105](https://github.com/rollup/rollup/pull/5105): Added option to name sourcemap files, i.e. a output.sourcemapFileName… (@atti187)
- [#5108](https://github.com/rollup/rollup/pull/5108): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5109](https://github.com/rollup/rollup/pull/5109): Docs: load full path of rollup.browser.js for Rollup V4 ( @TrickyPi)
- [#5112](https://github.com/rollup/rollup/pull/5112): feat(types): add generic type for plugin api (@sxzz)
- [#5115](https://github.com/rollup/rollup/pull/5115): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5123](https://github.com/rollup/rollup/pull/5123): Deoptimize custom event detail (@lukastaegert)

## 3.28.1

_2023-08-22_

### Bug Fixes

- Ensure external files with relative import paths outside the target are rendered correctly (#5099)

### Pull Requests

- [#5093](https://github.com/rollup/rollup/pull/5093): chore(deps): update dependency eslint-config-prettier to v9 ( @renovate[bot])
- [#5094](https://github.com/rollup/rollup/pull/5094): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5099](https://github.com/rollup/rollup/pull/5099): Fix resolution of relative external files outside target directory (@lukastaegert)
- [#5101](https://github.com/rollup/rollup/pull/5101): chore(deps): update dependency lint-staged to v14 ( @renovate[bot])
- [#5102](https://github.com/rollup/rollup/pull/5102): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])

## 3.28.0

_2023-08-09_

### Features

- Add a new property `preliminaryFileName` to generated chunks containing the file name placeholder (#5086)
- Improve performance of sourcemap generation by lazily decoding mappings (#5087)

### Bug Fixes

- Make the `code` property of rendered modules in the output readonly (#5091)

### Pull Requests

- [#5086](https://github.com/rollup/rollup/pull/5086): feat: add `preliminaryFileName` to `OutputChunk` (@lsdsjy)
- [#5087](https://github.com/rollup/rollup/pull/5087): perf(sourcemaps): add back lazy sourcemap decode and handling nullish mappings (@thebanjomatic)
- [#5091](https://github.com/rollup/rollup/pull/5091): fix: the type of RenderedModule.code is readonly (@TrickyPi)

## 3.27.2

_2023-08-04_

### Bug Fixes

- Revert sourcemap performance improvement for now as it causes issues with Vite (#5075)

### Pull Requests

- [#5075](https://github.com/rollup/rollup/pull/5075): Revert perf(sourcemap): lazy compute decoded mappings ( @thebanjomatic)

## 3.27.1

_2023-08-03_

### Bug Fixes

- Improve performance when generating sourcemaps (#5075)

### Pull Requests

- [#5075](https://github.com/rollup/rollup/pull/5075): perf(sourcemap): lazy compute decoded mappings (@thebanjomatic)

## 3.27.0

_2023-07-28_

### Features

- Mark `Object.values` and `Object.entries` as pure if their argument does not contain getters (#5072)

### Pull Requests

- [#5070](https://github.com/rollup/rollup/pull/5070): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5071](https://github.com/rollup/rollup/pull/5071): docs(tutorial): change the .js extension to .mjs (@TrickyPi)
- [#5072](https://github.com/rollup/rollup/pull/5072): Add known globals (@sapphi-red)
- [#5078](https://github.com/rollup/rollup/pull/5078): chore(deps): update dependency @vue/eslint-config-prettier to v8 (@renovate[bot])
- [#5079](https://github.com/rollup/rollup/pull/5079): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])

## 3.26.3

_2023-07-17_

### Bug Fixes

- Do not pass external modules to `manualChunks` to avoid breaking existing configs (#5068)

### Pull Requests

- [#5056](https://github.com/rollup/rollup/pull/5056): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5059](https://github.com/rollup/rollup/pull/5059): chore(config): migrate renovate config (@renovate[bot])
- [#5064](https://github.com/rollup/rollup/pull/5064): chore(deps): update dependency prettier to v3 (@renovate[bot])
- [#5065](https://github.com/rollup/rollup/pull/5065): chore(deps): update typescript-eslint monorepo to v6 (major) ( @renovate[bot])
- [#5068](https://github.com/rollup/rollup/pull/5068): fix: don't pass external modules to the manualChunks function ( @TrickyPi)

## 3.26.2

_2023-07-06_

### Bug Fixes

- Improve error handling when manual chunks would contain external modules (#5050)

### Pull Requests

- [#5050](https://github.com/rollup/rollup/pull/5050): fix: improve error for manualChunks' modules that are resolved as an external module (@TrickyPi)

## 3.26.1

_2023-07-05_

### Bug Fixes

- Support `hasOwnProperty` as exported name in CommonJS (#5010)
- Properly reference browser types in package file (#5051)

### Pull Requests

- [#5010](https://github.com/rollup/rollup/pull/5010): safe hasOwnProperty call (@LongTengDao)
- [#5051](https://github.com/rollup/rollup/pull/5051): @rollup/browser: fix types export map entry (@developit)

## 3.26.0

_2023-06-30_

### Features

- Add `--filterLogs` CLI flag and `ROLLUP_FILTER_LOGS` environment variable for log filtering (#5035)

### Pull Requests

- [#5035](https://github.com/rollup/rollup/pull/5035): Add ability to filter logs via CLI option or environment variable (@lukastaegert)
- [#5049](https://github.com/rollup/rollup/pull/5049): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])

## 3.25.3

_2023-06-26_

### Bug Fixes

- Fix error when inlining dynamic imports that contain unused reexported variables (#5047)

### Pull Requests

- [#5047](https://github.com/rollup/rollup/pull/5047): Do not add tree-shaken variables to namespaces when inlining dynamic imports (@lukastaegert)

## 3.25.2

_2023-06-24_

### Bug Fixes

- Handle plugin errors where `code` is not a string (#5042)
- Use current transformed source when generating code frames with positions in transform hooks (#5045)

### Pull Requests

- [#5038](https://github.com/rollup/rollup/pull/5038): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5040](https://github.com/rollup/rollup/pull/5040): Fix typo in index.md (@vHeemstra)
- [#5042](https://github.com/rollup/rollup/pull/5042): fix: a plugin error can contains numeric code (@TrickyPi)
- [#5045](https://github.com/rollup/rollup/pull/5045): Fix `this.error` with `pos` in `transform` hook (@sapphi-red)
- [#5046](https://github.com/rollup/rollup/pull/5046): chore(deps): update dependency locate-character to v3 ( @renovate[bot])

## 3.25.1

_2023-06-12_

### Bug Fixes

- Respect `__NO_SIDE_EFFECTS__` for async functions (#5031)

### Pull Requests

- [#5031](https://github.com/rollup/rollup/pull/5031): fix: `__NO_SIDE_EFFECTS__` annotation for async function (@antfu)

## 3.25.0

_2023-06-11_

### Features

- Add `this.info` and `this.debug` plugin context logging functions (#5026)
- Add `onLog` option to read, map and filter logs (#5026)
- Add `logLevel` option to fully suppress logs by level (#5026)
- Support function logs in `this.warn`, `this.info` and `this.debug` to avoid heavy computations based on log level ( #5026)
- Add `onLog` plugin hook to read, filter and map logs from plugins (#5026)

### Pull Requests

- [#5026](https://github.com/rollup/rollup/pull/5026): Add Logging API (@lukastaegert)

## 3.24.1

_2023-06-10_

### Bug Fixes

- Fix an issue where bundles with `@rollup/plugin-commonjs` were missing internal dependencies when code-splitting ( #5029)
- Do not use `process.exit(0)` in watch mode to avoid issues in embedded scenarios (#5027)

### Pull Requests

- [#5027](https://github.com/rollup/rollup/pull/5027): fix turborepo with rollup --watch (@plumber-dhaval)
- [#5028](https://github.com/rollup/rollup/pull/5028): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5029](https://github.com/rollup/rollup/pull/5029): fix: get right sideEffectModules (@TrickyPi)

## 3.24.0

_2023-06-07_

### Features

- Add new annotation `/* #__NO_SIDE_EFFECTS__ */` to mark function declarations as side effect free (#5024)

### Pull Requests

- [#5024](https://github.com/rollup/rollup/pull/5024): feat: support `#__NO_SIDE_EFFECTS__` annotation for function declaration (@antfu)

## 3.23.1

_2023-06-04_

### Bug Fixes

- Ensure the last segment of sourcemapBaseUrl is never omitted (#5022)

### Pull Requests

- [#5006](https://github.com/rollup/rollup/pull/5006): Better workflow caching (@lukastaegert)
- [#5012](https://github.com/rollup/rollup/pull/5012): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5022](https://github.com/rollup/rollup/pull/5022): fix: add a trailing slash automatically for sourcemapBaseUrl ( @TrickyPi)
- [#5023](https://github.com/rollup/rollup/pull/5023): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])

## 3.23.0

_2023-05-22_

### Features

- Support emitting "prebuilt chunks" from plugins (#4990)

### Bug Fixes

- Mark Sets and Maps as pure when they receive an array literal as argument (#5005)

### Pull Requests

- [#4990](https://github.com/rollup/rollup/pull/4990): feat: this.emitFile support prebuilt-chunk type (@TrickyPi)
- [#5005](https://github.com/rollup/rollup/pull/5005): feat: mark Set, Map, WeakSet and WeakMap with array arguments as pure (@TrickyPi)

## 3.22.1

_2023-05-21_

### Bug Fixes

- Remove force quit again as it caused some issues (#5004)

### Pull Requests

- [#5001](https://github.com/rollup/rollup/pull/5001): chore(deps): update dependency @rollup/plugin-commonjs to v25 ( @renovate[bot])
- [#5002](https://github.com/rollup/rollup/pull/5002): chore(deps): update dependency eslint-plugin-unicorn to v47 ( @renovate[bot])
- [#5003](https://github.com/rollup/rollup/pull/5003): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#5004](https://github.com/rollup/rollup/pull/5004): Do not force quit Rollup or close stdout (@lukastaegert)

## 3.22.0

_2023-05-17_

### Features

- Prevent empty non-facade chunks by merging them into other suitable chunks (#4989)
- Avoid facade chunks in some situations involving reexports (#4989)
- Improve algorithm for best merge target when using `experimentalMinChunkSize` to take tree-shaking into account ( #4989)

### Bug Fixes

- Take side effects of external dependencies into account when merging chunks for `experimentalMinChunkSize` (#4989)

### Pull Requests

- [#4989](https://github.com/rollup/rollup/pull/4989): Prevent empty chunks and thoroughly improve experimentalMinChunkSize (@lukastaegert)

## 3.21.8

_2023-05-16_

### Bug Fixes

- Allow a namespace to properly contain itself as a named export (#4991)

### Pull Requests

- [#4991](https://github.com/rollup/rollup/pull/4991): Handle self-referencing namespaces (@lukastaegert)

## 3.21.7

_2023-05-13_

### Bug Fixes

- Show correct error on uncaught exceptions in watch mode (#4987)

### Pull Requests

- [#4987](https://github.com/rollup/rollup/pull/4987): Properly quit on uncaught exceptions (@lukastaegert)
- [#4988](https://github.com/rollup/rollup/pull/4988): test: add options type for function tests (@TrickyPi)

## 3.21.6

_2023-05-09_

### Bug Fixes

- Ensure Rollup CLI prints everything to stdout before exiting (#4980)

### Pull Requests

- [#4980](https://github.com/rollup/rollup/pull/4980): chore(deps): lock file maintenance minor/patch updates ( @renovate[bot])
- [#4983](https://github.com/rollup/rollup/pull/4983): Prevent exit before stdout is drained (@lukastaegert)

## 3.21.5

_2023-05-05_

### Bug Fixes

- Keep all consecutive lines at the top of each module that start with a comment (#4975)
- Ensure that declarations inside switch cases do not use the same scope as the discriminator (#4979)

### Pull Requests

- [#4975](https://github.com/rollup/rollup/pull/4975): Keep leading comments on consecutive lines (@lukastaegert)
- [#4979](https://github.com/rollup/rollup/pull/4979): Use correct scope in switch statements (@lukastaegert)

## 3.21.4

_2023-05-03_

### Bug Fixes

- Resolve crash when shimming a missing export in an otherwise non-included module when preserving modules (#4971)

### Pull Requests

- [#4971](https://github.com/rollup/rollup/pull/4971): Handle shimming missing exports when preserving modules ( @lukastaegert)
- [#4972](https://github.com/rollup/rollup/pull/4972): Configure Renovate (@renovate[bot])

## 3.21.3

_2023-05-02_

### Bug Fixes

- Run `process.exit()` when Rollup CLI finishes successfully to solve issues on some systems (#4969)

### Pull Requests

- [#4954](https://github.com/rollup/rollup/pull/4954): test: enable typecheck for \_config files (@antfu)
- [#4969](https://github.com/rollup/rollup/pull/4969): Automatically force close Rollup when done (@lukastaegert)

## 3.21.2

_2023-04-30_

### Bug Fixes

- Mark global functions that trigger iterators as impure for now (#4955)

### Pull Requests

- [#4955](https://github.com/rollup/rollup/pull/4955): fix: mark some known globals or their functions as impure ( @TrickyPi)

## 3.21.1

_2023-04-29_

### Bug Fixes

- Make sure call arguments are properly deoptimized when a function uses the `arguments` variable (#4965)

### Pull Requests

- [#4957](https://github.com/rollup/rollup/pull/4957): Update dependencies (@lukastaegert)
- [#4964](https://github.com/rollup/rollup/pull/4964): Fix REPL in dev (@lukastaegert)
- [#4965](https://github.com/rollup/rollup/pull/4965): Ensure arguments are deoptimized when arguments variable is used (@lukastaegert)
- [#4967](https://github.com/rollup/rollup/pull/4967): Log REPL output to console (@lukastaegert)

## 3.21.0

_2023-04-23_

### Features

- Support tree-shaking of named exports in dynamic imports when using destructuring and similar patterns (#4952)

### Pull Requests

- [#4952](https://github.com/rollup/rollup/pull/4952): feat: tree-shake deterministic dynamic imports (@antfu)

## 3.20.7

_2023-04-21_

### Bug Fixes

- Properly track array element mutations when iterating with a for-of loop (#4949)
- Handle default exporting an anonymous class that extends another class (#4950)

### Pull Requests

- [#4943](https://github.com/rollup/rollup/pull/4943): Add a test for reserved keywords used as import/export specifiers (@Andarist)
- [#4949](https://github.com/rollup/rollup/pull/4949): Deoptimize right side in for-of loops (@lukastaegert)
- [#4950](https://github.com/rollup/rollup/pull/4950): Support default exported classes that extend other classes ( @lukastaegert)

## 3.20.6

_2023-04-18_

### Bug Fixes

- Revert handling of non-JS import and export names due to regressions (#4914)

### Pull Requests

- [#4914](https://github.com/rollup/rollup/pull/4914): feat: add locales in vitepress config (@iDestin)
- [#4946](https://github.com/rollup/rollup/pull/4946): Revert #4939 for now (@lukastaegert)

## 3.20.5

_2023-04-18_

### Bug Fixes

- Handle import and export names that are not valid JavaScript identifiers (#4939)

### Pull Requests

- [#4939](https://github.com/rollup/rollup/pull/4939): Fixed imports/exports that are illegal identifiers in the es output (@Andarist)
- [#4941](https://github.com/rollup/rollup/pull/4941): Reinstate global styles (@lukastaegert)

## 3.20.4

_2023-04-17_

### Bug Fixes

- Do not remove breaks statements after switch statements with conditional breaks (#4937)

### Pull Requests

- [#4937](https://github.com/rollup/rollup/pull/4937): fix: handle conditional breaks in nested switch statement cases ( @TrickyPi and @lukastaegert)

## 3.20.3

_2023-04-16_

### Bug Fixes

- Reduce memory consumption for function call parameter analysis (#4938)
- Fix types for `shouldTransformCachedModule` (#4932)

### Pull Requests

- [#4925](https://github.com/rollup/rollup/pull/4925): chore: repl style add scoped (@btea)
- [#4926](https://github.com/rollup/rollup/pull/4926): docs: Update the x_google_ignorelist url (@jecfish)
- [#4932](https://github.com/rollup/rollup/pull/4932): Allow shouldTransformCachedModule to return null (@bluwy)
- [#4935](https://github.com/rollup/rollup/pull/4935): Bump peter-evans/create-or-update-comment from 2 to 3 ( @dependabot[bot])
- [#4936](https://github.com/rollup/rollup/pull/4936): Disable puppeteer sandbox to fix Vercel deployment ( @lukastaegert)
- [#4938](https://github.com/rollup/rollup/pull/4938): Improve memory usage for parameter deoptimizations ( @lukastaegert)

## 3.20.2

_2023-03-24_

### Bug Fixes

- Fix a crash when using a manual chunk entry that is not already included in the module graph (#4921)
- Fix a crash when reporting a warning with incorrect sourcemap information (#4922)

### Pull Requests

- [#4921](https://github.com/rollup/rollup/pull/4921): Handle manual chunks where the entry is not part of the module graph (@lukastaegert)
- [#4922](https://github.com/rollup/rollup/pull/4922): Do not fail if the location of a warning is outside the original source (@lukastaegert)

## 3.20.1

_2023-03-23_

### Bug Fixes

- Fix returned file name from this.getFileName when assets are deduplicated (#4919)

### Pull Requests

- [#4919](https://github.com/rollup/rollup/pull/4919): Only set asset names when finalizing (@lukastaegert)

## 3.20.0

_2023-03-20_

### Features

- Allow dynamically imported files to have synthetic named exports when preserving modules (#4913)

### Bug Fixes

- Use deterministic file name when emitting several files with same source (#4912)
- Fix a crash when dynamically importing a file with synthetic named exports when preserving modules (#4913)

### Pull Requests

- [#4912](https://github.com/rollup/rollup/pull/4912): fix: make file name deterministic in parallel emits (fix #4909) ( @sun0day)
- [#4913](https://github.com/rollup/rollup/pull/4913): Provide synthetic namespace for dynamic imports when perserving modules (@lukastaegert)

## 3.19.1

_2023-03-10_

### Bug Fixes

- Produce valid code when the first statement in aclass static block is tree-shaken (#4898)

### Pull Requests

- [#4898](https://github.com/rollup/rollup/pull/4898): fix: set a correct node location for static blocks (@TrickyPi)
- [#4900](https://github.com/rollup/rollup/pull/4900): docs: fix table at `output.sanitizeFileName` section (@0x009922)

## 3.19.0

_2023-03-09_

### Features

- Make reassignment tracking of call parameters more specific to no lose information when an object is passed to a function (#4892)

### Pull Requests

- [#4890](https://github.com/rollup/rollup/pull/4890): Fix `npm run dev` (@lukastaegert)
- [#4892](https://github.com/rollup/rollup/pull/4892): Only selectively deoptimize call parameters (@lukastaegert)
- [#4897](https://github.com/rollup/rollup/pull/4897): Pre-render mermaid graphs on website (@lukastaegert)

## 3.18.0

_2023-03-01_

### Features

- Add `experimentalLogSideEffects` to log the first detected side effect in every module (#4871)
- Ignore-list sourcemaps of files inside node_modules by default (#4877)

### Pull Requests

- [#4871](https://github.com/rollup/rollup/pull/4871): Add experimental logging for side effects (@lukastaegert)
- [#4877](https://github.com/rollup/rollup/pull/4877): feat: mark files in a `node_modules` as ignore-listed by default (@bmeurer)
- [#4880](https://github.com/rollup/rollup/pull/4880): build: use @rollup/plugin-replace to replace chokidar fsevents ( @dnalborczyk)
- [#4887](https://github.com/rollup/rollup/pull/4887): Refactor (@dnalborczyk)

## 3.17.3

_2023-02-25_

### Bug Fixes

- Handle non-URL-safe characters when poly-filling import.meta.url (#4875)

### Pull Requests

- [#4870](https://github.com/rollup/rollup/pull/4870): fix: style optimization in dark mode (@huodoushigemi)
- [#4875](https://github.com/rollup/rollup/pull/4875): Fix transformation of `import.meta.url` in CommonJS (@fasttime)
- [#4876](https://github.com/rollup/rollup/pull/4876): fix: wrong params of the transform hook (@ZzqiZQute)
- [#4878](https://github.com/rollup/rollup/pull/4878): Improve test stability (@lukastaegert)

## 3.17.2

_2023-02-20_

### Bug Fixes

- Do not omit code if a file that only re-exports a used variable has `moduleSideEffects` set to `true` (#4867)
- Add missing `needsCodeReference` property in TypeScript for asset tree-shaking (#4868)
- Add correct side effect configuration for additional Object and Promise methods (#4323)

### Pull Requests

- [#4323](https://github.com/rollup/rollup/pull/4323): feat: add known globals (@dnalborczyk)
- [#4867](https://github.com/rollup/rollup/pull/4867): Include side effects of re-exporters unless they have moduleSideEffects: false (@lukastaegert)
- [#4868](https://github.com/rollup/rollup/pull/4868): Add `needsCodeReference` property to `EmittedAsset` (@sapphi-red)

## 3.17.1

_2023-02-18_

### Bug Fixes

- Add TypeScript types for `loadConfigFile` (#4853)
- Fix an issue that could include unused classes in the bundle if their super class was in a file with `moduleSideEffects: false` (#4866)

### Pull Requests

- [#4853](https://github.com/rollup/rollup/pull/4853): feat: export loadConfigFile type (@TrickyPi)
- [#4866](https://github.com/rollup/rollup/pull/4866): Do not mark variable access in files without side effects as TDZ (@lukastaegert)

## 3.17.0

_2023-02-18_

### Features

- Deprecate `experimentalDeepDynamicChunkOptimization` and always run the full chunk generation algorithm (#4862)

### Bug Fixes

- Fix an issue that caused very slow builds for projects with over 1000 dynamic imports when `experimentalDeepDynamicChunkOptimization` was enabled (#4862)

### Pull Requests

- [#4862](https://github.com/rollup/rollup/pull/4862): Improve chunking performance (@lukastaegert)

## 3.16.0

_2023-02-17_

### Features

- Support `output.sourcemapIgnoreList` option to mark file sources as ignored in the `x_google_ignoreList` attribute of the resulting sourcemap (#4848)
- Support sourcemaps where `sourcesContent` contains `null` entries (#4846)
- Allow explicitly passing `true` for the `cache` option to override Vite's default (#4859)

### Bug Fixes

- Fix an issue where unrelated side effects spilled into other chunks when using the `experimentalMinChunkSize` option ( #4851)

### Pull Requests

- [#4846](https://github.com/rollup/rollup/pull/4846): Update magic-string and adjust types. (@bmeurer)
- [#4848](https://github.com/rollup/rollup/pull/4848): Introduce `sourcemapIgnoreList` predicate. (@bmeurer)
- [#4851](https://github.com/rollup/rollup/pull/4851): Fix chunk graph update when merging chunks for minChunkSize ( @lukastaegert)
- [#4852](https://github.com/rollup/rollup/pull/4852): docs: make api params more readable (@cunzaizhuyi)
- [#4856](https://github.com/rollup/rollup/pull/4856): simplify code in includeStatements (@TrickyPi)
- [#4859](https://github.com/rollup/rollup/pull/4859): Allow to pass "true" to InputOptions.cache (@danielrentz)

## 3.15.0

_2023-02-10_

### Features

- Do not consider instantiating a constructor a side effect if it adds properties to "this" and is instantiated elsewhere (#4842)

### Bug Fixes

- Improve side effect detection in constructors (#4842)

### Pull Requests

- [#4842](https://github.com/rollup/rollup/pull/4842): fix: add this option to context.ignore (@TrickyPi)
- [#4843](https://github.com/rollup/rollup/pull/4843): fixed the logo link (@oMatheuss)
- [#4844](https://github.com/rollup/rollup/pull/4844): Update index.md (@cunzaizhuyi)
- [#4845](https://github.com/rollup/rollup/pull/4845): docs: fix style (@TrickyPi)

## 3.14.0

_2023-02-05_

### Features

- Add `experimentalDeepDynamicChunkOptimization` option to produce fewer chunks from dynamic imports (#4837)

### Pull Requests

- [#4837](https://github.com/rollup/rollup/pull/4837): Add flag to re-enable deep dynamic chunk optimization ( @lukastaegert)
- [#4839](https://github.com/rollup/rollup/pull/4839): fix: correct incorrect assertions (@TrickyPi)

## 3.13.0

_2023-02-03_

### Features

- Prevent chunk cycles when using `experimentalMinChunkSize` (#4723)

### Pull Requests

- [#4723](https://github.com/rollup/rollup/pull/4723): Improve minChunkSize algorithm (@lukastaegert)
- [#4833](https://github.com/rollup/rollup/pull/4833): docs: Fix typo (@mturoci)
- [#4835](https://github.com/rollup/rollup/pull/4835): Tables in docs (@lukastaegert)

## 3.12.1

_2023-02-01_

### Bug Fixes

- Handle self-references in class static blocks and construtors when the class is renamed (#4827)
- Improve warnings when creating circular chunks taht reexport variables (#4829)

### Pull Requests

- [#4827](https://github.com/rollup/rollup/pull/4827): fix: use the original class name in the class body (@TrickyPi)
- [#4829](https://github.com/rollup/rollup/pull/4829): Improve and fix cross-chunk-reexport warning (@lukastaegert)
- [#4830](https://github.com/rollup/rollup/pull/4830): Add Algolia doc search (@lukastaegert)
- [#4831](https://github.com/rollup/rollup/pull/4831): Add warning not to add assets directly to the bundle ( @lukastaegert)

## 3.12.0

_2023-01-28_

### Features

- Change generated external namespace reexport helper code for CommonJS to better work with NodeJS named export detection (#4826)

### Pull Requests

- [#4825](https://github.com/rollup/rollup/pull/4825): Add and use anchors for nested options (@lukastaegert)
- [#4826](https://github.com/rollup/rollup/pull/4826): Use old namespace reexport code pattern for better Node support ( @lukastaegert)

## 3.11.0

_2023-01-26_

### Features

- Support opt-in tree-shaking for emitted assets based on code references (#4805)

### Bug Fixes

- Adapt documentation references in Rollup to new website (#4807)

### Pull Requests

- [#4805](https://github.com/rollup/rollup/pull/4805): feat: add needsCodeReference field to EmittedAsset (@TrickyPi)
- [#4807](https://github.com/rollup/rollup/pull/4807): Rewrite website in Vitepress and merge it into the main repository (@lukastaegert)
- [#4816](https://github.com/rollup/rollup/pull/4816): web-publisher: Update docs/faqs/index.md (@PuruVJ)
- [#4819](https://github.com/rollup/rollup/pull/4819): Replace fs-extra with built-ins (@dnalborczyk)
- [#4820](https://github.com/rollup/rollup/pull/4820): Introduce timeout-minutes in Github actions ci (@dnalborczyk)
- [#4822](https://github.com/rollup/rollup/pull/4822): Tweak document landing page (@sapphi-red)
- [#4823](https://github.com/rollup/rollup/pull/4823): Minor migration guide improvements (@sapphi-red)
- [#4824](https://github.com/rollup/rollup/pull/4824): Add most options to the REPL (@lukastaegert)

## 3.10.1

_2023-01-20_

### Bug Fixes

- Fix some crashes when using optional chaining with namespaces and improve tree-shaking (#4812)
- Avoid wrongly removed code when using optional chaining (#4812)

### Pull Requests

- [#4809](https://github.com/rollup/rollup/pull/4809): fix: rollup bin file is in dist folder (@saibotsivad)
- [#4812](https://github.com/rollup/rollup/pull/4812): Rework tree-shaking support for optional chaining (@lukastaegert)

## 3.10.0

_2023-01-12_

### Features

- Add information about the resolving plugin to resolved ids (#4789)
- Improve treeshaking for optional chaining when the root is nullish (#4797)

### Bug Fixes

- Remove unnecessary internal defaults for acorn options (#4786)

### Pull Requests

- [#4785](https://github.com/rollup/rollup/pull/4785): Use @jridgewell/sourcemap-codec (@bluwy)
- [#4786](https://github.com/rollup/rollup/pull/4786): Remove default acorn options + other fixes (@dnalborczyk)
- [#4789](https://github.com/rollup/rollup/pull/4789): feat: add `resolvedBy` field to `ResolvedId` (@TrickyPi)
- [#4794](https://github.com/rollup/rollup/pull/4794): fix: import can be shortened (@cunzaizhuyi)
- [#4796](https://github.com/rollup/rollup/pull/4796): Update dependencies (@lukastaegert)
- [#4797](https://github.com/rollup/rollup/pull/4797): feat: treeshake for optional chaining (@antfu)

## 3.9.1

_2023-01-02_

### Bug Fixes

- Sort keys in generated dynamic namespace objects (#4780)
- Do not consider Array.group to be side effect free as the specs have changed (#4779)

### Pull Requests

- [#4777](https://github.com/rollup/rollup/pull/4777): Import from node:fs/promises (@dnalborczyk)
- [#4778](https://github.com/rollup/rollup/pull/4778): Bump deps (@dnalborczyk)
- [#4779](https://github.com/rollup/rollup/pull/4779): Remove array grouping (web compat issue) (@dnalborczyk)
- [#4780](https://github.com/rollup/rollup/pull/4780): Sort namespace object keys (@dnalborczyk)
- [#4781](https://github.com/rollup/rollup/pull/4781): Use Set and builtin-modules package (@dnalborczyk)
- [#4782](https://github.com/rollup/rollup/pull/4782): Use more restrictive types (@dnalborczyk)

## 3.9.0

_2022-12-28_

### Features

- Support ES2022 arbitrary module namespace identifiers (#4770)
- Add optional `version` property to plugin type (#4771)

### Pull Requests

- [#4768](https://github.com/rollup/rollup/pull/4768): Fix small typo in 999-big-list-of-options.md (@ericmutta)
- [#4769](https://github.com/rollup/rollup/pull/4769): docs: add a instruction about how to run one test on your local computer (@TrickyPi)
- [#4770](https://github.com/rollup/rollup/pull/4770): Add support for arbitrary module namespace identifiers ( @lukastaegert)
- [#4771](https://github.com/rollup/rollup/pull/4771): Add `version` property to Plugin type (@Septh)

## 3.8.1

_2022-12-23_

### Bug Fixes

- Reduce memory footprint when explicitly passing `cache: false` (#4762)
- Fix a crash when preserving modules and reexporting namespaces (#4766)

### Pull Requests

- [#4762](https://github.com/rollup/rollup/pull/4762): Improve AST garbage collection (@bluwy)
- [#4766](https://github.com/rollup/rollup/pull/4766): Fix handling of namespace reexports when preserving modules ( @lukastaegert)

## 3.8.0

_2022-12-22_

### Features

- Deduplicate ESM exports and reexports when preserving modules (#4759)

### Bug Fixes

- Handle files that are emitted as a side effect of the manualChunks option (#4759)

### Pull Requests

- [#4759](https://github.com/rollup/rollup/pull/4759): feat: deduplicate reexports and renderedExports to simplify output (@TrickyPi)
- [#4761](https://github.com/rollup/rollup/pull/4761): Support emitting files via manualChunks in output (@lukastaegert)
- [#4763](https://github.com/rollup/rollup/pull/4763): docs: update outdated info (@TrickyPi)

## 3.7.5

_2022-12-17_

### Bug Fixes

- Avoid name shadowing when default exporting a class that matches the name of another class (#4756)
- Do not display the error message both in a separate line and in the stack trace in rollup CLI (#4749)
- Make type of `RollupWarning.cause` compatible with `Error.cause` (#4757)
- Do not swallow side effects when interacting with modules namespaces nested in another object (#4758)

### Pull Requests

- [#4749](https://github.com/rollup/rollup/pull/4749): feat: simplify `stack` info in cli error (@TrickyPi)
- [#4756](https://github.com/rollup/rollup/pull/4756): Avoid name conflicts for default exported classes (@lukastaegert)
- [#4757](https://github.com/rollup/rollup/pull/4757): fix: RollupLog cause allow unknown (@Shinigami92)
- [#4758](https://github.com/rollup/rollup/pull/4758): Correctly handle side effects when a namespace is nested in an object (@lukastaegert)

## 3.7.4

_2022-12-13_

### Bug Fixes

- Do not remove calls to `.exec` and `.test` for included stateful regular expressions (#4742)

### Pull Requests

- [#4742](https://github.com/rollup/rollup/pull/4742): fix: check whether RegExp have the global or sticky flags set ( @TrickyPi)

## 3.7.3

_2022-12-11_

### Bug Fixes

- Ensure `this.getFileName` no longer returns a placeholder as soon as hash placeholders have been resolved (#4747)

### Pull Requests

- [#4747](https://github.com/rollup/rollup/pull/4747): provide hashed file name when using this.getFileName in generateBundle (@lukastaegert)

## 3.7.2

_2022-12-10_

### Bug Fixes

- Improve chunk generation performance when one module is dynamically imported by many other modules (#4736)

### Pull Requests

- [#4736](https://github.com/rollup/rollup/pull/4736): Improve chunk assignment performance (@lukastaegert)

## 3.7.1

_2022-12-09_

### Bug Fixes

- Ad a hint to use @rollup/plugin-json when imports from a JSON file are not found (#4741)

### Pull Requests

- [#4741](https://github.com/rollup/rollup/pull/4741): fix: provide json hint when importing a no export json file ( @TrickyPi)

## 3.7.0

_2022-12-08_

### Features

- Do not treat `.test` and `.exec` on regular expressions as side effects (#4737)

### Pull Requests

- [#4737](https://github.com/rollup/rollup/pull/4737): feat: add sutiable RegExp prototype methods (@TrickyPi)

## 3.6.0

_2022-12-05_

### Features

- extend `this.getModuleInfo` with information about exports (#4731)

### Pull Requests

- [#4731](https://github.com/rollup/rollup/pull/4731): feat: add `exports` and `exportedBindings` to `Module` class ( @TrickyPi)

## 3.5.1

_2022-12-01_

### Bug Fixes

- Accept functions returning a config in defineConfig (#4728)

### Pull Requests

- [#4728](https://github.com/rollup/rollup/pull/4728): Overload defineConfig to accept a RollupOptionsFunction parameter (@Septh)

## 3.5.0

_2022-11-27_

### Features

- Add `treeshake.manualPureFunctions` to override static analysis for explicit function names (#4718)

### Bug Fixes

- Do not throw when a plugin uses `this.load` without awaiting its result (#4725)

### Pull Requests

- [#4718](https://github.com/rollup/rollup/pull/4718): Add simple way to manually declare pure functions (@lukastaegert)
- [#4725](https://github.com/rollup/rollup/pull/4725): Fix isIncluded error when using rollup-plugin-typescript2 ( @lukastaegert)

## 3.4.0

_2022-11-22_

### Features

- Do not keep unused `Object.freeze` calls on object literals (#4720)

### Pull Requests

- [#4720](https://github.com/rollup/rollup/pull/4720): Only consider Object.freeze a side effect if the argument is used (@lukastaegert)

## 3.3.0

_2022-11-12_

### Features

- Add "experimentalMinChunkSize" option to merge smaller chunks into larger ones (#4705)
- Automatically deduplicate assets again when the source is a `Buffer` (#4712)
- Deduplicate `Buffer` with `string` assets (#4712)

### Bug Fixes

- Support plugins with object hooks when using `perf: true` (#4707)

### Pull Requests

- [#4702](https://github.com/rollup/rollup/pull/4702): docs: add additional tips for heap out of memory (@benmccann)
- [#4705](https://github.com/rollup/rollup/pull/4705): Allow to define minimum chunk size limit (@lukastaegert)
- [#4707](https://github.com/rollup/rollup/pull/4707): Fix perf timers for object hooks (@lukastaegert)
- [#4710](https://github.com/rollup/rollup/pull/4710): Update terser docs (@nikolas)
- [#4712](https://github.com/rollup/rollup/pull/4712): feat: deduplicate assets with buffer source (@patak-dev)

## 3.2.5

_2022-11-01_

### Bug Fixes

- We deconflicting classes, ensure the original class name still does not shadow variables (#4697)

### Pull Requests

- [#4697](https://github.com/rollup/rollup/pull/4697): Prevent class ids from shadowing other variables (@lukastaegert)

## 3.2.4

_2022-10-31_

### Bug Fixes

- Always use forward slashes in chunk ids when preserving modules, even on Windows (#4693)
- Escape problematic characters in ids when rewriting `import.meta.url` (#4693)

### Pull Requests

- [#4685](https://github.com/rollup/rollup/pull/4685): update package-lock version (@jerry-lllman)
- [#4689](https://github.com/rollup/rollup/pull/4689): Update 07-tools.md (@cokert)
- [#4693](https://github.com/rollup/rollup/pull/4693): Use correct import.meta.url slashes on Windows (@lukastaegert)

## 3.2.3

_2022-10-18_

### Bug Fixes

- Fix an issue whre Rollup confused `new.target` with `import.meta` (#4679)
- Ensure that Rollup does not make assumptions about the value of unknown namespace import members (#4684)

### Pull Requests

- [#4679](https://github.com/rollup/rollup/pull/4679): Do not rewrite new.target (@lukastaegert)
- [#4683](https://github.com/rollup/rollup/pull/4683): Remove typo in resolveId documentation (@ChrispyChris)
- [#4684](https://github.com/rollup/rollup/pull/4684): Return correct values for unknown namespace members ( @lukastaegert)

## 3.2.2

_2022-10-16_

### Bug Fixes

- Do not hang/crash on hashbang comments in input modules (#4676)

### Pull Requests

- [#4675](https://github.com/rollup/rollup/pull/4675): refactor: improve & simplify types (@sxzz)
- [#4676](https://github.com/rollup/rollup/pull/4676): Ignore hashhbang comments (@lukastaegert)

## 3.2.1

_2022-10-16_

### Bug Fixes

- Rewrite class declarations to preserve their .name property if necessary (#4674)

### Pull Requests

- [#4674](https://github.com/rollup/rollup/pull/4674): Preserve rendered class names (@lukastaegert)

## 3.2.0

_2022-10-15_

### Features

- Support providing Promises as plugins like Vite (#4671)

### Pull Requests

- [#4666](https://github.com/rollup/rollup/pull/4666): Add unicorn plugin (@lukastaegert)
- [#4667](https://github.com/rollup/rollup/pull/4667): refactor: improve types (@sxzz)
- [#4668](https://github.com/rollup/rollup/pull/4668): fix: nested plugin in options stage (@sxzz)
- [#4669](https://github.com/rollup/rollup/pull/4669): refactor: merge duplicate imports (@c0dedance)
- [#4670](https://github.com/rollup/rollup/pull/4670): docs: fix minor typo in migration documentation (@ThisIsMissEm)
- [#4671](https://github.com/rollup/rollup/pull/4671): feat: support async plugins (@sxzz)

## 3.1.0

_2022-10-12_

### Features

- Support using arrays of plugins as plugins like Vite (#4657)

### Pull Requests

- [#4657](https://github.com/rollup/rollup/pull/4657): feat: support nested plugin (@sxzz)

## 3.0.1

_2022-10-12_

### Bug Fixes

- Fix installation on Windows (#4662)
- Avoid missing parameters that are only used in a destructuring initializer (#4663)

### Pull Requests

- [#4661](https://github.com/rollup/rollup/pull/4661): Enforce type imports (@lukastaegert)
- [#4662](https://github.com/rollup/rollup/pull/4662): fix: missing "node" causes run script error (@c0dedance)
- [#4663](https://github.com/rollup/rollup/pull/4663): Ensure the initializer of a destructuring declaration is always included if the id is included (@lukastaegert)
- [#4664](https://github.com/rollup/rollup/pull/4664): fix: remove lint:js:nofix script redundancy options (@c0dedance)

## 3.0.0

_2022-10-11_

### Breaking Changes

#### General Changes

- Rollup now requires at least Node 14.18.0 to run (#4548 and #4596)
- The browser build has been split into a separate package `@rollup/browser` (#4593)
- The node build uses the `node:` prefix for imports of builtin modules (#4596)
- Some previously deprecated features have been removed (#4552):
  - Some plugin context functions have been removed:
    - `this.emitAsset()`: use `this.emitFile()`
    - `this.emitChunk()`: use `this.emitFile()`
    - `this.getAssetFileName()`: use `this.getFileName()`
    - `this.getChunkFileName()`: use `this.getFileName()`
    - `this.isExternal()`: use `this.resolve()`
    - `this.resolveId()`: use `this.resolve()`
  - The `resolveAssetUrl` plugin hook has been removed: use `resolveFileUrl`
  - Rollup no longer passes `assetReferenceId` or `chunkReferenceId` parameters to `resolveFileUrl`
  - The `treeshake.pureExternalModules` option has been removed: use `treeshake.moduleSideEffects: 'no-external'`
  - You may no longer use `true` or `false` for `output.interop`. As a replacement for `true`, you can use "compat"
  - Emitted assets no longer have an `isAsset` flag in the bundle
  - Rollup will no longer fix assets added directly to the bundle by adding the `type: "asset"` field
- Some features that were previously marked for deprecation now show warnings when used (#4552):
  - Some options have been deprecated:
    - `inlineDynamicImports` as part of the input options: use `output. inlineDynamicImports`
    - `manualChunks` as part of the input options: use `output. manualChunks `
    - `maxParallelFileReads`: use `maxParallelFileOps
    - `output.preferConst`: use `output.generatedCode.constBindings`
    - `output.dynamicImportFunction`: use the `renderDynamicImport` plugin hook
    - `output.namespaceToStringTag`: use `output.generatedCode.symbols`
    - `preserveModules` as part of the input options: use `output. preserveModules `
  - You should no longer access `this.moduleIds` in plugins: use `this.getModuleIds()`
  - You should no longer access `this.getModuleInfo(...).hasModuleSideEffects` in plugins: use `this.getModuleInfo(...).moduleSideEffects`
- Configuration files are only bundled if either the `--configPlugin` or the `--bundleConfigAsCjs` options are used. The configuration is bundled to an ES module unless the `--bundleConfigAsCjs` option is used. In all other cases, configuration is now loaded using Node's native mechanisms (#4574 and #4621)
- The properties attached to some errors have been changed so that there are fewer different possible properties with consistent types (#4579)
- Some errors have been replaced by others (ILLEGAL_NAMESPACE_REASSIGNMENT -> ILLEGAL_REASSIGNMENT, NON_EXISTENT_EXPORT -> MISSING_EXPORT) (#4579)
- Files in `rollup/dist/*` can only be required using their file extension (#4581)
- The `loadConfigFile` helper now has a named export of the same name instead of a default export (#4581)
- When using the API and sourcemaps, sourcemap comments are contained in the emitted files and sourcemaps are emitted as regular assets (#4605)
- Watch mode no longer uses Node's EventEmitter but a custom implementation that awaits Promises returned from event handlers (#4609)
- Assets may only be deduplicated with previously emitted assets if their source is a `string` (#4644)
- By default, Rollup will keep external dynamic imports as `import(…)` in commonjs output unless `output.dynamicImportInCjs` is set to false (#4647)

#### Changes to Rollup Options

- As functions passed to `output.banner/footer/intro/outro` are now called per-chunk, they should be careful to avoid performance-heavy operations (#4543)
- `entryFileNames/chunkFileNames` functions now longer have access to the rendered module information via `modules`, only to a list of included `moduleIds` (#4543)
- The path of a module is no longer prepended to the corresponding chunk when preserving modules (#4565)
- When preserving modules, the `[name]` placeholder (as well as the `chunkInfo.name` property when using a function) now includes the relative path of the chunk as well as optionally the file extension if the extension is not one of `.js`, `.jsx`, `.mjs`, `.cjs`, `.ts`, `.tsx`, `.mts`, or `.cts` (#4565)
- The `[ext]`, `[extName]` and `[assetExtName]` placeholders are no longer supported when preserving modules (#4565)
- The `perf` option no longer collects timings for the asynchronous part of plugin hooks as the readings were wildly inaccurate and very misleading, and timings are adapted to the new hashing algorithm (#4566)
- Change the default value of `makeAbsoluteExternalsRelative` to "ifRelativeSource" so that absolute external imports will no longer become relative imports in the output, while relative external imports will still be renormalized ( #4567)
- Change the default for `output.generatedCode.reservedNamesAsProps` to no longer quote properties like `default` by default (#4568)
- Change the default for `preserveEntrySignatures` to "exports-only" so that by default, empty facades for entry chunks are no longer created (#4576)
- Change the default for `output.interop` to "default" to better align with NodeJS interop (#4611)
- Change the default for `output.esModule` to "if-default-prop", which only adds \_\_esModule when the default export would be a property (#4611)
- Change the default for `output.systemNullSetters` to `true`, which requires at least SystemJS 6.3.3 (#4649)

#### Plugin API Changes

- Plugins that add/change/remove imports or exports in `renderChunk` should make sure to update `ChunkInfo.imports/importedBindings/exports` accordingly (#4543)
- The order of plugin hooks when generating output has changed (#4543)
- Chunk information passed to `renderChunk` now contains names with hash placeholders instead of final names, which will be replaced when used in the returned code or `ChunkInfo.imports/importedBindings/exports` (#4543 and #4631)
- Hooks defined in output plugins will now run after hooks defined in input plugins (used to be the other way around) ( #3846)

### Features

- Functions passed to `output.banner/footer/intro/outro` are now called per-chunk with some chunk information (#4543)
- Plugins can access the entire chunk graph via an additional parameter in `renderChunk` (#4543)
- Chunk hashes only depend on the actual content of the chunk and are otherwise stable against things like renamed/moved source files or changed module resolution order (#4543)
- The length of generated file hashes can be customized both globally and per-chunk (#4543)
- When preserving modules, the regular `entryFileNames` logic is used and the path is included in the `[name]` property. This finally gives full control over file names when preserving modules (#4565)
- `output.entryFileNames` now also supports the `[hash]` placeholder when preserving modules (#4565)
- The `perf` option will now collect (synchronous) timings for all plugin hooks, not just a small selection (#4566)
- All errors thrown by Rollup have `name: RollupError` now to make clearer that those are custom error types (#4579)
- Error properties that reference modules (such as id and ids) will now always contain the full ids. Only the error message will use shortened ids (#4579)
- Errors that are thrown in response to other errors (e.g. parse errors thrown by acorn) will now use the standardized cause property to reference the original error (#4579)
- If sourcemaps are enabled, files will contain the appropriate sourcemap comment in `generateBundle` and sourcemap files are available as regular assets (#4605)
- Returning a Promise from an event handler attached to a RollupWatcher instance will make Rollup wait for the Promise to resolve (#4609)
- There is a new value "compat" for output.interop that is similar to "auto" but uses duck-typing to determine if there is a default export (#4611)
- There is a new value "if-default-prop" for esModule that only adds an `__esModule` marker to the bundle if there is a default export that is rendered as a property (#4611)
- Rollup can statically resolve checks for `foo[Symbol.toStringTag]` to "Module" if foo is a namespace (#4611)
- There is a new CLI option `--bundleConfigAsCjs` which will force the configuration to be bundled to CommonJS (#4621)
- Import assertions for external imports that are present in the input files will be retained in ESM output (#4646)
- Rollup will warn when a module is imported with conflicting import assertions (#4646)
- Plugins can add, remove or change import assertions when resolving ids (#4646)
- The `output.externalImportAssertions` option allows to turn off emission of import assertions (#4646)
- Use `output.dynamicImportInCjs` to control if dynamic imports are emitted as `import(…)` or wrapped `require(…)` when generating commonjs output (#4647)

### Bug Fixes

- Chunk hashes take changes in `renderChunk`, e.g. minification, into account (#4543)
- Hashes of referenced assets are properly reflected in the chunk hash (#4543)
- No longer warn about implicitly using default export mode to not tempt users to switch to named export mode and break Node compatibility (#4624)
- Avoid performance issues when emitting thousands of assets (#4644)

### Pull Requests

- [#3846](https://github.com/rollup/rollup/pull/3846): [v3.0] Run output plugins last (@aleclarson)
- [#4543](https://github.com/rollup/rollup/pull/4543): [v3.0] New hashing algorithm that "fixes (nearly) everything" ( @lukastaegert)
- [#4548](https://github.com/rollup/rollup/pull/4548): [v3.0] Deprecate Node 12 (@lukastaegert)
- [#4552](https://github.com/rollup/rollup/pull/4552): [v3.0] Remove actively deprecated features, show warnings for other deprecated features (@lukastaegert)
- [#4558](https://github.com/rollup/rollup/pull/4558): [v3.0] Convert build scripts to ESM, update dependencies ( @lukastaegert)
- [#4565](https://github.com/rollup/rollup/pull/4565): [v3.0] Rework file name patterns when preserving modules ( @lukastaegert)
- [#4566](https://github.com/rollup/rollup/pull/4566): [v3.0] Restructure timings (@lukastaegert)
- [#4567](https://github.com/rollup/rollup/pull/4567): [v3.0] Change default for makeAbsoluteExternalsRelative ( @lukastaegert)
- [#4568](https://github.com/rollup/rollup/pull/4568): [v3.0] Change default for output.generatedCode.reservedNamesAsProps (@lukastaegert)
- [#4574](https://github.com/rollup/rollup/pull/4574): [v3.0] Better esm config file support (@lukastaegert)
- [#4575](https://github.com/rollup/rollup/pull/4575): [v3.0] Show deprecation warning for maxParallelFileReads ( @lukastaegert)
- [#4576](https://github.com/rollup/rollup/pull/4576): [v3.0] Change default for preserveEntrySignatures to exports-only (@lukastaegert)
- [#4579](https://github.com/rollup/rollup/pull/4579): [v3.0] Refine errors and warnings (@lukastaegert)
- [#4581](https://github.com/rollup/rollup/pull/4581): [v3.0] Use named export for loadConfigFile (@lukastaegert)
- [#4592](https://github.com/rollup/rollup/pull/4592): [v3.0] Port doc changes from #4572 and #4583 to 3.0 (@berniegp)
- [#4593](https://github.com/rollup/rollup/pull/4593): [v3.0] Browser build (@lukastaegert)
- [#4596](https://github.com/rollup/rollup/pull/4596): [v3.0] Use "node:" prefix for imports of node builtins ( @lukastaegert)
- [#4605](https://github.com/rollup/rollup/pull/4605): [v3.0] Better sourcemap emission (@lukastaegert)
- [#4609](https://github.com/rollup/rollup/pull/4609): [v3.0] Custom awaiting watch emitter (@lukastaegert)
- [#4611](https://github.com/rollup/rollup/pull/4611): [v3.0] Improve interop defaults (@lukastaegert)
- [#4621](https://github.com/rollup/rollup/pull/4621): [v3.0] Always try to load config files via Node if possible ( @lukastaegert)
- [#4624](https://github.com/rollup/rollup/pull/4624): [v3.0] Remove warning when using implicit default export mode ( @lukastaegert)
- [#4631](https://github.com/rollup/rollup/pull/4631): [v3.0] Use ASCII characters for hash placeholders (@lukastaegert)
- [#4644](https://github.com/rollup/rollup/pull/4644): [v3.0] Improve performance of asset emissions (@lukastaegert)
- [#4646](https://github.com/rollup/rollup/pull/4646): [v3.0] Basic support for import assertions (@lukastaegert)
- [#4647](https://github.com/rollup/rollup/pull/4647): [v3.0] Keep dynamic imports in CommonJS output (@lukastaegert)
- [#4649](https://github.com/rollup/rollup/pull/4649): [v3.0] Change default for systemNullSetters (@lukastaegert)
- [#4651](https://github.com/rollup/rollup/pull/4651): [v3.0] use compiler target ES2020 (@dnalborczyk)

## 2.79.1

_2022-09-22_

### Bug Fixes

- Avoid massive performance degradation when creating thousands of chunks (#4643)

### Pull Requests

- [#4639](https://github.com/rollup/rollup/pull/4639): fix: typo docs and contributors link in CONTRIBUTING.md ( @takurinton)
- [#4641](https://github.com/rollup/rollup/pull/4641): Update type definition of resolveId (@ivanjonas)
- [#4643](https://github.com/rollup/rollup/pull/4643): Improve performance of chunk naming collision check ( @lukastaegert)

## 2.79.0

_2022-08-31_

### Features

- Add `amd.forceJsExtensionForImports` to enforce using `.js` extensions for relative AMD imports (#4607)

### Pull Requests

- [#4607](https://github.com/rollup/rollup/pull/4607): add option to keep extensions for amd (@wh1tevs)

## 2.78.1

_2022-08-19_

### Bug Fixes

- Avoid inferring "arguments" as name for a default export placeholder variable (#4613)

### Pull Requests

- [#4613](https://github.com/rollup/rollup/pull/4613): Prevent using arguments for generated variable names ( @lukastaegert)

## 2.78.0

_2022-08-14_

### Features

- Support writing plugin hooks as objects with a "handler" property (#4600)
- Allow changing execution order per plugin hook (#4600)
- Add flag to execute plugins in async parallel hooks sequentially (#4600)

### Pull Requests

- [#4600](https://github.com/rollup/rollup/pull/4600): Allow using objects as hooks to change execution order ( @lukastaegert)

## 2.77.3

_2022-08-11_

### Bug Fixes

- Correctly resolve preserveModulesRoot in Vite (#4591)

### Pull Requests

- [#4591](https://github.com/rollup/rollup/pull/4591): resolve currentPath (@cleverpp)

## 2.77.2

_2022-07-27_

### Bug Fixes

- Avoid a rendering failure when mixing outputs with inlined and non-inlined dynamic imports (#4589)

### Pull Requests

- [#4589](https://github.com/rollup/rollup/pull/4589): Handle generating non-inlined imports after inlined ones ( @lukastaegert)

## 2.77.1

_2022-07-26_

### Bug Fixes

- Ensure IIFE output generates a global variable when generating ES5 (#4588)

### Pull Requests

- [#4577](https://github.com/rollup/rollup/pull/4577): broken link removed (@Jawad-H)
- [#4580](https://github.com/rollup/rollup/pull/4580): Update dependencies (@lukastaegert)
- [#4584](https://github.com/rollup/rollup/pull/4584): Documentation clarity and syntax improvements (@berniegp)
- [#4588](https://github.com/rollup/rollup/pull/4588): Use var for IIFE (@lukastaegert)

## 2.77.0

_2022-07-15_

### Features

- Introduce `maxParallelFileOps` to limit both read and write operations, default to 20 and replaces `maxParallelFileRead` (#4570)

### Bug Fixes

- Avoid including variables referenced from return statements that are never reached (#4573)

### Pull Requests

- [#4570](https://github.com/rollup/rollup/pull/4570): Introduce maxParallelFileOps to limit parallel writes ( @lukastaegert)
- [#4572](https://github.com/rollup/rollup/pull/4572): Document more ways to read package.json in ESM (@berniegp)
- [#4573](https://github.com/rollup/rollup/pull/4573): Do not include unused return expressions (@lukastaegert)

## 2.76.0

_2022-07-08_

### Features

- Allow setting a `sourcmapBaseUrl` for absolute paths in sourcemaps (#4527)

### Bug Fixes

- Support absolute CLI plugin paths on Windows (#4533)

### Pull Requests

- [#4527](https://github.com/rollup/rollup/pull/4527): Add sourcemapBaseUrl option (@nickgarlis)
- [#4533](https://github.com/rollup/rollup/pull/4533): Add support for absolute plugin paths (@ygoe)
- [#4538](https://github.com/rollup/rollup/pull/4538): chore: Included githubactions in the dependabot config ( @naveensrinivasan)
- [#4546](https://github.com/rollup/rollup/pull/4546): Adapt Node versions on CI to prepare for v3 (@lukastaegert)
- [#4556](https://github.com/rollup/rollup/pull/4556): Improve error message for invalid patterns (@DysphoricUnicorn)
- [#4559](https://github.com/rollup/rollup/pull/4559): Update dependencies (@lukastaegert)
- [#4560](https://github.com/rollup/rollup/pull/4560): Bump peter-evans/create-or-update-comment from 1 to 2 ( @dependabot)
- [#4561](https://github.com/rollup/rollup/pull/4561): Bump peter-evans/find-comment from 1 to 2 (@dependabot)
- [#4562](https://github.com/rollup/rollup/pull/4562): Bump codecov/codecov-action from 1 to 3 (@dependabot)

## 2.75.7

_2022-06-20_

### Bug Fixes

- Mark Array.prototype.group/groupToMap as side effect free. (#4531)

### Pull Requests

- [#4523](https://github.com/rollup/rollup/pull/4523): chore: remove source map workaround, bump deps (@dnalborczyk)
- [#4525](https://github.com/rollup/rollup/pull/4525): Add regression tests for instanceof (@lukastaegert)
- [#4528](https://github.com/rollup/rollup/pull/4528): chore: Set permissions for GitHub actions (@naveensrinivasan)
- [#4531](https://github.com/rollup/rollup/pull/4531): fix: rename Array.prototype.group/groupToMap (@dnalborczyk)
- [#4535](https://github.com/rollup/rollup/pull/4535): chore: bump resolve from 1.22.0 to 1.22.1 (@pos777)

## 2.75.6

_2022-06-07_

### Bug Fixes

- Properly deoptimize "this" when using member expressions with getters/setters in for loops and update expressions ( #4522)

### Pull Requests

- [#4522](https://github.com/rollup/rollup/pull/4522): Refactor side effect handling for property interactions ( @lukastaegert)

## 2.75.5

_2022-06-01_

### Bug Fixes

- Avoid crashes when using logical expressions for unused constructor arguments (#4519)
- Fix missing parameter defaults for calls from try statements and functions returned by functions (#4520)

### Pull Requests

- [#4519](https://github.com/rollup/rollup/pull/4519): Try to make logical expression deoptimization more robust ( @lukastaegert)
- [#4520](https://github.com/rollup/rollup/pull/4520): Roll back parameter default tree shaking (@lukastaegert)

## 2.75.4

_2022-05-31_

### Bug Fixes

- Ensure parameter defaults are retained when a function is used as an object property (#4516)

### Pull Requests

- [#4516](https://github.com/rollup/rollup/pull/4516): Deoptimize parameter defaults when referenced from object/array/class literals (@lukastaegert)

## 2.75.3

_2022-05-29_

### Bug Fixes

- Retain parameter defaults for functions that are defaults themselves (#4515)
- Track mutations for objects as default values (#4515)

### Pull Requests

- [#4515](https://github.com/rollup/rollup/pull/4515): Ensure parameter defaults are deoptimized (@lukastaegert)

## 2.75.1

_2022-05-28_

### Pull Requests

- [#4513](https://github.com/rollup/rollup/pull/4513): Update link to node polyfill repo (@lukastaegert)

## 2.75.0

_2022-05-27_

### Features

- Re-implement default parameter tree-shaking for top-level functions (#4510)
- Do not consider calling string methods like `.trim()` on template literals a side effect (#4511)

### Pull Requests

- [#4510](https://github.com/rollup/rollup/pull/4510): Tree-shake parameter defaults (replaces #4498) (@lukastaegert)
- [#4511](https://github.com/rollup/rollup/pull/4511): Tree-shake side-effect-free string methods on template literals ( @lukastaegert)

## 2.74.1

_2022-05-19_

### Bug Fixes

- Revert #4498 until some issues are understood and resolved

## 2.74.0

_2022-05-19_

### Features

- Remove unneeded default values for function parameters (#4498)

### Bug Fixes

- Use a consistent mechanism to resolve the config file to avoid issues on Windows (#4501)
- Avoid an inaccurate warning about an event emitter leak for complicated builds (#4502)
- Ensure that reexporting values from other chunks via dynamic imports does not reference non-imported variables (#4499)

### Pull Requests

- [#4498](https://github.com/rollup/rollup/pull/4498): Tree shake parameter defaults (@lukastaegert)
- [#4499](https://github.com/rollup/rollup/pull/4499): Ensure reexports are available for namespaces (@lukastaegert)
- [#4501](https://github.com/rollup/rollup/pull/4501): fix: config path problem on windows (@pos777)
- [#4502](https://github.com/rollup/rollup/pull/4502): Avoid maximum listeners exceeded warning (@lukastaegert)

## 2.73.0

_2022-05-13_

### Features

- Do not treat Object.defineProperty/ies as side effect when called on an unused object (#4493)
- Do not assume that assigning a property can create a getter with side effects (#4493)
- Do not treat string.prototype.replace(All) as side effect when used with two literals (#4493)

### Bug Fixes

- Detect side effects when manually declaring getters on functions (#4493)

### Pull Requests

- [#4493](https://github.com/rollup/rollup/pull/4493): Handle getters on functions and improve property deoptimization ( @lukastaegert)
- [#4494](https://github.com/rollup/rollup/pull/4494): Do not treat string.replace as side effect when used with a literal (@lukastaegert)
- [#4495](https://github.com/rollup/rollup/pull/4495): Update docs for --configPlugin using typescript ( @Jimmydalecleveland)

## 2.72.1

_2022-05-07_

### Bug Fixes

- Improve tree-shaking of classes with super classes in certain scenarios (#4489)

### Pull Requests

- [#4489](https://github.com/rollup/rollup/pull/4489): Do not deoptimize entire super class when adding a property ( @lukastaegert)

## 2.72.0

_2022-05-05_

### Features

- Add CLI hooks to run external commands at certain points in watch mode (#4457)

### Bug Fixes

- Fix an issue that could accidentally treat relevant assignments as side effect free (#4486)

### Pull Requests

- [#4457](https://github.com/rollup/rollup/pull/4457): feat: CLI event hook flags (@Harris-Miller)
- [#4486](https://github.com/rollup/rollup/pull/4486): Fix reassignment tracking (@lukastaegert)

## 2.71.1

_2022-04-30_

### Bug Fixes

- Allow importing loadConfigFile without extension (#4483)

### Pull Requests

- [#4483](https://github.com/rollup/rollup/pull/4483): Add exports exception for loadConfigFile (@lukastaegert)

## 2.71.0

_2022-04-30_

## Features

- Mark `Object.hasOwn` as pure (#4482)

### Bug Fixes

- Prevent infinite recursion and display proper warning for recursive reexports (#4472)
- Fix type issue in TypeScript nightly (#4471)

### Pull Requests

- [#4467](https://github.com/rollup/rollup/pull/4467): docs: update deprecated option in tools.md (@kimjh96)
- [#4471](https://github.com/rollup/rollup/pull/4471): Fix: tsc did not build (@frank-dspeed)
- [#4472](https://github.com/rollup/rollup/pull/4472): Throw proper error when indirectly reexporting a recursive binding (@lukastaegert)
- [#4475](https://github.com/rollup/rollup/pull/4475): chore: bump deps (#4475) (@dnalborczyk)
- [#4477](https://github.com/rollup/rollup/pull/4477): chore: bump github actions (@dnalborczyk)
- [#4478](https://github.com/rollup/rollup/pull/4478): ci: test with node.js v18, remove v17 (@dnalborczyk)
- [#4479](https://github.com/rollup/rollup/pull/4479): chore(repo): replace `git.io` in the issue template (@SukkaW)
- [#4482](https://github.com/rollup/rollup/pull/4482): feat: add Object.hasOwn as pure function (@dnalborczyk)

## 2.70.2

_2022-04-15_

### Bug Fixes

- Do not enforce undefined return values in TypeScript types (#4463)

### Pull Requests

- [#4463](https://github.com/rollup/rollup/pull/4463): use void for options hook instead of undefined (@ycmjason)

## 2.70.1

_2022-03-14_

### Bug Fixes

- Handle unfinished hook action errors as regular errors and avoid console logging (#4434)
- Allow access to "dist" folder in a Node 17 compatible way (#4436)

### Pull Requests

- [#4434](https://github.com/rollup/rollup/pull/4434): Track unfinished hook actions as regular errors (@lukastaegert)
- [#4436](https://github.com/rollup/rollup/pull/4436): Update package.json (@frank-dspeed)

## 2.70.0

_2022-03-07_

### Features

- Make the `watchChange` and `closeWatcher` hooks asynchronous and make Rollup wait for these hooks before continuing ( #4427)

### Bug Fixes

- Do not abort watch mode for errors in `watchChange` but display them properly (#4427)

### Pull Requests

- [#4427](https://github.com/rollup/rollup/pull/4427): Do not abort watch mode on errors in watchChange (@lukastaegert)

## 2.69.2

_2022-03-06_

### Bug Fixes

- Mark `Object.entries` and `Object.fromEntries` as pure (#4429)
- Make sure new properties on Array.prototype and Object.prototype are not evaluated as "undefined" (#4428)

### Pull Requests

- [#4428](https://github.com/rollup/rollup/pull/4428): Treat unknown prototype props as unknown (@lukastaegert)
- [#4429](https://github.com/rollup/rollup/pull/4429): Treat unknown prototype props as unknown (@869288142)

## 2.69.1

_2022-03-04_

### Bug Fixes

- Approximate source position instead of ignoring it when using a low-resolution source map in a transform hook (#4334)

### Pull Requests

- [#4334](https://github.com/rollup/rollup/pull/4334): fix(sourcemap): fall back to low-resolution line mapping ( @aleclarson and @lukastaegert)

## 2.69.0

_2022-03-02_

### Features

- Introduce new `output.generatedCode.symbols` to control the usage of Symbols in Rollup-generated code (#4378)
- soft-deprecate `output.namespaceToStringTag` in favor of `output.generatedCode.symbols` (#4378)

### Bug Fixes

- Properly handle `./` and `../` as external dependencies (#4419)
- Make generated "Module" namespace toStringTag non-enumerable for correct Object.assign/spread behaviour (#4378)
- Add file name to error when top-level-await is used in disallowed formats (#4421)

### Pull Requests

- [#4378](https://github.com/rollup/rollup/pull/4378): Make namespace @@toStringTag "Module" non-enumerable ( @dnalborczyk and @lukastaegert)
- [#4413](https://github.com/rollup/rollup/pull/4413): refactor: some code and type fixes (@dnalborczyk)
- [#4418](https://github.com/rollup/rollup/pull/4418): chore: bump deps (@dnalborczyk)
- [#4419](https://github.com/rollup/rollup/pull/4419): Properly handle upper directories as external dependencies ( @lukastaegert)
- [#4421](https://github.com/rollup/rollup/pull/4421): Improve the error prompt and output the error file name ( @caoxiemeihao)
- [#4423](https://github.com/rollup/rollup/pull/4423): Update 999-big-list-of-options.md (@leoj3n)

## 2.68.0

_2022-02-22_

### Features

- provide information about cached import resolutions in `shouldTransformCachedModule` (#4414)
- Add "types" field to Rollup's package exports (#4416)

### Pull Requests

- [#4410](https://github.com/rollup/rollup/pull/4410): refactor: use map for declarations and name suggestions ( @dnalborczyk)
- [#4411](https://github.com/rollup/rollup/pull/4411): refactor: use map for namespace reexports by name (@dnalborczyk)
- [#4412](https://github.com/rollup/rollup/pull/4412): refactor: use includes where appropriate (@dnalborczyk)
- [#4414](https://github.com/rollup/rollup/pull/4414): Add resolved sources to shouldTransformCachedModule ( @lukastaegert)
- [#4416](https://github.com/rollup/rollup/pull/4416): Add Typescript 4.5 nodenext node12 module resolution support ( @frank-dspeed)

## 2.67.3

_2022-02-18_

### Bug Fixes

- Do not swallow other errors when unfinished hook actions are detected (#4409)
- Add additional information to output when there are unfinished hook actions (#4409)

### Pull Requests

- [#4399](https://github.com/rollup/rollup/pull/4399): docs: remove const (@TrickyPi)
- [#4401](https://github.com/rollup/rollup/pull/4401): Improve test stability by getting independent of module id ordering in more places (@lukastaegert)
- [#4403](https://github.com/rollup/rollup/pull/4403): fix: remove unnecessary property descriptor spread (@dnalborczyk)
- [#4404](https://github.com/rollup/rollup/pull/4404): refactor: use map for import descriptions + re-export descriptions (@dnalborczyk)
- [#4405](https://github.com/rollup/rollup/pull/4405): refactor: module exports to map (@dnalborczyk)
- [#4406](https://github.com/rollup/rollup/pull/4406): Fix a typo in 'Direct plugin communication' code example ( @younesmln)
- [#4407](https://github.com/rollup/rollup/pull/4407): Document how resolveId is cached (@lukastaegert)
- [#4409](https://github.com/rollup/rollup/pull/4409): Print ids for unfinished moduleParsed and shouldTransformCachedModule hooks (@lukastaegert)

## 2.67.2

_2022-02-10_

### Bug Fixes

- Ensure consistent order between manual chunks to fix hashing issues (#4397)

### Pull Requests

- [#4390](https://github.com/rollup/rollup/pull/4390): refactor: add @types/estree explicitly, fix dynamic type imports (@dnalborczyk)
- [#4391](https://github.com/rollup/rollup/pull/4391): chore: remove acorn-walk ambient type definitions (@dnalborczyk)
- [#4397](https://github.com/rollup/rollup/pull/4397): Sort manual chunks generated via a function by name ( @lukastaegert)

## 2.67.1

_2022-02-07_

### Bug Fixes

- Make chunk file and variable names more deterministic when emitting chunks (#4386)
- Improve default module resolver performance by using non-blocking IO (#4386)

### Pull Requests

- [#4373](https://github.com/rollup/rollup/pull/4373): fix: even more types (@dnalborczyk)
- [#4382](https://github.com/rollup/rollup/pull/4382): Update contribution tut link desc (@lemredd)
- [#4383](https://github.com/rollup/rollup/pull/4383): chore: bump deps (@dnalborczyk)
- [#4384](https://github.com/rollup/rollup/pull/4384): chore: move "wait" to utils + re-use (@dnalborczyk)
- [#4385](https://github.com/rollup/rollup/pull/4385): refactor: convert watch tests to async functions (@dnalborczyk)
- [#4386](https://github.com/rollup/rollup/pull/4386): refactor: use fs.promises in resolve id, Part 4 (@dnalborczyk and @lukastaegert)
- [#4389](https://github.com/rollup/rollup/pull/4389): refactor: use fs.promises in generate license file, rollup config, Part 5 (@dnalborczyk)

## 2.67.0

_2022-02-02_

### Features

- Improve side effect detection when using Array.prototype.groupBy/groupByToMap (#4360)
- Allow changing `moduleSideEffects` at any time during the build (#4379)
- Soft-deprecate `ModuleInfo.hasModuleSideEffects` in favour of `ModuleInfo.moduleSideEffects` (#4379)

### Bug Fixes

- Do not include queries and hashes in generated file names when preserving modules (#4374)

### Pull Requests

- [#4319](https://github.com/rollup/rollup/pull/4319): refactor: use fs, fs-extra, remove sander (@dnalborczyk)
- [#4360](https://github.com/rollup/rollup/pull/4360): feat: add Array.prototype.groupBy/groupByToMap (@dnalborczyk)
- [#4361](https://github.com/rollup/rollup/pull/4361): fix: more types (@dnalborczyk)
- [#4369](https://github.com/rollup/rollup/pull/4369): fix: remove acorn-walk patch (@dnalborczyk)
- [#4371](https://github.com/rollup/rollup/pull/4371): refactor: use fs.promises in cli/run (@dnalborczyk)
- [#4372](https://github.com/rollup/rollup/pull/4372): refactor: use fs.promises in module loader (@dnalborczyk)
- [#4374](https://github.com/rollup/rollup/pull/4374): Ignore queries and hashes in file names when preserving modules ( @lukastaegert)
- [#4375](https://github.com/rollup/rollup/pull/4375): Fix typo in \_config.js (@eltociear)
- [#4376](https://github.com/rollup/rollup/pull/4376): refactor: fs.promises, move mkdir to writeoutputfile, Part 3 ( @dnalborczyk)
- [#4379](https://github.com/rollup/rollup/pull/4379): Deprecate hasModuleSideEffects in favor of moduleSideEffects and ensure it is mutable on ModuleInfo (@lukastaegert)

## 2.66.1

_2022-01-25_

### Bug Fixes

- Only warn for conflicting names in namespace reexports if it actually causes problems (#4363)
- Only allow explicit exports or reexports as synthetic namespaces and hide them from namespace reexports (#4364)

### Pull Requests

- [#4362](https://github.com/rollup/rollup/pull/4362): refactor: convert exportsByName object to map (@dnalborczyk)
- [#4363](https://github.com/rollup/rollup/pull/4363): Do not warn unnecessarily for namespace conflicts (@lukastaegert)
- [#4364](https://github.com/rollup/rollup/pull/4364): Do not expose synthetic namespace export in entries and namespaces (@lukastaegert)

## 2.66.0

_2022-01-22_

### Features

- Note if a module has a default export in ModuleInfo to allow writing better proxy modules (#4356)
- Add option to wait until all imported ids have been resolved when awaiting `this.load` (#4358)

### Pull Requests

- [#4356](https://github.com/rollup/rollup/pull/4356): Add hasDefaultExport to ModuleInfo (@lukastaegert)
- [#4358](https://github.com/rollup/rollup/pull/4358): Add "resolveDependencies" option to "this.load" (@lukastaegert)

## 2.65.0

_2022-01-21_

### Features

- Add complete import resolution objects to ModuleInfo for use in `this.load` (#4354)

### Bug Fixes

- Use correct context in plugin hooks with `perf: true` (#4357)

### Pull Requests

- [#4351](https://github.com/rollup/rollup/pull/4351): refactor: re-use source mapping url (@dnalborczyk)
- [#4352](https://github.com/rollup/rollup/pull/4352): refactor: replace require-relative with built-in require.resolve (@dnalborczyk)
- [#4353](https://github.com/rollup/rollup/pull/4353): chore: bump deps (@dnalborczyk)
- [#4354](https://github.com/rollup/rollup/pull/4354): Add importedIdResolutions to moduleInfo (@lukastaegert)
- [#4355](https://github.com/rollup/rollup/pull/4355): chore: remove external from config (@dnalborczyk)
- [#4357](https://github.com/rollup/rollup/pull/4357): fix: timed plugin context (@dnalborczyk)

## 2.64.0

_2022-01-14_

### Features

- Allow inspecting cached modules and forcing them to be transformed again via shouldTransformCachedModule (#4320)
- Do not wait for the config file to be parsed in watch mode if it is updated before that (#4344)

### Bug Fixes

- Do not mutate objects returned as `meta` from the resolveId hook (#4347)

### Pull Requests

- [#4326](https://github.com/rollup/rollup/pull/4326): refactor: type fixes (@dnalborczyk)
- [#4339](https://github.com/rollup/rollup/pull/4339): More watch test stabilization (@lukastaegert)
- [#4340](https://github.com/rollup/rollup/pull/4340): refactor: performance timers for node.js and browser ( @dnalborczyk)
- [#4341](https://github.com/rollup/rollup/pull/4341): Implement shouldTransformCachedModule hook (@lukastaegert)
- [#4344](https://github.com/rollup/rollup/pull/4344): Directly restart Rollup when config file change is detected in watch mode (@lukastaegert)
- [#4347](https://github.com/rollup/rollup/pull/4347): Create a shallow copy when returning meta from resolveId ( @lukastaegert)

## 2.63.0

_2022-01-04_

### Features

- Report a helpful error if rollup exits due to an empty event loop when using `this.load` (#4320)
- Allow directly mutating ModuleInfo.meta for modules and never replace this object (#4328)
- Detect additional side effect free array prototype methods (#4332)

### Bug Fixes

- Do not watch if CLI watch options are specified but `--watch` is missing (#4335)

### Pull Requests

- [#4320](https://github.com/rollup/rollup/pull/4320): Detect unfulfilled async hook actions and report error on exit ( @kzc)
- [#4328](https://github.com/rollup/rollup/pull/4328): Make initial ModuleInfo.meta mutable and maintain object identity (@lukastaegert)
- [#4318](https://github.com/rollup/rollup/pull/4318): Stabilize watch tests (@lukastaegert)
- [#4331](https://github.com/rollup/rollup/pull/4331): Improve JS docs example (@lukastaegert)
- [#4332](https://github.com/rollup/rollup/pull/4332): add support for Array.prototype.findLast,findLastIndex ( @dnalborczyk)
- [#4333](https://github.com/rollup/rollup/pull/4333): convert utils.transform to async function (@dnalborczyk)
- [#4335](https://github.com/rollup/rollup/pull/4335): Do not watch unless --watch is specified explicitly ( @lukastaegert)
- [#4338](https://github.com/rollup/rollup/pull/4338): Add build delay for plugin event test (@lukastaegert)

## 2.62.0

_2021-12-24_

### Features

- Mark additional string prototype methods as side-effect-free and correct typings of existing ones (#4299)
- Mark additional array prototype methods as side-effect-free and correct typings of existing ones (#4309)
- Expose if a module is included after tree-shaking in its ModuleInfo (#4305)

### Bug Fixes

- Fix how fsevents is included to improve watch mode on MacOS (#4312)

### Pull Requests

- [#4299](https://github.com/rollup/rollup/pull/4299): Add additional string prototype methods (@dnalborczyk)
- [#4300](https://github.com/rollup/rollup/pull/4300): Bump deps, fix expected test result for core-js (@dnalborczyk)
- [#4302](https://github.com/rollup/rollup/pull/4302): Replace type assertion with type guard (@dnalborczyk)
- [#4304](https://github.com/rollup/rollup/pull/4304): Re-use reserved names set (@dnalborczyk)
- [#4305](https://github.com/rollup/rollup/pull/4305): Expose isIncluded in module info (@william57m)
- [#4306](https://github.com/rollup/rollup/pull/4306): Fix git line breaks on windows (@dnalborczyk)
- [#4307](https://github.com/rollup/rollup/pull/4307): Add macos to pipeline (@dnalborczyk)
- [#4309](https://github.com/rollup/rollup/pull/4309): Add additional array prototype methods (@dnalborczyk)
- [#4311](https://github.com/rollup/rollup/pull/4311): Add Deno instructions to docs (@jespertheend)
- [#4312](https://github.com/rollup/rollup/pull/4312): fsevents integration (@dnalborczyk)
- [#4313](https://github.com/rollup/rollup/pull/4313): Remove non-existing static functions from known globals ( @dnalborczyk)

## 2.61.1

_2021-12-11_

### Bug Fixes

- Only resolve this.load once the code of the module is available (#4296)

### Pull Requests

- [#4296](https://github.com/rollup/rollup/pull/4296): Make sure this.load waits for modules that are already loading ( @lukastaegert)
- [#4298](https://github.com/rollup/rollup/pull/4298): use set for reserved words (@dnalborczyk)

## 2.61.0

_2021-12-09_

### Features

- Support ergonomic brand checks for private fields (#4293)

### Bug Fixes

- Improve handling of directory creation on systems with restrictive open files limit (#4288)

### Pull Requests

- [#4288](https://github.com/rollup/rollup/pull/4288): modifymkdirpath (@mgrabowski84)
- [#4293](https://github.com/rollup/rollup/pull/4293): bump deps (@dnalborczyk)

## 2.60.2

_2021-11-30_

### Bug Fixes

- Produce correct output when dynamic import paths contain quotes (#4286)

### Pull Requests

- [#4286](https://github.com/rollup/rollup/pull/4286): Escape dynamic import paths (@danielroe)

## 2.60.1

_2021-11-22_

### Bug Fixes

- Make sure virtual files have proper file extensions when preserving modules (#4270)

### Pull Requests

- [#4270](https://github.com/rollup/rollup/pull/4270): Use entryFileNames when generating filenames for virtual modules (@BPScott)

## 2.60.0

_2021-11-11_

### Features

- Add `this.load` context function to load, transform and parse modules without adding them to the graph (#4234)
- Sanitize non-url-safe characters in generated chunk names by default (#4262)
- Support ESM plugins via command line (#4265)

### Pull Requests

- [#4234](https://github.com/rollup/rollup/pull/4234): Plugin context function for pre-loading modules (@lukastaegert)
- [#4262](https://github.com/rollup/rollup/pull/4262): exclude invalid URL chars (@danielroe)
- [#4265](https://github.com/rollup/rollup/pull/4265): support loading ESM plugins from the CLI via --plugin (@kzc)

## 2.59.0

_2021-11-01_

### Features

- Support static class initialization blocks (#4249)

### Bug Fixes

- Fix an issue with the CommonJS plugin when module.exports has inherited properties (#4256)

### Pull Requests

- [#4236](https://github.com/rollup/rollup/pull/4236): typescript bug class field initialization order (@dnalborczyk)
- [#4249](https://github.com/rollup/rollup/pull/4249): Support for class static initialization block (@dnalborczyk and @lukastaegert)
- [#4256](https://github.com/rollup/rollup/pull/4256): Skip inherited properties in synthetic namespaces (@lukastaegert)

## 2.58.3

_2021-10-25_

### Bug Fixes

- Republish 2.58.1 with npm 6 as files were missing

## 2.58.2

_2021-10-25_

### Bug Fixes

- Republish 2.58.1 as files were missing

## 2.58.1

_2021-10-25_

### Bug Fixes

- Fix an issue with the CommonJS plugin when module.exports is falsy (#4247)

### Pull Requests

- [#4247](https://github.com/rollup/rollup/pull/4247): Handle falsy synthetic namespaces (@lukastaegert)

## 2.58.0

_2021-10-01_

### Features

- Add a flag to more reliably identify entry points in the `resolveId` hook (#4230)

### Pull Requests

- [#4230](https://github.com/rollup/rollup/pull/4230): Add isEntry flag to resolveId and this.resolve (@lukastaegert)
- [#4233](https://github.com/rollup/rollup/pull/4233): Remove unused rollup-plugin-typescript ambient module types ( @dnalborczyk)
- [#4235](https://github.com/rollup/rollup/pull/4235): Update dependencies (@lukastaegert)

## 2.57.0

_2021-09-22_

### Features

- Add `generatedCode` option to allow Rollup to use es2015 features for smaller output and more efficient helpers ( #4215)
- Improve AMD and SystemJS parsing performance by wrapping relevant functions in parentheses (#4215)
- Using `preferConst` will now show a warning with `strictDeprecations: true` (#4215)

### Bug Fixes

- Improve ES3 syntax compatibility by more consequently quoting reserved words as props in generated code (#4215)
- Do not use `Object.assign` in generated code to ensure ES5 compatibility without the need for polyfills (#4215)
- Support live-bindings in dynamic namespace objects that contain reexported external or synthetic namespaces (#4215)
- Use correct "this" binding in dynamic import expressions for CommonJS and AMD (#4215)
- Properly handle `shimMissingExports` for exports that are only used internally (#4215)
- Prevent unhandled rejection for failed module parsing (#4228)

### Pull Requests

- [#4212](https://github.com/rollup/rollup/pull/4212): chore: remove unused ambient types (@dnalborczyk)
- [#4215](https://github.com/rollup/rollup/pull/4215): Use ES2015 features in generated code snippets (@lukastaegert)
- [#4219](https://github.com/rollup/rollup/pull/4219): chore: bump rollup typescript, remove unused micromatch ( @dnalborczyk)
- [#4220](https://github.com/rollup/rollup/pull/4220): chore: use forceConsistentCasingInFileNames in ts-config ( @dnalborczyk)
- [#4224](https://github.com/rollup/rollup/pull/4224): prepare for useDefineForClassFields (@dnalborczyk)
- [#4228](https://github.com/rollup/rollup/pull/4228): fix: prevent UnhandledPromiseRejectionWarning when module resolution/parsing fails (@kherock)

## 2.56.3

_2021-08-23_

### Bug Fixes

- Make sure moduleInfo contains complete information about imported ids in the moduleParsed hook (#4208)

### Pull Requests

- [#4208](https://github.com/rollup/rollup/pull/4208): `ModuleInfo.importedIds` will return null if `resolvedIds[source]` is undefined (@FoxDaxian and @lukastaegert)

## 2.56.2

_2021-08-10_

### Bug Fixes

- Check if after simplification, an object pattern would become an expression statement or arrow function return value ( #4204)

### Pull Requests

- [#4204](https://github.com/rollup/rollup/pull/4204): Do not create invalid code when simplifying object pattern assignments (@lukastaegert)

## 2.56.1

_2021-08-08_

### Bug Fixes

- Fix rendering of SystemJS export declarations initialized with a simplifiable expression (#4202)

### Pull Requests

- [#4202](https://github.com/rollup/rollup/pull/4202): Fix incorrect rendering of export declarations in SystemJS ( @lukastaegert)

## 2.56.0

_2021-08-05_

### Features

- Create more efficient code for SystemJS exports (#4199)
- Extend `maxParallelFileReads` option to also throttle plugin load hooks (#4200)

### Bug Fixes

- Return correct value for postfix update expressions of exported variables (#4194)

### Pull Requests

- [#4199](https://github.com/rollup/rollup/pull/4199): Refine SystemJS export rendering (@lukastaegert)
- [#4200](https://github.com/rollup/rollup/pull/4200): Restrict parallel execution of load hook (@schummar)

## 2.55.1

_2021-07-29_

### Bug Fixes

- Improve CLI warning message for unused external imports (#4194)

### Pull Requests

- [#4194](https://github.com/rollup/rollup/pull/4194): Align batch warning for UNUSED_EXTERNAL_IMPORT to individual warning (@benmccann)

## 2.55.0

_2021-07-28_

### Features

- Support default export live-bindings when generating ESM output (#4182)

### Bug Fixes

- Always write `["default"]` as computed property when used as named export (#4182)
- Do not mask default export TDZ errors (#4182)

### Pull Requests

- [#4182](https://github.com/rollup/rollup/pull/4182): Use mutable bindings for default exports (@lukastaegert)

## 2.54.0

_2021-07-25_

### Features

- Extend UMD import.meta.url polyfill to support web workers (#4186)

### Bug Fixes

- Resolve an issue where certain uses of classes could lead to an infinite recursion (#4189)

### Pull Requests

- [#4186](https://github.com/rollup/rollup/pull/4186): Fix UMD import.meta.url inside web workers (@ceifa)
- [#4188](https://github.com/rollup/rollup/pull/4188): Fix typo in renderHelpers.ts (@eltociear)
- [#4189](https://github.com/rollup/rollup/pull/4189): Move long path recursion prevention to MemberExpression ( @lukastaegert)
- [#4190](https://github.com/rollup/rollup/pull/4190): Stop recommending node-builtins (@curran)

## 2.53.3

_2021-07-21_

### Bug Fixes

- Solve an issue that could lead to severe memory issues and crashes when there are a lot of hoisted variables (#4183)

### Pull Requests

- [#4183](https://github.com/rollup/rollup/pull/4183): Avoid memory issues with hoisted variables (@lukastaegert)

## 2.53.2

_2021-07-15_

### Bug Fixes

- Identify additional TDZ situations in functions that are run more than once (#4177)
- Fix a scoping issue when a variable inside a catch scope matches the scope parameter's name (#4178)

### Pull Requests

- [#4177](https://github.com/rollup/rollup/pull/4177): Fix additional let/var init bugs (@kzc)
- [#4178](https://github.com/rollup/rollup/pull/4178): Correctly create outside variable when shadowed by catch parameter (@lukastaegert)

## 2.53.1

_2021-07-11_

### Bug Fixes

- Do not omit namespace reexports when `treeshake` is `false` (#4175)

### Pull Requests

- [#4175](https://github.com/rollup/rollup/pull/4175): Generate namespace objects when not tree-shaking (@lukastaegert)

## 2.53.0

_2021-07-09_

### Features

- Add `maxParallelFileReads` option to limit read operations with a default of 20 (#4170)

### Pull Requests

- [#4170](https://github.com/rollup/rollup/pull/4170): Limit parallel file reads to prevent "EMFILE: too many open files" error (@schummar)

## 2.52.8

_2021-07-07_

### Bug Fixes

- Automatically handle many use `var` before declaration and TDZ access scenarios correctly without the need for `treeshake.correctVarValueBeforeDeclaration` (#4148)

### Pull Requests

- [#4148](https://github.com/rollup/rollup/pull/4148): Fix var/const/let variable use before declaration (@kzc and @lukastaegert)

## 2.52.7

_2021-07-02_

### Bug Fixes

- Fix an issue where reassignments where not tracked through async function returns (#4163)

### Pull Requests

- [#4163](https://github.com/rollup/rollup/pull/4163): Deoptimize return values of async functions (@lukastaegert)

## 2.52.6

_2021-07-01_

### Bug Fixes

- Fix an issue where reassignments where not tracked through an await expression (#4162)

### Pull Requests

- [#4162](https://github.com/rollup/rollup/pull/4162): doptimize awaited expressions (@lukastaegert)

## 2.52.5

_2021-07-01_

### Bug Fixes

- Properly display parser errors not tied to a code location (#4160)

### Pull Requests

- [#4160](https://github.com/rollup/rollup/pull/4160): fix: max stack call error is caught on locate (@semoal)

## 2.52.4

_2021-06-30_

### Bug Fixes

- Fix an error when external namespaces are reexported across several files (#4159)

### Pull Requests

- [#4159](https://github.com/rollup/rollup/pull/4159): Properly handle double reexports from external namespaces ( @lukastaegert)

## 2.52.3

_2021-06-25_

### Bug Fixes

- Fix an issue where code was wrongly removed when using vars in nested scopes (#4149)

### Pull Requests

- [#4149](https://github.com/rollup/rollup/pull/4149): Make sure the initializer of hoisted variables is deoptimized ( @lukastaegert)

## 2.52.2

_2021-06-21_

### Bug Fixes

- Support falsy plugins in types (#4144)
- Do not require return value in renderChunkHook type (#4144)

### Pull Requests

- [#4144](https://github.com/rollup/rollup/pull/4144): Use TypeScript config and improve some types (@lukastaegert)

## 2.52.1

_2021-06-17_

### Bug Fixes

- Fix a memory leak in watch mode (#4142)

### Pull Requests

- [#4142](https://github.com/rollup/rollup/pull/4142): Make array and object prototype singletons immutable for now ( @lukastaegert)

## 2.52.0

_2021-06-16_

### Features

- Add `--configPlugin` CLI option to apply plugins to the config file for e.g. TypeScript configs (#3835)
- Add "safest" and "smallest" presets to tree-shaking options for easier configuration (#4131)
- Add `treeshake.correctVarValueBeforeDeclaration` option to deoptimize `var` declarations (#4139)

### Pull Requests

- [#3835](https://github.com/rollup/rollup/pull/3835): Add typescript config support (@TheRealSyler)
- [#4131](https://github.com/rollup/rollup/pull/4131): Add presets to the tree-shaking options (@lukastaegert)
- [#4139](https://github.com/rollup/rollup/pull/4139): Add option to deoptimize var declarations for tree-shaking ( @lukastaegert)
- [#4141](https://github.com/rollup/rollup/pull/4141): Update dependencies (@lukastaegert)

## 2.51.2

_2021-06-11_

### Bug Fixes

- Include modules imported from no-treeshake modules even if they would be empty (#4138)

### Pull Requests

- [#4138](https://github.com/rollup/rollup/pull/4138): Include all dependencies from modules with no-treeshake ( @lukastaegert)

## 2.51.1

_2021-06-08_

### Bug Fixes

- Fix error when using `defineConfig` (#4134)

### Pull Requests

- [#4134](https://github.com/rollup/rollup/pull/4134): export `rollup.defineConfig` at runtime (@mshrtsr)

## 2.51.0

_2021-06-06_

### Features

- Add a helper for IntelliSense support in config files (#4127)

### Bug Fixes

- Improve performance when generating source maps (#4122)

### Pull Requests

- [#4122](https://github.com/rollup/rollup/pull/4122): User Map to optimize performance (@izevo)
- [#4127](https://github.com/rollup/rollup/pull/4127): Export defineConfig defines the auxiliary function of the configuration (@rxliuli)

## 2.50.6

_2021-06-03_

### Bug Fixes

- Do not consider the object spread operator as side effect when `propertyReadSideEffects` are false (#4119)
- Detect side effects when returning thenables from async arrow functions (#4120)

### Pull Requests

- [#4119](https://github.com/rollup/rollup/pull/4119): Respect propertyReadSideEffects in spread elements ( @lukastaegert)
- [#4120](https://github.com/rollup/rollup/pull/4120): Detect async arrow thenable side effects (@lukastaegert)

## 2.50.5

_2021-05-30_

### Bug Fixes

- Detect side effects when accessing thenables (#4115)

### Pull Requests

- [#4114](https://github.com/rollup/rollup/pull/4114): use `colorette` instead of `turbocolor` (@ryuever)
- [#4115](https://github.com/rollup/rollup/pull/4115): Tracks side effects of thenables (@lukastaegert)

## 2.50.4

_2021-05-29_

### Bug Fixes

- Fix a situation where tree-shaking would stop including nodes prematurely (#4111)
- Track mutations and accessor side effects when using `__proto__` in an object literal (#4112)
- Check for getter effects when spreading an object (#4113)

### Pull Requests

- [#4111](https://github.com/rollup/rollup/pull/4111): Always request a new tree-shaking pass when deoptimizations of a node are first included (@lukastaegert)
- [#4112](https://github.com/rollup/rollup/pull/4112): Actually set the prototype when using a **proto** property ( @lukastaegert)
- [#4113](https://github.com/rollup/rollup/pull/4113): Track access side effects when using object spread operator ( @lukastaegert)

## 2.50.3

_2021-05-28_

### Bug Fixes

- Wrap parentheses around leading elements in simplified sequence expressions if this would otherwise lead to invalid code (#4110)
- Do not associate block soped variables in catch clauses with the clause parameter (#4108)
- Do not associate hoisted variables in catch clauses with outside variables if they match the parameter (#4108)
- Use correct "this" context for tagged template literal member expressions in simplified sequences (#4110)

### Pull Requests

- [#4108](https://github.com/rollup/rollup/pull/4108): Correctly handle catch declarations (@lukastaegert)
- [#4110](https://github.com/rollup/rollup/pull/4110): Invalid sequence expression simplification (@lukastaegert)

## 2.50.2

_2021-05-27_

### Bug Fixes

- Avoid unnecessary side effects when using methods like `.filter` and `.map` (#4103)
- Avoid crash when a module with moduleSideEffects no-treeshake imports a tree-shaken module (#4104)

### Pull Requests

- [#4103](https://github.com/rollup/rollup/pull/4103): Do not track side-effect-free array methods as side effects ( @lukastaegert)
- [#4104](https://github.com/rollup/rollup/pull/4104): Fix crash when using inlineDynamicImports with no-treeshake ( @lukastaegert)

## 2.50.1

_2021-05-26_

### Bug Fixes

- Do not associate pure annotations in simplified expressions with wrong elements (#4095)
- Prevent invalid code when simplified conditionals start with an IIFE function expression (#4099)

### Pull Requests

- [#4095](https://github.com/rollup/rollup/pull/4095): Correctly associate pure annotations and remove invalid ones ( @lukastaegert)
- [#4099](https://github.com/rollup/rollup/pull/4099): Wrap leading function expression iifes in conditionals ( @lukastaegert)

## 2.50.0

_2021-05-25_

### Features

- Only include last elements of comma expressions if they are used or have side effects (#4087)

### Bug Fixes

- Prevent a crash that could occur when calling object methods (#4091)

### Pull Requests

- [#4085](https://github.com/rollup/rollup/pull/4085): Switch to ESLint (@lukastaegert)
- [#4087](https://github.com/rollup/rollup/pull/4087): Drop unused last sequence element (@lukastaegert)
- [#4091](https://github.com/rollup/rollup/pull/4091): Prevent crash for recursive "this" deoptimization (@lukastaegert)

## 2.49.0

_2021-05-23_

### Features

- Detect side-effect-free static class methods and properties (#4018)
- Detect side-effect-free array elements (#4018)
- Do not apply deoptimizations from dead code (#4018)

### Bug Fixes

- Handle side effect detection for getters and setters added in untracked code (#4018)
- Track "this" mutations for methods, getters and setters (#4018)

### Pull Requests

- [#4018](https://github.com/rollup/rollup/pull/4018): Class method effects (@marijnh and @lukastaegert)

## 2.48.0

_2021-05-15_

### Features

- Add replacement to conditionally insert asset extensions in `entryFileNames` when preserving modules (#4077)

### Bug Fixes

- Fix crash when dynamically assigning to namespace members (#4070)
- Do not associate pure annotations in front of a semi-colon or comma with succeeding code (#4068)

### Pull Requests

- [#4068](https://github.com/rollup/rollup/pull/4068): ignore invalid trailing pure annotations (@kzc)
- [#4070](https://github.com/rollup/rollup/pull/4070): undefined `deoptimizePath` when the first element is empty string (@si3nloong)
- [#4071](https://github.com/rollup/rollup/pull/4071): add node.js v16 support (@dnalborczyk)
- [#4077](https://github.com/rollup/rollup/pull/4077): Add assetExtname replacement in entryFileNames (@BPScott)
- [#4080](https://github.com/rollup/rollup/pull/4080): Added Rollup logo in README.md (@priyanshurav)
- [#4081](https://github.com/rollup/rollup/pull/4081): fix comment regarding invalid annotation handling (@kzc)

## 2.47.0

_2021-05-04_

### Features

- Warn about ambiguous imports from combined external namespace reexports (#4064)
- In case of combined namespace reexports, always prefer local exports over external namespaces (#4064)
- Treat conflicting names in local namespace reexports as undefined (#4064)

### Pull Requests

- [#4064](https://github.com/rollup/rollup/pull/4064): Prefer locally defined exports and reexports over external namespaces (@lukastaegert)

## 2.46.0

_2021-04-29_

### Features

- Add option to disable file name sanitation (#4058)
- Add information about importers to unused external import warning (#4054)

### Pull Requests

- [#4042](https://github.com/rollup/rollup/pull/4042): Use Github actions only (@lukastaegert)
- [#4045](https://github.com/rollup/rollup/pull/4045): Fix REPL artefact branch reference (@lukastaegert)
- [#4046](https://github.com/rollup/rollup/pull/4046): Use codecov action for coverage (@lukastaegert)
- [#4054](https://github.com/rollup/rollup/pull/4054): Add to `UNUSED_EXTERNAL_IMPORT` warning information about the origin of the problem (@cawa-93)
- [#4058](https://github.com/rollup/rollup/pull/4058): Add sanitizeFileName option (@guybedford)

## 2.45.2

_2021-04-13_

### Bug Fixes

- Do not user a dynamic entry file name for naming a manual chunk (#4040)

### Pull Requests

- [#4040](https://github.com/rollup/rollup/pull/4040): Prioritize manual chunk name over dynamic entry id ( @lukastaegert)

## 2.45.1

_2021-04-10_

### Bug Fixes

- Handle falsy return values from async plugin options hooks (#4039)

### Pull Requests

- [#4039](https://github.com/rollup/rollup/pull/4039): Do not fail when returning null or undefined from an async options hook (@lukastaegert)

## 2.45.0

_2021-04-09_

### Features

- Support private class instance methods and accessors (#4034)

### Pull Requests

- [#4034](https://github.com/rollup/rollup/pull/4034): feat: add support for private class methods (@dnalborczyk)

## 2.44.0

_2021-03-29_

### Features

- Add a new option `makeAbsoluteExternalsRelative` to opt out of renormalizing absolute external ids to relative ids ( #4021)
- Extend the `resolveId` plugin hook to allow forcing or preventing renormalization of absolute external ids (#4021)
- Make the rendered code of individual modules available in the generated bundle (#4028)

### Bug Fixes

- Handle objects with `__proto__` properties correctly (#4019)

### Pull Requests

- [#4019](https://github.com/rollup/rollup/pull/4019): Deoptimize ObjectExpression when a `__proto__` property is present (@marijnh)
- [#4021](https://github.com/rollup/rollup/pull/4021): Improve absolute path handling (@lukastaegert)
- [#4026](https://github.com/rollup/rollup/pull/4026): chore: fix vscode launch config (change tdd to bdd) (@jameslahm)
- [#4027](https://github.com/rollup/rollup/pull/4027): Post comment for PRs from forks (@lukastaegert)
- [#4028](https://github.com/rollup/rollup/pull/4028): Expose rendered module code to generateBundle hook (@btd)

## 2.43.1

_2021-03-28_

### Bug Fixes

- Prevent infinite recursions in certain scenarios when calling object properties (#4025)

### Pull Requests

- [#4025](https://github.com/rollup/rollup/pull/4025): Handle recursive this mutation detection (@lukastaegert)

## 2.43.0

_2021-03-27_

### Features

- Track side effects of function properties in objects for better tree-shaking (#4011)

### Pull Requests

- [#4011](https://github.com/rollup/rollup/pull/4011): Disable pessimistic object deoptimization for calls when the called function doesn't ref this (@marijnh)
- [#4012](https://github.com/rollup/rollup/pull/4012): fix `sourcemap` reference in docs (@tjenkinson)
- [#4015](https://github.com/rollup/rollup/pull/4015): Use SIGTERM instead of SIGINT to kill test child processes in tests (@marijnh)

## 2.42.4

_2021-03-24_

### Bug Fixes

- Do not discard plugin return values when using perf option (#4010)

### Pull Requests

- [#4010](https://github.com/rollup/rollup/pull/4010): Return hook result inside promise with async timer end ( @SuperOleg39)

## 2.42.3

_2021-03-22_

### Bug Fixes

- Do not ignore `#__PURE__` comments in front of optional chaining expressions (#4007)

### Pull Requests

- [#4007](https://github.com/rollup/rollup/pull/4007): Tree-shake pure call expressions with optional chaining ( @lukastaegert)

## 2.42.2

_2021-03-22_

### Bug Fixes

- Use correct import.meta.url in relative imports from transpiled config files (#4005)

### Pull Requests

- [#4005](https://github.com/rollup/rollup/pull/4005): Use correct import.meta.url in config files (@lukastaegert)

## 2.42.1

_2021-03-20_

### Bug Fixes

- Do not produce unhandled Promise rejections when plugins throw while using the `perf` option (#4004)

### Pull Requests

- [#4004](https://github.com/rollup/rollup/pull/4004): Fixed unhandled promise rejections (@gluck)

## 2.42.0

_2021-03-19_

### Features

- Prevent infinite loops when several plugins are using `this.resolve` in their resolveId hook (#4000)

### Pull Requests

- [#4000](https://github.com/rollup/rollup/pull/4000): Break infinite loops in this.resolve (@lukastaegert)

## 2.41.5

_2021-03-18_

### Bug Fixes

- Make sure unused property accesses of external namespaces can be tree-shaken (#4001)

### Pull Requests

- [#4001](https://github.com/rollup/rollup/pull/4001): Do not count accessing members of an external namespace as side-effects (@lukastaegert)

## 2.41.4

_2021-03-16_

### Bug Fixes

- Do not replace external namespace imports with individual named imports to avoid changing behaviour with regard to missing exports (#3999)

### Pull Requests

- [#3999](https://github.com/rollup/rollup/pull/3999): Allow to safely probe external namespaces (@lukastaegert)

## 2.41.3

_2021-03-16_

### Bug Fixes

- Always retain arguments passed to empty object pattern parameters (#3998)

### Pull Requests

- [#3998](https://github.com/rollup/rollup/pull/3998): Do not create invalid code if a function argument is an empty object pattern (@lukastaegert)

## 2.41.3

_2021-03-16_

### Bug Fixes

- Always retain arguments passed to empty object pattern parameters (#3998)

### Pull Requests

- [#3998](https://github.com/rollup/rollup/pull/3998): Do not create invalid code if a function argument is an empty object pattern (@lukastaegert)

## 2.41.2

_2021-03-12_

### Bug Fixes

- Also remove sourcemaps comments if plugins return a pre-made ast (#3987)

### Pull Requests

- [#3987](https://github.com/rollup/rollup/pull/3987): Change removal of sourcemap comment (@yannayl)

## 2.41.1

_2021-03-11_

### Pull Requests

- [#3990](https://github.com/rollup/rollup/pull/3990): Add browser sourcemap and remove log (@lukastaegert)

## 2.41.0

_2021-03-09_

### Features

- Add option to `treeshake.propertyReadSideEffects` to keep all property accesses (#3985)

### Bug Fixes

- Also respect pure comment annotations when a plugin provides an AST in the transform hook provided they use this.parse (#3981)

### Pull Requests

- [#3981](https://github.com/rollup/rollup/pull/3981): Move pure comment annotation to Graph.contextParse (@yannayl)
- [#3985](https://github.com/rollup/rollup/pull/3985): implement --treeshake.propertyReadSideEffects=always to handle getters with side effects (@kzc)

## 2.40.0

_2021-02-26_

### Features

- Make sure that entry point variable names take precedence over variable names in dependencies when deconflicting ( #3977)

### Bug Fixes

- Replace `:` in generated file names to prevent invalid files on Windows (#3972)

### Pull Requests

- [#3972](https://github.com/rollup/rollup/pull/3972): Don't allow `:` in file names (@lukastaegert)
- [#3976](https://github.com/rollup/rollup/pull/3976): Add soft breaks to guide to improve mobile experience ( @lukastaegert)
- [#3977](https://github.com/rollup/rollup/pull/3977): Reverse module deconflicting order (@lukastaegert)

## 2.39.1

_2021-02-23_

### Bug Fixes

- Make sure local variables named Symbol, Object or Promise do not conflict with code generated by Rollup (#3971)

### Pull Requests

- [#3964](https://github.com/rollup/rollup/pull/3964): Remove extra word (@jamonholmgren)
- [#3971](https://github.com/rollup/rollup/pull/3971): Avoid conflicts with local variables named Symbol, Object, Promise (@lukastaegert)

## 2.39.0

_2021-02-12_

### Features

- Add "validate" option to verify generated chunks are valid JavaScript (#3952)

### Bug Fixes

- Always add exports properties for uninitialized named exports (#3957)
- Allow using an external namespace reexport together with named exports (#3959)
- Avoid invalid generated code in certain scenarios with SystemJS exports (#3960)

### Pull Requests

- [#3952](https://github.com/rollup/rollup/pull/3952): implement `validate` output option and `--validate` CLI option ( @kzc)
- [#3956](https://github.com/rollup/rollup/pull/3956): Update dependencies, fix fsevents issue (@lukastaegert)
- [#3957](https://github.com/rollup/rollup/pull/3957): Make sure uninitialised exports turn up via .hasOwnProperty for non-ES formats (@lukastaegert)
- [#3959](https://github.com/rollup/rollup/pull/3959): Allow overriding individual exports of reexported external namespaces (@lukastaegert)
- [#3960](https://github.com/rollup/rollup/pull/3960): Make sure system exports are valid JavaScript (@lukastaegert)

## 2.38.5

_2021-02-05_

### Bug Fixes

- Prevent invalid code when simplifying assignments and delcarations (#3951)
- Prevent behaviour-changing line-breaks when simplifying assignments in return statements (#3951)
- Slightly improve white-space rendering when simplifying certain expressions (#3951)

### Pull Requests

- [#3951](https://github.com/rollup/rollup/pull/3951): Wrap simplified assignments if necessary (@lukastaegert)

## 2.38.4

_2021-02-02_

### Bug Fixes

- Do not change logic when tree-shaking declarations in if statements or loops (#3947)

### Pull Requests

- [#3947](https://github.com/rollup/rollup/pull/3947): Do not tear apart declarations in loop or if bodies ( @lukastaegert)

## 2.38.3

_2021-02-01_

### Bug Fixes

- Prevent an unexpected live-binding when default exporting a synthetic named export (#3946)

### Pull Requests

- [#3945](https://github.com/rollup/rollup/pull/3945): Upgrade chokidar and fsevents for Apple M1 compatibility ( @threepointone)
- [#3946](https://github.com/rollup/rollup/pull/3946): Make sure default exports snapshot synthetic named exports ( @lukastaegert)

## 2.38.2

_2021-01-31_

### Bug Fixes

- Do not generate invalid code for partially tree-shaken declarations in for loops (#3943)
- Always include function bodies of functions in side-effect-free modules (#3944)

### Pull Requests

- [#3943](https://github.com/rollup/rollup/pull/3943): Do not partially tree-shake unused declarations in for loops ( @lukastaegert)
- [#3944](https://github.com/rollup/rollup/pull/3944): Correctly include functions with side effects from side-effect-free modules (@lukastaegert)

## 2.38.1

_2021-01-28_

### Bug Fixes

- Fix internal error when resolving a missing entry point in the browser build (#3935)

### Pull Requests

- [#3935](https://github.com/rollup/rollup/pull/3935): fix: remove isolated resolve() for compat with browser distribution (@cmorten and @lukastaegert)
- [#3936](https://github.com/rollup/rollup/pull/3936): Ensure test after() callback is always executed ( @Benjamin-Dobell)
- [#3937](https://github.com/rollup/rollup/pull/3937): Modernize references to other software (@ludofischer)

## 2.38.0

_2021-01-22_

### Features

- Entirely remove declared variables that only have an initializer side effect (#3933)

### Pull Requests

- [#3933](https://github.com/rollup/rollup/pull/3933): Tree-shake unused declarations while keeping initializer side-effects (@lukastaegert)

## 2.37.1

_2021-01-20_

### Pull Requests

- [#3929](https://github.com/rollup/rollup/pull/3929): Deduplicate acorn import (@lukastaegert)

## 2.37.0

_2021-01-19_

### Features

- Always check modules for side effects that only indirectly reexport a used variable (#3840)
- Warn if a circular dependency would cause wrong execution order when preserving modules (#3840)

### Bug Fixes

- Allow consuming synthetic exports via modules that reexport a namespace (#3894)
- Do not crash for circular default reexports (#3840)
- Do not crash for circular synthetic namespaces (#3840)
- Improve circular dependency execution order in certain scenarios (#3840)

### Pull Requests

- [#3840](https://github.com/rollup/rollup/pull/3840): Improve circular dependency execution order (@lukastaegert)
- [#3894](https://github.com/rollup/rollup/pull/3894): Always respect synthetic namespaces in namespace reexport ( @lukastaegert)

## 2.36.2

_2021-01-16_

### Bug Fixes

- Fix an issue where invalid code was generated for unused assignments with side effects (#3926)

### Pull Requests

- [#3926](https://github.com/rollup/rollup/pull/3926): Correctly simplify assignments with parentheses (@lukastaegert)

## 2.36.1

_2021-01-06_

### Bug Fixes

- Solve issues that result in invalid code when partially removing assignments (#3921)

### Pull Requests

- [#3921](https://github.com/rollup/rollup/pull/3921): Prevent invalid code when removing assignment target of side-effectful object expression (@lukastaegert)

## 2.36.0

_2021-01-05_

### Features

- Support partial tree-shaking of chained assignments and unused assignment targets (#3919)

### Pull Requests

- [#3919](https://github.com/rollup/rollup/pull/3919): Treeshake chained assignment expressions (@lukastaegert)

## 2.35.1

_2020-12-14_

### Bug Fixes

- Allow closing the bundle when watching in case of generate errors by adding the bundle to the error event (#3909)
- Automatically close all bundles on generate errors when watching and using the CLI (#3909)
- Try to create remaining bundles when watching and one of them throws (#3909)

### Pull Requests

- [#3909](https://github.com/rollup/rollup/pull/3909): Forward bundle through watch error events (@lukastaegert)

## 2.35.0

_2020-12-14_

### Features

- Add `closeBundle` hook that is triggered by `bundle.close()` in the JS API (#3883)

### Pull Requests

- [#3883](https://github.com/rollup/rollup/pull/3883): Revert pattern to folder export (@intrnl)

## 2.34.2

_2020-12-06_

### Bug Fixes

- Revert pattern export change (#3898)

### Pull Requests

- [#3898](https://github.com/rollup/rollup/pull/3898): Revert pattern to folder export (@lukastaegert)

## 2.34.1

_2020-12-03_

### Bug Fixes

- Avoid Node deprecation warning by using a pattern export for nested Rollup files (#3896)

### Pull Requests

- [#3887](https://github.com/rollup/rollup/pull/3887): Run memory leak test on all systems (@lukastaegert)
- [#3892](https://github.com/rollup/rollup/pull/3892): Add pull_request to windows github actions (@shellscape)
- [#3893](https://github.com/rollup/rollup/pull/3893): Update dependencies (@lukastaegert)
- [#3896](https://github.com/rollup/rollup/pull/3896): Replace deprecated folder package export with pattern export ( @lukastaegert)

## 2.34.0

_2020-11-29_

### Features

- Support RequireJS comaptible AMD ids in code-splitting builds via amd.autoId (#3867)
- Allow adding an AMD id base path (#3867)

### Bug Fixes

- Warn when using an constant AMD id in a code-splitting build (#3867)

### Pull Requests

- [#3867](https://github.com/rollup/rollup/pull/3867): Implement amd.autoId/amd.basePath options (@tjenkinson)

## 2.33.3

_2020-11-18_

### Bug Fixes

- Do not use `.js` extension when importing AMD files from a UMD bundle (#3872)

### Pull Requests

- [#3861](https://github.com/rollup/rollup/pull/3861): Update chat/support links (@shellscape)
- [#3872](https://github.com/rollup/rollup/pull/3872): Also removeExtensionFromRelativeAmdId in UMD finaliser ( @tjenkinson)

## 2.33.2

_2020-11-14_

### Bug Fixes

- Fix an issue where statements were ignored after a conditional return in a labeled statement (#3871)

### Pull Requests

- [#3871](https://github.com/rollup/rollup/pull/3871): Correctly track label usage in try statements (@Amareis)

## 2.33.1

_2020-11-02_

### Bug Fixes

- Add `syntheticNamedExports` to `this.getModuleInfo` to align with documentation (#3847)

### Pull Requests

- [#3847](https://github.com/rollup/rollup/pull/3847): Expose syntheticNamedExports to ModuleInfo (@Amareis)
- [#3852](https://github.com/rollup/rollup/pull/3852): Fix typo on docs (@jpsc)

## 2.33.0

_2020-11-01_

### Features

- Add parameter to "watchChange" hook to denote if a change was an addition, update or deletion (#3841)
- Add "closeWatcher" hook to allow plugins to clean up resources when the watcher is closed (#3841)
- Add "this.getWatchFiles" function to plugin context to get the current set of watched files (#3841)

### Pull Requests

- [#3841](https://github.com/rollup/rollup/pull/3841): Improved watcher hooks (@Amareis)
- [#3848](https://github.com/rollup/rollup/pull/3848): Add options hook to asyncpluginhooks (@intrnl)

## 2.32.1

_2020-10-21_

### Bug Fixes

- Print warning location for plugin warnings if only `loc` is supplied (#3824)

### Pull Requests

- [#3824](https://github.com/rollup/rollup/pull/3824): plugin warnings not showing warning.loc (@luciotato)

## 2.32.0

_2020-10-16_

### Features

- Extend `preserveEntrySignatures` with a value `"exports-only"` to allow extension only if an entry does not have exports (#3823)

### Pull Requests

- [#3823](https://github.com/rollup/rollup/pull/3823): Add "exports-only" option to preserveSignature (@lukastaegert)

## 2.31.0

_2020-10-15_

### Features

- When using the `output.moduleToStringTag` option, also add the tag to entries with exports and simulated external namespaces (#3822)
- Add the `__esModule` interop marker to IIFE global variables unless `output.esModule` is turned off (#3822)

### Pull Requests

- [#3822](https://github.com/rollup/rollup/pull/3822): Add module toStringTag to entries and interop namespaces ( @lukastaegert)

## 2.30.0

_2020-10-13_

### Features

- Add `moduleParsed` hook that is called for each module once code and AST are available (#3813)
- Include code and AST in `this.getModuleInfo` (#3813)

### Bug Fixes

- Provide the original Acorn AST instead of the internal one when resolving dynamic imports that contain non-trivial expressions (#3813)

### Pull Requests

- [#3813](https://github.com/rollup/rollup/pull/3813): Add moduleParsed plugin hook (@lukastaegert)
- [#3815](https://github.com/rollup/rollup/pull/3815): Docs: wile => while (@tjenkinson)
- [#3817](https://github.com/rollup/rollup/pull/3817): Docs: fix code snippet (@codefrau)
- [#3818](https://github.com/rollup/rollup/pull/3818): Update documentation on configuring Babel, removing the section on passing '{"modules": false}' as that is no longer needed since Babel 7 (@Robin-Hoodie)

## 2.29.0

_2020-10-08_

### Features

- Allow passing custom options to other plugins via `this.resolve` (#3807)
- Allow attaching custom meta information to modules when resolving, loading or transforming (#3807)
- Do not throw but return `null` when using `this.getModuleInfo` for an unknown id (#3807)

### Bug Fixes

- Trigger build in watch mode when files are added to a watched directory (#3812)
- Make `code` optional when transforming modules (#3807)

### Pull Requests

- [#3807](https://github.com/rollup/rollup/pull/3807): Implement new APIs for inter-plugin communication (@lukastaegert)
- [#3808](https://github.com/rollup/rollup/pull/3808): Document that the default value of --format is 'es' ( @jameshfisher)
- [#3812](https://github.com/rollup/rollup/pull/3812): Watch: listen for new files added to a directory (@dmitrage)

## 2.28.2

_2020-09-24_

### Bug Fixes

- Fix a source of possible variable name conflicts when using preserveModules with SystemJS (#3796)

### Pull Requests

- [#3792](https://github.com/rollup/rollup/pull/3792): add documentation for output.PreserveModulesRoot (@davidroeca)
- [#3796](https://github.com/rollup/rollup/pull/3796): Fix SystemJS default variable conflict (@lukastaegert)

## 2.28.1

_2020-09-21_

### Bug Fixes

- Fix a path slash issue when using the preserveModulesRoot option on Windows (#3791)

### Pull Requests

- [#3791](https://github.com/rollup/rollup/pull/3791): Fix preserveModulesRoot path on Windows (@lukastaegert)

## 2.28.0

_2020-09-21_

### Features

- Add an option to treat modules at a given path as located at root when preserving modules (#3786)

### Pull Requests

- [#3786](https://github.com/rollup/rollup/pull/3786): Add preserveModulesRoot config option (@davidroeca)

## 2.27.1

_2020-09-17_

### Bug Fixes

- Do not fail when using ES module imports in symlinked config files (#3783)

### Pull Requests

- [#3783](https://github.com/rollup/rollup/pull/3783): Handle loading symlinked config files (@lukastaegert)

## 2.27.0

_2020-09-16_

### Features

- Support specifying a file extension when reading from stdin (#3775)

### Bug Fixes

- Do not break logic if a branch with hoisted variables is tree-shaken in an else-if statement (#3782)

### Pull Requests

- [#3770](https://github.com/rollup/rollup/pull/3770): Docs: Exception for babel plugin and commonjs plugin (@jsk7)
- [#3775](https://github.com/rollup/rollup/pull/3775): add ability to specify stdin file extension via --stdin=ext ( @kzc)
- [#3782](https://github.com/rollup/rollup/pull/3782): Handle hoisted variables in dead branches of nested if statements (@lukastaegert)

## 2.26.11

_2020-09-08_

### Bug Fixes

- Do not fail for unknown nodes as if statement branches (#3769)

### Pull Requests

- [#3769](https://github.com/rollup/rollup/pull/3769): Handle debugger statements as if-statement branches ( @lukastaegert)

## 2.26.10

_2020-09-04_

### Bug Fixes

- Do not create invalid code when simplifying expressions in return statements that contain line comments (#3762)

### Pull Requests

- [#3757](https://github.com/rollup/rollup/pull/3757): Fix api docs loadconfigfile (@maxwell8888)
- [#3762](https://github.com/rollup/rollup/pull/3762): Handle line-comments when removing line-breaks to prevent ASI ( @lukastaegert)

## 2.26.9

_2020-09-01_

### Bug Fixes

- Add regular expression support to watch include/exclude types (#3754)

### Pull Requests

- [#3754](https://github.com/rollup/rollup/pull/3754): Add RegExp to the include and exclude fields of the WatcherOptions type (@dagda1)
- [#3756](https://github.com/rollup/rollup/pull/3756): Update FAQ: I think it was meant "external" instead of " other-entry.js" (@madacol)

## 2.26.8

_2020-08-29_

### Bug Fixes

- Make sure that both unresolved and resolved ids are passed to the `external` option in all cases (#3753)

### Pull Requests

- [#3753](https://github.com/rollup/rollup/pull/3753): Also pass resolved ids to external if they use the object for ( @lukastaegert)

## 2.26.7

_2020-08-28_

### Bug Fixes

- Avoid invalid code when rendering hoisted variable declarations from dead branches (#3752)
- Mark the `options` parameter of `this.parse` as optional for TypeScript plugins (#3750)

### Pull Requests

- [#3750](https://github.com/rollup/rollup/pull/3750): Make `options` of `PluginContext#parse` optional (@intrnl)
- [#3752](https://github.com/rollup/rollup/pull/3752): Extract hoisted variables from dead branches (@lukastaegert)

## 2.26.6

_2020-08-27_

### Bug Fixes

- Avoid conflicts between the namespace of synthetic named exports and local variables (#3747)

### Pull Requests

- [#3747](https://github.com/rollup/rollup/pull/3747): Properly deconflict synthetic named exports (@lukastaegert)

## 2.26.5

_2020-08-22_

### Bug Fixes

- Use correctly deconflicted variable names for reexported namespaces in ES formats (#3742)

### Pull Requests

- [#3742](https://github.com/rollup/rollup/pull/3742): Avoid variable name conflict when reexporting several namespaces from a chunk (@lukastaegert)

## 2.26.4

_2020-08-19_

### Bug Fixes

- Fix a situation where invalid code was rendered when dynamically importing a module with synthetic named exports when preserving modules (#3738)
- Create a proper namespace object when in a non-es format, a namespace is imported from a chunk with `default` export mode (#3738)
- Use the same variable when in a chunk, a namespace is both imported and reexported as a binding (#3738)
- Do not include the synthetic namespace in static entry points unless it is actually used (#3738)
- Make sure the chunking of one output does not interfere with the namespace objects of another output (#3738)

### Pull Requests

- [#3738](https://github.com/rollup/rollup/pull/3738): Improve synthetic entry handling (@lukastaegert)

## 2.26.3

_2020-08-16_

### Bug Fixes

- Fix a situation where line-breaks in a nested simplified conditional expression could result in broken code (#3734)

### Pull Requests

- [#3734](https://github.com/rollup/rollup/pull/3734): Prevent ASI when simplifying a nested logical expression ( @lukastaegert)

## 2.26.2

_2020-08-16_

### Bug Fixes

- Fix a situation where line-breaks in a simplified conditional expression could result in broken code (#3732)

### Pull Requests

- [#3732](https://github.com/rollup/rollup/pull/3732): Prevent unintended ASI for nested conditionals (@lukastaegert)

## 2.26.1

_2020-08-16_

### Bug Fixes

- Correctly render external namespace imports when only generating SystemJS output (#3731)

### Pull Requests

- [#3731](https://github.com/rollup/rollup/pull/3731): Render system namespace import (@sastan and @lukastaegert)

## 2.26.0

_2020-08-15_

### Features

- Add a new entry `importedBindings` to the bundle information to list bindings per dependency (#3722)

### Bug Fixes

- Do not render an invalid UMD wrapper when no bindings are imported from a dependency (#3724)
- Avoid situations where removing the `else` branch from an `if` statement might catch the `else` branch from another one (#3725)

### Pull Requests

- [#3722](https://github.com/rollup/rollup/pull/3722): Add import specifiers to bundle information (@lukastaegert)
- [#3724](https://github.com/rollup/rollup/pull/3724): Fix missing variables for UMD and IIFE builds (@lukastaegert)
- [#3725](https://github.com/rollup/rollup/pull/3725): Do not entirely remove else branch if another else branch might accidentally be referenced (@lukastaegert)

## 2.25.0

_2020-08-14_

### Features

- Add `--failAfterWarnings` CLI flag that will complete builds with warnings but return an error at the end (#3712)

### Pull Requests

- [#3712](https://github.com/rollup/rollup/pull/3712): Implement `--failAfterWarnings` flag (@tjenkinson)

## 2.24.0

_2020-08-13_

### Features

- Allow defining interop per dependency via a function (#3710)
- Support interop "auto" as a more compatible version of "true" (#3710)
- Support interop "default" and "esModule" to avoid unnecessary interop helpers (#3710)
- Support interop "defaultOnly" for simplified helpers and Node ESM interop compatible output (#3710)
- Respect interop option for external dynamic imports (#3710)
- Support live-bindings for external default imports in non-ES formats unless "externalLiveBindings" is "false" (#3710)
- Use shared default interop helpers for AMD, UMD and IIFE formats (#3710)
- Avoid unnecessarily deconflicted module variables in non-ES formats (#3710)
- Freeze generated interop namespace objects (#3710)
- Always mark interop helpers as pure (#3710)
- Avoid default export interop if there is already an interop namespace object (#3710)
- Sort all `require` statements to the top in CommonJS output for easier back-transpilation to ES modules by other tools (#3710)

### Bug Fixes

- Handle accessing `super` in static class fields (#3720)
- Deconflict the names of helper variables introduced for interop (#3710)
- Generate proper namespace objects for static namespace imports in non-ES formats (#3710)
- Do not add unused interop helpers when using the renderDynamicImport hook (#3710)

### Pull Requests

- [#3710](https://github.com/rollup/rollup/pull/3710): Rework interop handling (@lukastaegert)
- [#3720](https://github.com/rollup/rollup/pull/3720): Handle super in static class fields (@lukastaegert)

## 2.23.1

_2020-08-07_

### Bug Fixes

- Fix an issue where dynamically importing an entry point could return a malformed namespace for CJS and AMD formats ( #3709)

### Pull Requests

- [#3709](https://github.com/rollup/rollup/pull/3709): Properly construct namespace when dynamically importing chunks with facades in default export mode (@lukastaegert)

## 2.23.0

_2020-07-23_

### Features

- Handle environments with only globalThis in UMD output (#3691)

### Pull Requests

- [#3691](https://github.com/rollup/rollup/pull/3691): Check for globalThis in UMD wrapper (@lukastaegert)

## 2.22.2

_2020-07-21_

### Bug Fixes

- Always generate correct exports when an implicit entry is reexporting from another module (#3688)

### Pull Requests

- [#3688](https://github.com/rollup/rollup/pull/3688): Include all relevant modules to generate reexports for implicit dependencies (@lukastaegert)

## 2.22.1

_2020-07-18_

### Bug Fixes

- Remove unused arguments when calling a conditional expression (#3680)

### Pull Requests

- [#3680](https://github.com/rollup/rollup/pull/3680): Allow tree-shaking of arguments of functions that are returned by conditional expressions (@lukastaegert)

## 2.22.0

_2020-07-18_

### Features

- Allow resolving synthetic named exports via an arbitrary export name (#3657)
- Display a warning when the user does not explicitly select an export mode and would generate a chunk with default export mode when targeting CommonJS (#3657)

### Pull Requests

- [#3657](https://github.com/rollup/rollup/pull/3657): Add basic support for using a non-default export for syntheticNamedExports (@lukastaegert)
- [#3659](https://github.com/rollup/rollup/pull/3659): Warn when implicitly using default export mode (@lukastaegert)

## 2.21.0

_2020-07-07_

### Features

- Allow plugins to disable tree-shaking for individual modules to ensure even empty modules are associated with chunks ( #3663)

### Pull Requests

- [#3663](https://github.com/rollup/rollup/pull/3663): Disable treeshaking per module (@lukastaegert)

## 2.20.0

_2020-07-06_

### Features

- Support using a function to generate different chunk and asset naming patterns per chunk or asset (#3658)
- Add `referencedFiles` property to the chunk info in generateBundle to list referenced assets (#3661)

### Pull Requests

- [#3658](https://github.com/rollup/rollup/pull/3658): Add ability to use a function that returns a pattern string in all places where you could use a pattern string before (@frank-dspeed)
- [#3661](https://github.com/rollup/rollup/pull/3661): Add referenced files to bundle (@lukastaegert)

## 2.19.0

_2020-07-05_

### Features

- Allow plugins to return a Promise in the options hook (#3660)

### Pull Requests

- [#3660](https://github.com/rollup/rollup/pull/3660): Make options hooks async (@TomerAberbach)

## 2.18.2

_2020-07-02_

### Bug Fixes

- Do not remove spread element args when the corresponding positional parameter is unused (#3652)

### Pull Requests

- [#3652](https://github.com/rollup/rollup/pull/3652): Do not tree-shake arguments that contain a spread element ( @lukastaegert)

## 2.18.1

_2020-06-26_

### Bug Fixes

- Make sure synthetic exports are present when a module is imported dynamically (#3648)
- Strip the `rollup-plugin-` prefix off the plugin name when looking for the plugin export in a CLI plugin without a default export (#3647)
- Convert plugin names with dashes to camel case when looking for the plugin export in a CLI plugin without a default export (#3647)

### Pull Requests

- [#3647](https://github.com/rollup/rollup/pull/3647): Strip rollup-plugin prefix to find named plugin exports, throw when export cannot be found (@lukastaegert)
- [#3648](https://github.com/rollup/rollup/pull/3648): Always create a dynamic namespace object when a module with synthetic named exports is imported dynamically (@lukastaegert)

## 2.18.0

_2020-06-22_

### Features

- `inlineDynamicImports`, `manualChunks` and `preserveModules` can now be used as output options (#3645)
- Use sourcemaps for certain warnings that reference source code locations (#3645)

### Bug Fixes

- `this.getFileName` will now always return the correct file name for chunks when multiple outputs are created (#3645)

### Pull Requests

- [#3645](https://github.com/rollup/rollup/pull/3645): Per output chunking (@lukastaegert)

## 2.17.1

_2020-06-19_

### Bug Fixes

- Properly resolve accessing properties of namespace members again (#3643)

### Pull Requests

- [#3643](https://github.com/rollup/rollup/pull/3643): Fix accessing nested properties of namespaces (@lukastaegert)

## 2.17.0

_2020-06-17_

### Features

- When importing Rollup via package.exports, always fall back to the browser ESM build for non-Node environments (#3634)
- Create more efficient code when handling namespace mutations (#3637)

### Bug Fixes

- Fix a severe performance regression when the same module is imported by a lot of modules (#3641)
- Properly escape special characters in imports (#3638)

### Pull Requests

- [#3634](https://github.com/rollup/rollup/pull/3634): Set browser build in exports (@guybedford)
- [#3637](https://github.com/rollup/rollup/pull/3637): Do not include the whole namespace when illegally mutating a namespace (@lukastaegert)
- [#3638](https://github.com/rollup/rollup/pull/3638): Support backslash escaping, retain exact newline escaping ( @guybedford)
- [#3641](https://github.com/rollup/rollup/pull/3641): Fix performance regression when a file is imported by many importers (@lukastaegert)

## 2.16.1

_2020-06-13_

### Bug Fixes

- Do not produce invalid code when an external or chunk id contain quotes or line-breaks (#3632)
- Do not fail but emit a warning when mutating a namespace object (#3633)

### Pull Requests

- [#3632](https://github.com/rollup/rollup/pull/3632): Handle single quote escaping in ids (@guybedford)
- [#3633](https://github.com/rollup/rollup/pull/3633): Turn namespace assignment error into a warning (@guybedford)

## 2.16.0

_2020-06-12_

### Features

- Add support for numeric separators (#3626)
- Switch to finalized ESTree optional chaining AST (#3628)

### Pull Requests

- [#3626](https://github.com/rollup/rollup/pull/3626): Support numeric separator (@TrySound)
- [#3628](https://github.com/rollup/rollup/pull/3628): Acorn 7.3.0 upgrade (@guybedford)
- [#3631](https://github.com/rollup/rollup/pull/3631): Improve discoverability of `manualChunks` for code splitting ( @zlamma)

## 2.15.0

_2020-06-08_

### Features

- Allow to skip watching some configs via `watch: false` (#3620)
- Provide the resolved sourcemap path to `sourcemapPathTransform` (#3617)

### Pull Requests

- [#3617](https://github.com/rollup/rollup/pull/3617): Update sourcemapPathTransform to also take the path to the sourcemap file as a second argument (@dgoldstein0)
- [#3620](https://github.com/rollup/rollup/pull/3620): Rollup watch only one config in exported array (@luwol03)

## 2.14.0

_2020-06-07_

### Features

- Make `this.meta.watchMode` available for plugins to detect watch mode (#3616)

### Bug Fixes

- Handle exporting the same binding with different names in SystemJS (#3575)

### Pull Requests

- [#3575](https://github.com/rollup/rollup/pull/3575): Handle some cases of duplicate export bindings (@joeljeske)
- [#3616](https://github.com/rollup/rollup/pull/3616): Make watch mode available in plugins (@lukastaegert)

## 2.13.1

_2020-06-04_

### Bug Fixes

- Prevent conflicts in SystemJS when `module` is used as a top-level variable (#3614)

### Pull Requests

- [#3614](https://github.com/rollup/rollup/pull/3614): Handle system reserved identifier dedupes (@guybedford)

## 2.13.0

_2020-06-03_

### Features

- Allow to specify that an emitted chunk is only loaded after a given module has loaded to improve chunking (#3606)

### Pull Requests

- [#3606](https://github.com/rollup/rollup/pull/3606): Enable specifying implicit dependencies when emitting chunks ( @lukastaegert)

## 2.12.1

_2020-06-02_

### Bug Fixes

- Render valid imports when chunk names correspond to directory names in virtual setups (#3609)

### Pull Requests

- [#3609](https://github.com/rollup/rollup/pull/3609): Handle imports from chunks with names that correspond to parent directory names of other chunks (@guybedford)

## 2.12.0

_2020-05-31_

### Features

- Add an option `--waitForBundleInput` to let the build wait until all entry point files are available before starting ( #3577)

### Pull Requests

- [#3577](https://github.com/rollup/rollup/pull/3577): Wait for bundle input option (@Heerschop)

## 2.11.2

_2020-05-28_

### Bug Fixes

- Include side-effects in the second argument of `Array.from` (#3604)

### Pull Requests

- [#3604](https://github.com/rollup/rollup/pull/3604): Mark `Array.from` as side-effectful, use two-argument Array.from when mapping Sets (@lukastaegert)

## 2.11.1

_2020-05-28_

### Bug Fixes

- Also include side-effects in files that are marked as side-effect-free if they contain an included default export that is reexported (#3602)

### Pull Requests

- [#3602](https://github.com/rollup/rollup/pull/3602): Handle side-effects next to side-effect-free default exports in case the default export is reexported (@lukastaegert)

## 2.11.0

_2020-05-27_

### Features

- Add basic support for optional chaining (#3582)
- Provide a normalized set of options with proper default values to `buildStart` and `renderStart` (#3597)
- Do not count adding properties to the prototype of an unused class as a side-effect (#3598)
- Support providing `null` for empty setters in SystemJS via option (#3592)

### Bug Fixes

- Do not fail when using a `/*#__PURE__*/` annotation inside a class field (#3599)
- Allow using `--watch` and `--treeshake` together with sub-options such as `--watch.clearScreen` on the command line ( #3597)

### Pull Requests

- [#3582](https://github.com/rollup/rollup/pull/3582): Support optional chaining via acorn fork(@guybedford)
- [#3592](https://github.com/rollup/rollup/pull/3592): System format optional setters(@guybedford)
- [#3597](https://github.com/rollup/rollup/pull/3597): Provide normalized options (@lukastaegert)
- [#3598](https://github.com/rollup/rollup/pull/3598): Treeshake prototype modifications in classes (@lukastaegert)
- [#3599](https://github.com/rollup/rollup/pull/3599): Retain pure annotations in class fields (@lukastaegert)
- [#3601](https://github.com/rollup/rollup/pull/3601): Fix white-space in docs (@tu4mo)

## 2.10.9

_2020-05-24_

### Bug Fixes

- Prevent invalid exports when facades are created (#3590)

### Pull Requests

- [#3590](https://github.com/rollup/rollup/pull/3590): Prevent unneeded exports when entry facades are created and ensure all exported variables in facades are imported (@lukastaegert)

## 2.10.8

_2020-05-23_

### Bug Fixes

- Fix issues when synthetic named exports are reexported as default exports (#3586)

### Pull Requests

- [#3584](https://github.com/rollup/rollup/pull/3584): Clarify documentation for `output.paths` (@jacksteamdev)
- [#3585](https://github.com/rollup/rollup/pull/3585): Target Node.js v14 instead of v13 in Windows tests (@mangs)
- [#3586](https://github.com/rollup/rollup/pull/3586): Handle default reexports of synthetic named exports over several stages (@lukastaegert)

## 2.10.7

_2020-05-22_

### Bug Fixes

- Handle modules re-exporting namespaces without further own code (#3576)

### Pull Requests

- [#3576](https://github.com/rollup/rollup/pull/3576): Fix "cannot read exports of undefined" error (@guybedford)

## 2.10.6

_2020-05-22_

### Bug Fixes

- Fix some issues around class fields (#3580)
- Prevent a maximum call stack error when a called entity references itself in its declaration (#3581)

### Pull Requests

- [#3580](https://github.com/rollup/rollup/pull/3580): Update acorn class features (@guybedford)
- [#3581](https://github.com/rollup/rollup/pull/3581): Do not fail when including call arguments of recursively defined variables (@lukastaegert)

## 2.10.5

_2020-05-19_

### Bug Fixes

- Do not remove side-effects that may influence an included default export declaration when side-effects are disabled ( #3572)

### Pull Requests

- [#3572](https://github.com/rollup/rollup/pull/3572): Observe side-effects in files containing a default export declaration that reexports a variable (@lukastaegert)

## 2.10.4

_2020-05-19_

### Bug Fixes

- Tree-shake unused classes with fields unless there are side-effects in the field declaration (#3569)

### Pull Requests

- [#3569](https://github.com/rollup/rollup/pull/3569): Make sure unused classes with fields are tree-shaken if possible (@lukastaegert)

## 2.10.3

_2020-05-18_

### Bug Fixes

- Validate return value of sourcemapPathTransform option (#3561)

### Pull Requests

- [#3561](https://github.com/rollup/rollup/pull/3561): Throw error if sourcemapPathTransform-option does not return a string (@Simonwep)

## 2.10.2

_2020-05-15_

### Bug Fixes

- Properly include calls to mutating array methods in certain scenarios (#3559)

### Pull Requests

- [#3559](https://github.com/rollup/rollup/pull/3559): Make sure UnknownFooExpressions are included when referenced as return values in a MultiExpression (@lukastaegert)

## 2.10.1

_2020-05-15_

### Bug Fixes

- Do not throw when "undefined" is used as a default export (#3558)

### Pull Requests

- [#3558](https://github.com/rollup/rollup/pull/3558): Properly handle default exporting undefined (@lukastaegert)

## 2.10.0

_2020-05-13_

### Features

- Avoid unnecessary empty imports from a facade chunk to the original chunk (#3552)
- Pin facade creation order so that if several user-defined chunks reference the same module, the first always becomes the "actual" chunk while the later ones become facades (#3552)

### Bug Fixes

- Do not omit reexports from secondary chunks when creating facades for entry points without hoisting transitive dependencies (#3552)

### Pull Requests

- [#3552](https://github.com/rollup/rollup/pull/3552): Avoid unnecessary facade dependency inlining (@guybedford)

## 2.9.1

_2020-05-11_

### Bug Fixes

- Do not create unintended live-bindings or invalid reexports when reexporting global variables (#3550)

### Pull Requests

- [#3550](https://github.com/rollup/rollup/pull/3550): Track updates of globals that are exported as default ( @lukastaegert)

## 2.9.0

_2020-05-10_

### Features

- Add ids of static and dynamic imports to `this.getModuleInfo` (#3542)
- Provide `getModuleInfo` and `getModuleIds` to `manualChunks` functions (#3542)
- Add nullish coalescing support (#3548)
- Make the rebuild delay in watch mode configurable and set the default to `0` for snappy rebuilds (#3502)
- Add `this.getModuleIds` to the plugin context as future replacement for `this.moduleIds` (#3542)

### Pull Requests

- [#3502](https://github.com/rollup/rollup/pull/3502): Configurable build delay (@mattdesl)
- [#3542](https://github.com/rollup/rollup/pull/3542): Extend manualChunks API (@lukastaegert)
- [#3548](https://github.com/rollup/rollup/pull/3548): Support nullish coalescing with tree-shaking (@lukastaegert)

## 2.8.2

_2020-05-07_

### Bug Fixes

- Avoid invalid code when simplifying the body of a shorthand arrow function expression (#3540)

### Pull Requests

- [#3540](https://github.com/rollup/rollup/pull/3540): Wrap object expressions in parentheses if they become children of an arrow function expression (@lukastaegert)

## 2.8.1

_2020-05-07_

### Bug Fixes

- Allow using plugins on CLI that are exported as `exports.default` (#3529)
- Do not fail side-effect detection in nested callbacks of builtins (#3539)

### Pull Requests

- [#3529](https://github.com/rollup/rollup/pull/3529): Use default named export with plugins (@NotWoods)
- [#3539](https://github.com/rollup/rollup/pull/3539): Track call side-effects both by entity and CallExpression to avoid untracked side-effects in nested calls (@lukastaegert)

## 2.8.0

_2020-05-06_

### Features

- When a dynamically imported chunk contains more exports than the imported module namespace, do not create a facade chunk but an inline namespace (#3535)

### Bug Fixes

- Do not execute dynamically imported code before synchronous code in the importing module when generating CommonJS ( #3535)

### Pull Requests

- [#3535](https://github.com/rollup/rollup/pull/3535): Avoid dynamic facade chunks (@lukastaegert)

## 2.7.6

_2020-04-30_

### Bug Fixes

- Fix a type issue when a default export references a global variable (#3526)

### Pull Requests

- [#3526](https://github.com/rollup/rollup/pull/3526): Handles default exporting global variables (@lukastaegert)

## 2.7.5

_2020-04-29_

### Bug Fixes

- Prevent infinite loop when default values of function parameters in a default export contain a slash (#3522)

### Pull Requests

- [#3522](https://github.com/rollup/rollup/pull/3522): Avoid infinite loop when finding position for id insertion in default export (@lukastaegert)

## 2.7.4

_2020-04-29_

### Bug Fixes

- Fix an issue where wrong variable names were used when preserving modules (#3521)

### Pull Requests

- [#3521](https://github.com/rollup/rollup/pull/3521): Fix and improve default export alias logic (@lukastaegert)

## 2.7.3

_2020-04-27_

### Bug Fixes

- Do not access `__proto__` when running Rollup (#3518)

### Pull Requests

- [#3518](https://github.com/rollup/rollup/pull/3518): use acorn-class-fields and acorn-static-class-features from npm ( @nitsky)

## 2.7.2

_2020-04-22_

### Bug Fixes

- Prevent an infinite loop when creating separate manual chunks with circular dependencies (#3510)
- Do not fail if "super" is used in the definition of a class field (#3511)
- Throw if a plugin tries to emit a file with an absolute Windows path (#3509)

### Pull Requests

- [#3509](https://github.com/rollup/rollup/pull/3509): Ban emitFile via absolute paths on Windows OS (@SASUKE40)
- [#3510](https://github.com/rollup/rollup/pull/3510): Do not fail for circular imports between manual chunks ( @lukastaegert)
- [#3511](https://github.com/rollup/rollup/pull/3511): Support "super" in class fields (@lukastaegert)

## 2.7.1

_2020-04-21_

### Bug Fixes

- Use correct path for dynamic imports if `output.paths` is used (#3508)

### Pull Requests

- [#3508](https://github.com/rollup/rollup/pull/3508): Respect output.paths in dynamic imports (@lukastaegert)

## 2.7.0

_2020-04-21_

### Features

- Add `preserveEntrySignatures` option to control how exports of entry points are handled (#3498)
- Add `preserveSignature` flag to `this.emitFile` to control exports of emitted chunks (#3498)
- Add `output.minifyInternalExports` option to control if internal exports are minified (#3498)

### Pull Requests

- [#3498](https://github.com/rollup/rollup/pull/3498): Add option to configure if entry signatures are preserved ( @lukastaegert)

## 2.6.1

_2020-04-12_

### Bug Fixes

- Close watch mode when stdin closes in a non-TTY environment (#3493)

### Pull Requests

- [#3493](https://github.com/rollup/rollup/pull/3493): Ensure --watch mode exits correctly when stdin is closed ( @jakesgordon)

## 2.6.0

_2020-04-10_

### Features

- Allow regular expressions to declare external modules (#3482)

### Pull Requests

- [#3482](https://github.com/rollup/rollup/pull/3482): Allow regular expressions in config.external (@johannes-z)

## 2.5.0

This version is identical to 2.4.0

## 2.4.0

_2020-04-09_

### Features

- Add support for most private and public class field features (#3488)

### Bug Fixes

- Do not replace `this` with `undefined` in class field definitions (#3488)

### Pull Requests

- [#3488](https://github.com/rollup/rollup/pull/3488): Rollup class fields support (@guybedford and @lukastaegert)

## 2.3.5

_2020-04-09_

### Bug Fixes

- Never remove labels when tree-shaking is disabled (#3492)

### Pull Requests

- [#3492](https://github.com/rollup/rollup/pull/3492): Always use a new inclusion context when including declarations of variables, always inlcude labels when not treeshaking (@lukastaegert)

## 2.3.4

_2020-04-07_

### Bug Fixes

- Handle re-exporting synthetic exports from entry-points (#3319)
- Fix cross-chunk imports of synthetic exports (#3319)
- Handle namespace objects that contain re-exported synthetic namespaces (#3319)

### Pull Requests

- [#3319](https://github.com/rollup/rollup/pull/3319): Handle re-exports of synthetic named exports (@manucorporat and @lukastaegert)

## 2.3.3

_2020-04-04_

### Bug Fixes

- Add external namespaces to dynamic namespace objects (#3474)

### Pull Requests

- [#3474](https://github.com/rollup/rollup/pull/3474): Support external star exports on namespace objects (@guybedford)

## 2.3.2

_2020-03-31_

### Bug Fixes

- Only warn but do not fail build when a namespace is called as a function (#3475)
- Make sure pre-existing sourcemap comments are also removed when rebuilding using the cache (#3476)

### Pull Requests

- [#3475](https://github.com/rollup/rollup/pull/3475): Call namespace error as a warning (@guybedford)
- [#3476](https://github.com/rollup/rollup/pull/3476): Store locations for removed comments in cache (@lukastaegert)

## 2.3.1

_2020-03-30_

### Bug Fixes

- Do not fail if the config file returns an function returning a Promise (#3472)

### Pull Requests

- [#3472](https://github.com/rollup/rollup/pull/3472): Fix support for async functions as config (@lukastaegert)

## 2.3.0

_2020-03-29_

### Features

- Do not transpile config files with `.mjs` extension in Node 13+ or `.cjs` extension in any Node version and load them appropriately (#3445)
- Extract helper to load a config file the way rollup does it via `rollup/dist/loadConfigFile` (#3445)

### Bug Fixes

- Keep watching the config file if an error occurs during initial load in watch node (#3445)
- Add a helpful error message when using a transpiled config in a repository with "type": "module" (#3445)

### Pull Requests

- [#3445](https://github.com/rollup/rollup/pull/3445): Support native ESM configs in Node 13, support untranspiled configs (@lukastaegert)
- [#3468](https://github.com/rollup/rollup/pull/3468): Don't use esm output format alias in the documentation (@vsn4ik)

## 2.2.0

_2020-03-24_

### Features

- Add `renderDynamicImport` hook to rewrite dynamic import expressions (#3449)
- Add information about dynamically imported modules to `this.getModuleInfo` (#3449)

### Bug Fixes

- Make file emission work with Uin8Array sources when using Rollup in the browser (#3452)
- Fix types to allow watch to accept an array of configs (#3453)
- Do not strip `.js` extensions from AMD imports when the import is a user-supplied replacement for a non-resolvable dynamic import target (#3453)

### Pull Requests

- [#3449](https://github.com/rollup/rollup/pull/3449): Add hook to rewrite dynamic import expressions (@lukastaegert)
- [#3452](https://github.com/rollup/rollup/pull/3452): Avoid the assumption of Buffer in browser envs (@JoviDeCroock)
- [#3453](https://github.com/rollup/rollup/pull/3453): fix types since watch accepts single or array config (@lukeed)
- [#3456](https://github.com/rollup/rollup/pull/3456): fix SystemJS url in tutorial (@guybedford)

## 2.1.0

_2020-03-18_

### Features

- Allow specifying an importer when emitting files to resolve relative ids (#3442)

### Pull Requests

- [#3442](https://github.com/rollup/rollup/pull/3442): Add optional `importer` parameter to `this.emitFile` ( @lukastaegert)

## 2.0.6

_2020-03-13_

### Bug Fixes

- Do not use file names from different outputs when generating sourcemaps using the `dir` option (#3440)

### Pull Requests

- [#3440](https://github.com/rollup/rollup/pull/3440): Use correct file names when writing sourcemaps for multiple outputs (@lukastaegert)

## 2.0.5

_2020-03-12_

### Bug Fixes

- Fix an issue where conditional statements would assume they have the wrong test value (#3438)

### Pull Requests

- [#3438](https://github.com/rollup/rollup/pull/3438): Make sure logical expressions always check the left argument for side-effects (@lukastaegert)

## 2.0.4

_2020-03-12_

### Bug Fixes

- Avoid conflicts between namespace imports when preserving modules (#3435)

### Pull Requests

- [#3435](https://github.com/rollup/rollup/pull/3435): Deconflict multiple `index` imports for ES format using nested export star statements (@kamranayub)

## 2.0.3

_2020-03-10_

### Bug Fixes

- Add type for this.getCombinedSourcemap to transform context (#3431)

### Pull Requests

- [#3377](https://github.com/rollup/rollup/pull/3377): Switch to yargs-parser lib (@jamesgeorge007)
- [#3426](https://github.com/rollup/rollup/pull/3426): Use strict types with PluginDriver (@NotWoods)
- [#3431](https://github.com/rollup/rollup/pull/3431): Add missing type declaration for getCombinedSourcemap ( @Anidetrix)
- [#3432](https://github.com/rollup/rollup/pull/3432): Detail how return values from `augmentChunkHash` are used ( @jakearchibald)

## 2.0.2

_2020-03-07_

### Bug Fixes

- Make sure the ESM import still works (#3430)

### Pull Requests

- [#3430](https://github.com/rollup/rollup/pull/3430): Fix conditional exports again (@lukastaegert)

## 2.0.1

_2020-03-07_

### Bug Fixes

- Reenable importing rollup in Node 13.0 - 13.7 (#3428)

### Pull Requests

- [#3428](https://github.com/rollup/rollup/pull/3428): Fix conditional exports in Node 13.0 - 13.7 (@lukastaegert)

## 2.0.0

_2020-03-06_

### Breaking Changes

- Rollup now requires at least Node 10 to run, or a sufficiently modern browser (#3346)
- The file structure of Rollup's ESM builds has changed:
  - The main ESM entry point is now at `rollup/dist/es/rollup.js` instead of `rollup/dist/rollup.es.js`
  - The ESM browser build is at `rollup/dist/es/rollup.browser.js` instead of `rollup/dist/rollup.browser.es.js`

  In general, the ESM builds now follow the same naming scheme as the CJS builds but are located in the `rollup/dist/es` subfolder instead of `rollup/dist` (#3391)

- The "watch.chokidar" option no longer accepts a `boolean` value but only an object of parameters that is passed to the bundled Chokidar instance. Chokidar installations by the user will be ignored in favour of the bundled instance ( #3331)
- Modules that are completely tree-shaken will no longer be listed as part of any chunks in `generateBundle`
- The `experimentalOptimizeChunks` and `chunkGroupingSize` options have been removed
- [acorn](https://github.com/acornjs/acorn) plugins can only be used if they accept a passed-in acorn instance instead of importing it themselves. See https://github.com/acornjs/acorn/pull/870#issuecomment-527339830 for what needs to be done to make plugins compatible that do not support this yet (#3391)
- Emitted chunks now have the TypeScript type `Uint8Array` instead of `Buffer`. A `Buffer` can still be used, though ( #3395)
- The TypeScript types no longer use ESTree types for AST nodes but a very generic type that does not contain information specific to certain node types (#3395)
- The signature of the `writeBundle` plugin hook has been changed to match `generateBundle`: The bundle object is now passed as second parameter instead of first and the first parameter is the output options (#3361)
- The following plugin hooks have been removed:
  - ongenerate: use `generateBundle` instead
  - onwrite: use `writeBundle` instead
  - transformBundle: use `renderChunk` instead
  - transformChunk: use `renderChunk` instead
- You can no longer access `this.watcher` on the plugin context.
- The `transform` hook can no longer return `dependencies`.
- The `treeshake.pureExternalModules` option will now show a deprecation warning when used: use `treeshake.moduleSideEffects: 'no-external'` instead
- Using `import.meta.ROLLUP_ASSET_URL_<..>` and `import.meta.ROLLUP_CHUNK_URL_<..>` in code will now show warnings: use `import.meta.ROLLUP_FILE_URL_<..>` instead
- The `resolveAssetUrl` hook will now show a deprecation warning when used: use `resolveFileUrl` instead
- The following plugin context functions will show warnings when used:
  - `this.emitAsset`: use `this.emitFile`
  - `this.emitChunk`: use `this.emitFile`
  - `this.getAssetFileName`: use `this.getFileName`
  - `this.getChunkFileName`: use `this.getFileName`
  - `this.isExternal`: use `this.resolve`
  - `this.resolveId`: use `this.resolve`
- Directly adding properties to the bundle object in the `generateBundle` is deprecated will show a warning (removing properties is allowed, though): Use `this.emitFile`
- Accessing `chunk.isAsset` on the bundle is deprecated: Use `chunk.type === 'asset'` instead
- The error code for a missing `name` property when targeting UMD has been changed to `MISSING_NAME_OPTION_FOR_IIFE_EXPORT` to emphasize this is needed for the IIFE part of UMD (#3393)

### Features

- Rollup now bundles [Chokidar](https://github.com/paulmillr/chokidar) for a better watch experience (#3331)
- Rollup now bundles [acorn](https://github.com/acornjs/acorn) again, removing its only external dependency (#3391)
- Do not consider empty imports from side-effect-free modules for chunking and hoist side-effect imports if necessary ( #3369)
- Rollup can now be imported as an ES module in Node via `import {rollup} from 'rollup'`. Note that this relies on Node's experimental [conditional package exports](https://nodejs.org/dist/latest-v13.x/docs/api/esm.html#esm_conditional_exports) feature and is therefore itself experimental (#3391)
- `systemjs` can be used as format alias for `system` (#3381)

### Bug Fixes

- Unknown output options now trigger a warning when using the JavaScript API (#3352)
- Rollup will no longer introduce Node types into TypeScript projects that do not use them (#3395)
- Generate correct sourcemaps when tree-shaking occurs in a multi-file bundle (#3423)

### Pull Requests

- [#3331](https://github.com/rollup/rollup/pull/3331): Bundle Chokidar (@lukastaegert)
- [#3343](https://github.com/rollup/rollup/pull/3343): Remove experimentalOptimizeChunks (@lukastaegert)
- [#3346](https://github.com/rollup/rollup/pull/3346): Update minimum required Node version to 10 (@lukastaegert)
- [#3352](https://github.com/rollup/rollup/pull/3352): Remove active deprecations (@lukastaegert)
- [#3361](https://github.com/rollup/rollup/pull/3361): Change writeBundle signature to match generateBundle ( @lukastaegert)
- [#3369](https://github.com/rollup/rollup/pull/3369): Avoid empty imports from side-effect-free chunks (@lukastaegert)
- [#3381](https://github.com/rollup/rollup/pull/3381): Rename esm to es everywhere, add systemjs alias (@lukastaegert)
- [#3391](https://github.com/rollup/rollup/pull/3391): Bundle acorn, allow importing Rollup as Node ES module, update dependencies (@lukastaegert)
- [#3393](https://github.com/rollup/rollup/pull/3393): Better error code for name-less umd bundle (@rail44)
- [#3395](https://github.com/rollup/rollup/pull/3395): Remove `@types` dependencies (@lukastaegert)
- [#3423](https://github.com/rollup/rollup/pull/3423): Update magic-string and fix sourcemaps (@lukastaegert)

## 1.32.1

_2020-03-06_

### Bug Fixes

- Handle default export detection for AMD and IIFE externals that do not have a prototype (#3420)
- Handle missing whitespace when the else branch of an if-statement is simplified (#3421)
- Mention the importing module when reporting errors for missing named exports (#3401)
- Add code to warning for missing output.name of IIFE bundles (#3372)

### Pull Requests

- [#3372](https://github.com/rollup/rollup/pull/3372): Add warning code for missing output.name of IIFE bundle that has export (@rail44)
- [#3401](https://github.com/rollup/rollup/pull/3401): Missing exports errors now print the importing module (@timiyay)
- [#3418](https://github.com/rollup/rollup/pull/3418): Structure lifecycle hooks, add links to build time hooks ( @lukastaegert)
- [#3420](https://github.com/rollup/rollup/pull/3420): Update generated code of getInteropBlock() to work with null prototype objects (@jdalton)
- [#3421](https://github.com/rollup/rollup/pull/3421): Avoid invalid code when "else" branch is simplified ( @lukastaegert)

## 1.32.0

_2020-02-28_

### Features

- Allow adding plugins on the command line via `--plugin <plugin>` (#3379)

### Pull Requests

- [#3379](https://github.com/rollup/rollup/pull/3379): introduce CLI --plugin support (@kzc)
- [#3390](https://github.com/rollup/rollup/pull/3390): fix typo: this.addWatchfile (@mistlog)
- [#3392](https://github.com/rollup/rollup/pull/3392): Bump codecov from 3.6.1 to 3.6.5
- [#3404](https://github.com/rollup/rollup/pull/3404): Update resolveFileUrl docs (@jakearchibald)

## 1.31.1

_2020-02-14_

### Bug Fixes

- Make sure errored files are always re-evaluated in watch mode to avoid an issue in the typescript plugin (#3388)

### Pull Requests

- [#3366](https://github.com/rollup/rollup/pull/3366): Correct spelling minifaction to minification (@VictorHom)
- [#3371](https://github.com/rollup/rollup/pull/3371): Adjust bug template to mention REPL.it (@lukastaegert)
- [#3388](https://github.com/rollup/rollup/pull/3388): Run transform hooks again in watch mode on files that errored ( @lukastaegert)

## 1.31.0

_2020-01-31_

### Features

- Always disable tree-shaking for asm.js functions to maintain semantics (#3362)

### Pull Requests

- [#3362](https://github.com/rollup/rollup/pull/3362): Preserve asm.js code (@lukastaegert)

## 1.30.1

_2020-01-27_

### Bug Fixes

- Do not mistreat static entgry points as dynamic ones when chunking (#3357)
- Resolve a crash when chunking circular dynamic imports (#3357)

### Pull Requests

- [#3357](https://github.com/rollup/rollup/pull/3357): Resolve issues with circular dynamic entries (@lukastaegert)

## 1.30.0

_2020-01-27_

### Features

- Do not split chunks when dynamically imported modules import modules that are already loaded by all dynamic importers (#3354)
- Add `hoistTransitiveImports` option to disable hoisting imports of static dependencies into entry chunks (#3353)

### Bug Fixes

- Make sure polyfills are always loaded first when each static entry point contains them as first import (#3354)

### Pull Requests

- [#3353](https://github.com/rollup/rollup/pull/3353): Add option to avoid hoisting transitive imports (@lukastaegert)
- [#3354](https://github.com/rollup/rollup/pull/3354): Improve chunking algorithm for dynamic imports (@tjenkinson and @lukastaegert)

## 1.29.1

_2020-01-21_

### Bug Fixes

- Avoid crashes for circular reexports when named exports cannot be found (#3350)

### Pull Requests

- [#3335](https://github.com/rollup/rollup/pull/3335): Fix typo (@robbinworks)
- [#3342](https://github.com/rollup/rollup/pull/3342): Remove ":" from test file names for Windows and update dependencies (@lukastaegert)
- [#3350](https://github.com/rollup/rollup/pull/3350): Properly handle circular reexports (@lukastaegert)

## 1.29.0

_2020-01-08_

### Features

- Enable top-level await by default (#3089)
- Add typings for watch events (#3302)

### Bug Fixes

- Deconflict files that would conflict only on a case-insensitive OS (#3317)
- Do not fail in certain scenarios where a logical expression inside a sequence expression was being directly included ( #3327)

### Pull Requests

- [#3089](https://github.com/rollup/rollup/pull/3089): Move top-level await out of experimental (@guybedford)
- [#3302](https://github.com/rollup/rollup/pull/3302): Adds type definitions for RollupWatcher events (@NotWoods)
- [#3317](https://github.com/rollup/rollup/pull/3317): Fix module id conflict on a case insensitive OS (@yesmeck)
- [#3327](https://github.com/rollup/rollup/pull/3327): Handle deoptimizations while a node is being included ( @lukastaegert)

## 1.28.0

_2020-01-04_

### Features

- Allow piping in stdin via the command line interface (#3312, #3290)
- Allow plugins to mark modules as having syntheticNamedExports for e.g. better CJS interoperability (#3295)
- Ignore variable reassignments in dead code when tree-shaking to remove more unneeded code (#3212)

### Bug Fixes

- Properly respect tree-shaken code when generating sourcemaps (#3318)

### Pull Requests

- [#3212](https://github.com/rollup/rollup/pull/3212): Handle assignments in dead code (@tjenkinson)
- [#3290](https://github.com/rollup/rollup/pull/3290): Implement stdin input with optional "-" as the file name (@kzc)
- [#3295](https://github.com/rollup/rollup/pull/3295): Add syntheticNamedExports (@manucorporat)
- [#3300](https://github.com/rollup/rollup/pull/3300): Add note about setting `types` in tsconfig file (@tjenkinson)
- [#3303](https://github.com/rollup/rollup/pull/3303): Use ! to assert not-null in TypeScript (@NotWoods)
- [#3312](https://github.com/rollup/rollup/pull/3312): Implement stdin input (@lukastaegert)
- [#3318](https://github.com/rollup/rollup/pull/3318): Update magic-string and other dependencies (@lukastaegert)

## 1.27.14

_2019-12-22_

### Bug Fixes

- Update references to official rollup plugins in error messages (#3297, #3298)

### Pull Requests

- [#3286](https://github.com/rollup/rollup/pull/3286): Update link to JavaScript API documentation (@romankaravia)
- [#3294](https://github.com/rollup/rollup/pull/3294): Update deprecated references to the node-resolve plugin in the documentation (@Vlad-Shcherbina)
- [#3297](https://github.com/rollup/rollup/pull/3297): Update references to rollup-plugin-json (@cprecioso)
- [#3298](https://github.com/rollup/rollup/pull/3298): Update references to official rollup plugins (@cprecioso)

## 1.27.13

_2019-12-14_

### Bug Fixes

- Do not truncate environment variable values at the first colon when using the `--environment` option (#3283)

### Pull Requests

- [#3283](https://github.com/rollup/rollup/pull/3283): Allow environment variables to contain colons (@tlaverdure)

## 1.27.12

_2019-12-13_

### Bug Fixes

- Prevent invalid AMD or SystemJS code when accessing `import.meta` (#3282)

### Pull Requests

- [#3282](https://github.com/rollup/rollup/pull/3282): Always make "module" available for SystemJS and AMD formats if `import.meta` is accessed directly (@lukastaegert)

## 1.27.11

_2019-12-12_

### Bug Fixes

- Resolve a crash due to an infinite loop (#3280)

### Pull Requests

- [#3280](https://github.com/rollup/rollup/pull/3280): Prevent infinite deoptimizations (@lukastaegert)

## 1.27.10

_2019-12-11_

### Bug Fixes

- Keep track of function return values in more situations (#3278)

### Pull Requests

- [#3278](https://github.com/rollup/rollup/pull/3278): Avoid some unnecessary value tracking deoptimizations ( @lukastaegert)

## 1.27.9

_2019-12-07_

### Bug Fixes

- Fix an issue where reexports could be missing when preserving modules (#3273)
- Allow turning of color output via NO_COLOR or FORCE_COLOR=0 environment variables (#3272)

### Pull Requests

- [#3272](https://github.com/rollup/rollup/pull/3272): Support either NO_COLOR or FORCE_COLOR=0 to turn off color ( @kikonen)
- [#3273](https://github.com/rollup/rollup/pull/3273): Make sure that indirectly reexported modules also become chunk dependencies when preserving modules(@lukastaegert)

## 1.27.8

_2019-12-02_

### Bug Fixes

- Deoptimize objects when a method is called on them to make sure modifications via "this" are observed (#3266)

### Pull Requests

- [#3266](https://github.com/rollup/rollup/pull/3266): Workaround for various object literal mutation bugs (@kzc)

## 1.27.7

_2019-12-01_

### Bug Fixes

- Fix a scenario where a reassignments to computed properties were not tracked (#3267)

### Pull Requests

- [#3267](https://github.com/rollup/rollup/pull/3267): Fix incomplete computed property deoptimization (@lukastaegert)

## 1.27.6

_2019-11-30_

### Bug Fixes

- Use "auto" export mode by default for all modules when preserving modules (#3265)
- Observe "output.exports" when preserving modules and warn for mixed exports if necessary (#3265)

### Pull Requests

- [#3265](https://github.com/rollup/rollup/pull/3265): Use export mode "auto" by default when preserving modules ( @lukastaegert)

## 1.27.5

_2019-11-25_

### Bug Fixes

- Make sure namespaces for inlined dynamic imports are treated as variable accesses when deconflicting (#3256)

### Pull Requests

- [#3256](https://github.com/rollup/rollup/pull/3256): Avoid name conflicts when inlining dynamic imports nested in functions (@lukastaegert)
- [#3257](https://github.com/rollup/rollup/pull/3257): Update dependencies (@lukastaegert)

## 1.27.4

_2019-11-22_

### Bug Fixes

- Aggregate circular dependency warnings in the CLI (#3249)
- Do not defer non-aggregated handlers in the CLI (#3249)

### Pull Requests

- [#3249](https://github.com/rollup/rollup/pull/3249): Fix broken Windows CLI tests (@lukastaegert)
- [#3251](https://github.com/rollup/rollup/pull/3251): Add installation as a separate header (@ashrith-kulai)

## 1.27.3

_2019-11-20_

### Bug Fixes

- Provide better warning when empty chunks are created in a code-splitting scenario (#3244)

### Pull Requests

- [#3244](https://github.com/rollup/rollup/pull/3244): Clearer empty chunk warning (@tjenkinson)

## 1.27.2

_2019-11-18_

### Bug Fixes

- Fix an issue where live bindings were not working correctly when using `+=` in SystemJS (#3242)

### Pull Requests

- [#3242](https://github.com/rollup/rollup/pull/3242): Export updated assignments when using shorthand update assignment expressions in SystemJS (@lukastaegert)

## 1.27.1

_2019-11-18_

### Bug Fixes

- Fix an issue where code after a switch-statement with removed cases was erroneously not included (#3241)

### Pull Requests

- [#3237](https://github.com/rollup/rollup/pull/3237): make `acornOptions` optional in `parse()` in docs (@tjenkinson)
- [#3240](https://github.com/rollup/rollup/pull/3240): Update dependencies and fix vulnerability (@lukastaegert)
- [#3241](https://github.com/rollup/rollup/pull/3241): Do not truncate after switch-statement with removed case ( @lukastaegert)

## 1.27.0

_2019-11-12_

### Features

- Add support for output-specific plugins (#3218)
- Reenable parallel output processing when using the CLI (#3218)
- Warn if files are emitted that would overwrite previously emitted files (#3218)

### Bug Fixes

- Do not overwrite files emitted in other builds if outputs are generated in parallel (#3218)

### Pull Requests

- [#3218](https://github.com/rollup/rollup/pull/3218): Per output plugins (@lukastaegert)

## 1.26.5

_2019-11-11_

### Bug Fixes

- Fix a regression where it was no longer to pass a certain option format to generate (#3223)

### Pull Requests

- [#3223](https://github.com/rollup/rollup/pull/3223): Allow passing input options to output (@lukastaegert)

## 1.26.4

_2019-11-09_

### Bug Fixes

- Keep watching known files after a plugin error during the initial build (#3219)

### Pull Requests

- [#3216](https://github.com/rollup/rollup/pull/3216): Fix small typo (@kaisermann)
- [#3217](https://github.com/rollup/rollup/pull/3217): Update dependencies and fix security vulnerability ( @lukastaegert)
- [#3219](https://github.com/rollup/rollup/pull/3219): Also recover from plugin errors during the initial build ( @lukastaegert)

## 1.26.3

_2019-11-02_

### Bug Fixes

- Work around an incompatibility with rollup-plugin-dts (#3211)

### Pull Requests

- [#3211](https://github.com/rollup/rollup/pull/3211): Do no fail if the source attribute is `undefined` in an unused named export (@lukastaegert)

## 1.26.2

_2019-10-31_

### Bug Fixes

- Do not create invalid code when using `treeshake: false` and star re-exports (#3209)

### Pull Requests

- [#3209](https://github.com/rollup/rollup/pull/3209): Also remove export-all declarations when not tree-shaking ( @lukastaegert)

## 1.26.1

_2019-10-31_

### Bug Fixes

- Prevent an issue where outputs would overwrite files emitted by other outputs (#3201)
- Do not throw an error if the config file does not have a .js extension (#3204)

### Pull Requests

- [#3201](https://github.com/rollup/rollup/pull/3201): Make the CLI run generate/output in serial (@marijnh)
- [#3204](https://github.com/rollup/rollup/pull/3204): support all config file extensions (.js,.mjs,...) (@arlac77)

## 1.26.0

_2019-10-27_

### Features

- Only warn when no output is provided for an IIFE bundle but still produce valid code (#3181)
- Support reexporting namespaces as a binding (#3193)
- Switch from hash.js to crypto for hashing in the Node build for better performance and support for very large assets ( #3194)

### Bug Fixes

- Correctly handle chunks reexporting the same namespace as two different bindings (#3193)

### Pull Requests

- [#3181](https://github.com/rollup/rollup/pull/3181): Remove the need to provide an output name for IIFE bundles ( @bterrier)
- [#3193](https://github.com/rollup/rollup/pull/3193): Add support for "export \* as name from …" (@lukastaegert)
- [#3194](https://github.com/rollup/rollup/pull/3194): Add support for large assets (> 100 MB) (@SebastianNiemann)

## 1.25.2

_2019-10-23_

### Bug Fixes

- Improve performance of bundled UMD code by adding additional parentheses to enforce eager parsing (#3183)
- Improve types to tolerate passing a Rollup config with multiple outputs to `rollup.rollup` (#3184)

### Pull Requests

- [#3183](https://github.com/rollup/rollup/pull/3183): Add parentheses to factory function of UMD bundles (@ajihyf)
- [#3184](https://github.com/rollup/rollup/pull/3184): RollupOptions accept output as array (@imcotton)

## 1.25.1

_2019-10-20_

### Bug Fixes

- Handle a situation where code was not included after a switch statement (#3178)
- Handle a situation where code was not included after a do-while loop (#3180)
- Do not fail if different outputs emit the same file (#3175)
- Give access to the original acorn error for parse errors (#3176)

### Pull Requests

- [#3175](https://github.com/rollup/rollup/pull/3175): Disable errors for duplicate emitted file names (@marijnh)
- [#3176](https://github.com/rollup/rollup/pull/3176): Add original parser error to rollup error; Update tests ( @gribnoysup)
- [#3178](https://github.com/rollup/rollup/pull/3178): Fix switch case not being included correctly (@lukastaegert)
- [#3179](https://github.com/rollup/rollup/pull/3179): Update dependencies (@lukastaegert)
- [#3180](https://github.com/rollup/rollup/pull/3180): Handle conditional breaks in do-while loops with unconditional return (@lukastaegert)

## 1.25.0

_2019-10-18_

### Features

- Remove try-catch if there is no side-effect in the try-block (#3166)
- Omit side-effect-free trailing cases in switch-statements (#3166)
- Remove unused labels (#3170)

### Bug Fixes

- Do not remove code after labeled statements that contain a throw or return if the label is used (#3170)
- Prevent invalid code when expressions are simplified that do not follow a white-space character (#3173)
- Do not remove continue statements inside switch statements (#3166)
- Prevent trailing empty lines when tree-shaking inside switch statements (#3166)

### Pull Requests

- [#3166](https://github.com/rollup/rollup/pull/3166): Better try statement tree shaking (@lukastaegert)
- [#3170](https://github.com/rollup/rollup/pull/3170): Handle optional control flow in labeled statements, remove unused labels (@lukastaegert)
- [#3173](https://github.com/rollup/rollup/pull/3173): Add missing spaces in certain statements and expressions to avoid invalid code (@lukastaegert)

## 1.24.0

_2019-10-15_

### Features

- Respect `break`, `continue`, `return` and `throw` when tree-shaking to detect dead code (#3153)
- Do treat treat hoisted function declarations as "unknown" when checking for call side-effects (#3153)

### Bug Fixes

- Make sure that unknown `import.meta` properties produce valid code in SystemJS (#3152)
- Make sure `treeshake.annotations: false` is respected for class instantiation (#3153)
- Check property access side-effects for class instantiation (#3153)
- Do not suppress break statements inside labeled statements (#3153)

### Pull Requests

- [#3152](https://github.com/rollup/rollup/pull/3152): Allow import.meta.\* for systemjs format (@dmail)
- [#3153](https://github.com/rollup/rollup/pull/3153): Get rid of immutable.js and implement tree-shaking for broken control flow (@lukastaegert)

## 1.23.1

_2019-10-05_

### Bug Fixes

- Fix a regression where the node types had a specific minimal version (#3143)

### Pull Requests

- [#3143](https://github.com/rollup/rollup/pull/3143): Ensure that types packages have star version ranges ( @lukastaegert)

## 1.23.0

_2019-10-03_

### Features

- Add placeholders for extensions when preserving modules (#3116)

### Pull Requests

- [#3116](https://github.com/rollup/rollup/pull/3116): Include extensions in preserveModules output filenames for scriptified assets (@Andarist)
- [#3142](https://github.com/rollup/rollup/pull/3142): Fix typo (@tu4mo)

## 1.22.0

_2019-09-29_

### Features

- Add a new "hidden" sourcemap type that generates the map files but omits the sourcemap comment (#3120)
- Generate more efficient code when using `namespaceToStringTag: true` (#3135)
- Make sure namespace objects do not have a prototype (#3136)

### Bug Fixes

- Do not ignore side-effectful iterators by always preserving for..of loops for now (#3132)
- Make sure `--context` is observed as a CLI option (#3134)
- Do not require specific versions for @types dependencies (#3131)

### Pull Requests

- [#3120](https://github.com/rollup/rollup/pull/3120): Generate sourcemaps but omit the comment (@rohitmohan96)
- [#3131](https://github.com/rollup/rollup/pull/3131): Use asterisk for @types/\* dependencies (@frenzzy)
- [#3132](https://github.com/rollup/rollup/pull/3132): Preserve empty for...of loops (@imatlopez)
- [#3133](https://github.com/rollup/rollup/pull/3133): Update dependencies (@lukastaegert)
- [#3134](https://github.com/rollup/rollup/pull/3134): Wire up --context CLI flag (@tchetwin)
- [#3135](https://github.com/rollup/rollup/pull/3135): Remove Symbol polyfill in module namespaces (@mkubilayk)
- [#3136](https://github.com/rollup/rollup/pull/3136): Set null prototype on namespace objects (@rpamely)

## 1.21.4

_2019-09-16_

### Bug Fixes

- Recognize common browser globals (#3117)
- Do not treat "typeof <global>" as a side-effect (#3117)

### Pull Requests

- [#3117](https://github.com/rollup/rollup/pull/3117): Add browser globals to known globals and prevent "typeof" side-effects (@lukastaegert)

## 1.21.3

_2019-09-14_

### Bug Fixes

- Fix a regression where modifying a watched file did not trigger a rebuild (#3112)

### Pull Requests

- [#3112](https://github.com/rollup/rollup/pull/3112): Fix .addWatchFile() dependencies failing to invalidate in watch mode (@tivac)

## 1.21.2

_2019-09-09_

### Bug Fixes

- Fix wrong deprecation message to direct to `this.emitFile` instead of `this.emitAsset`

## 1.21.1

_2019-09-09_

### Bug Fixes

- Allow legacy plugins to still add assets directly to the bundle object (#3105)

### Pull Requests

- [#3105](https://github.com/rollup/rollup/pull/3105): Allow legacy plugins to still add assets directly to the bundle object (@lukastaegert)

## 1.21.0

_2019-09-08_

### Features

- Respect `output.entryFileNames` when preserving modules (#3088)
- Make accessing unknown globals a side-effect unless this is deactivated via `treeshake.unknownGlobalSideEffects` ( #3068)
- Respect global objects when checking for pure global functions (#3068)
- Introduce a `type` to more easily distinguish chunks and assets in the output bundle (#3080)

### Bug Fixes

- Recover in watch mode when the initial build fails (#3081)
- Make sure `output.strict` is respected for SystemJS output (#3101)

### Pull Requests

- [#3068](https://github.com/rollup/rollup/pull/3068): Make accessing unknown globals a side-effect (@lukastaegert)
- [#3080](https://github.com/rollup/rollup/pull/3080): OutputBundle Tagged union with 'type = chunk|asset' (@askbeka)
- [#3081](https://github.com/rollup/rollup/pull/3081): Watch files onbuild, even if build fails (@mhkeller)
- [#3088](https://github.com/rollup/rollup/pull/3088): Add support for entryFileNames pattern used in combination with preserveModules option (@Andarist)
- [#3101](https://github.com/rollup/rollup/pull/3101): Remove 'use strict'; from systemjs when strict=false (@askbeka)

## 1.20.3

_2019-08-28_

### Bug Fixes

- Make sure file hashes change when a change of the naming pattern leads to a file name change of a dependency (#3083)
- Fix several issues where reexporting an external "default" export could lead to invalid or incorrect code (#3084)

### Pull Requests

- [#3078](https://github.com/rollup/rollup/pull/3078): Add github actions workflow config for windows (@shellscape)
- [#3083](https://github.com/rollup/rollup/pull/3083): Properly reflect dependency file names in hash (@lukastaegert)
- [#3084](https://github.com/rollup/rollup/pull/3084): Fix "default" reexport issues in non ESM/System formats ( @lukastaegert)

## 1.20.2

_2019-08-25_

### Bug Fixes

- Avoid an issue where circular namespace reexports would crash Rollup (#3074)

### Pull Requests

- [#3077](https://github.com/rollup/rollup/pull/3077): Handle namespaces that reexport themselves (@lukastaegert)

## 1.20.1

_2019-08-22_

### Bug Fixes

- Fix an issue where variable names inside dynamic import expressions were not rendered correctly (#3073)
- Fix type definition to allow a single watcher config as well as an array (#3074)

### Pull Requests

- [#3073](https://github.com/rollup/rollup/pull/3073): Fix wrong variable name in import expression (@lukastaegert)
- [#3074](https://github.com/rollup/rollup/pull/3074): Fixes type definition on watch and Watcher constructor ( @MicahZoltu)

## 1.20.0

_2019-08-21_

### Features

- Add augmentChunkHash plugin hook to be able to reflect changes in renderChunk in the chunk hash (#2921)

### Bug Fixes

- Do not mutate the acorn options object (#3051)
- Make sure the order of emitted chunks always reflects the order in which they were emitted (#3055)
- Do not hang when there are strings containing comment-like syntax in some scenarios (#3069)

### Pull Requests

- [#2921](https://github.com/rollup/rollup/pull/2921): Add augmentChunkHash plugin hook (@isidrok)
- [#2995](https://github.com/rollup/rollup/pull/2995): Add info on installing locally to docs (@mesqueeb)
- [#3037](https://github.com/rollup/rollup/pull/3037): Refresh pull request labels (@shellscape)
- [#3048](https://github.com/rollup/rollup/pull/3048): Document ROLLUP_WATCH environment variable (@shellscape)
- [#3051](https://github.com/rollup/rollup/pull/3051): Avoid changes to the original options (.acorn) object ( @LongTengDao)
- [#3052](https://github.com/rollup/rollup/pull/3052): Minor refactoring: Remove one try-catch (@KSXGitHub)
- [#3053](https://github.com/rollup/rollup/pull/3053): Refactor to use async-await in more places (@KSXGitHub)
- [#3055](https://github.com/rollup/rollup/pull/3055): Provide consistent chunking via a consistent order of entry modules when emitting chunks (@lukastaegert)
- [#3058](https://github.com/rollup/rollup/pull/3058): Remove acorn-bigint and acorn-dynamic-import from bundle ( @LongTengDao)
- [#3061](https://github.com/rollup/rollup/pull/3061): Update to acorn@7 (@lukastaegert)
- [#3063](https://github.com/rollup/rollup/pull/3063): Auto-generate license file (@lukastaegert)
- [#3069](https://github.com/rollup/rollup/pull/3069): Prevent infinite loop when scanning for line-breaks and there are comment-like strings (@lukastaegert)

## 1.19.4

_2019-08-07_

### Bug Fixes

- Prevent invalid code when exporting an external namespace (#3034)
- Prevent invalid or non-equivalent code when simplifying expressions in return and throw statements (#3035)

### Pull Requests

- [#3034](https://github.com/rollup/rollup/pull/3034): Avoid generating .\* as export (@LongTengDao)
- [#3035](https://github.com/rollup/rollup/pull/3035): Prevent ASI errors for conditional expressions (@lukastaegert)
- [#3036](https://github.com/rollup/rollup/pull/3036): Fix documents to use https, not http (@giraffate)

## 1.19.3

_2019-08-06_

### Bug Fixes

- Fix wrong URLs in error messages (#3033)

### Pull Requests

- [#3033](https://github.com/rollup/rollup/pull/3033): Fix wrong URLs in error messages (@giraffate)

## 1.19.2

_2019-08-05_

### Bug Fixes

- Add bin file to package

## 1.19.1

_2019-08-05_

### Bug Fixes

- Remove wrong extension in package.json file (#3031)

### Pull Requests

- [#3031](https://github.com/rollup/rollup/pull/3031): Fix wrong extension (@lukastaegert)

## 1.19.0

_2019-08-05_

### Features

- Implement a new unified file emission API for assets and chunks with support for explicit file names (#2999)
- Use the id of the last module in a chunk as base for the chunk name if no better name is available (#3025)
- Use the id of the last module in a chunk as base for the variable name of a chunk in some formats if no better name is available (#2999)

### Bug Fixes

- Do not produce invalid variable names if an empty name is chosen for a virtual module (#3026)
- Fix an issue where a module variable name would conflict with a local variable name in some formats (#3020)

### Pull Requests

- [#2999](https://github.com/rollup/rollup/pull/2999): Unified file emission api (@lukastaegert)
- [#3020](https://github.com/rollup/rollup/pull/3020): Switch to a code-splitting build and update dependencies ( @lukastaegert)
- [#3025](https://github.com/rollup/rollup/pull/3025): Use id of last module in chunk as name base for auto-generated chunks (@lukastaegert)
- [#3026](https://github.com/rollup/rollup/pull/3026): Avoid variable from empty module name be empty (@LongTengDao)

## 1.18.0

_2019-08-01_

### Features

- Add `externalLiveBindings: false` option to optimize code when live bindings are not needed (#3010)

### Pull Requests

- [#2997](https://github.com/rollup/rollup/pull/2997): Integrate coverage into CI setup (@lukastaegert)
- [#2998](https://github.com/rollup/rollup/pull/2998): Update readme badges (@lukastaegert)
- [#3010](https://github.com/rollup/rollup/pull/3010): Add option to prevent code for external live bindings ( @lukastaegert)

## 1.17.0

_2019-07-15_

### Features

- Allow plugins to access current combined sourcemap in transform hook for coverage instrumentation (#2993)

### Pull Requests

- [#2987](https://github.com/rollup/rollup/pull/2987): Fix code fences for link (@johanholmerin)
- [#2989](https://github.com/rollup/rollup/pull/2989): Bump lodash from 4.17.11 to 4.17.14 (@dependabot)
- [#2993](https://github.com/rollup/rollup/pull/2993): Add getCombinedSourceMap in transform plugin context (@billowz)

## 1.16.7

_2019-07-09_

### Bug Fixes

- Fix an issue where exported import.meta properties would lead to invalid code (#2986)

### Pull Requests

- [#2985](https://github.com/rollup/rollup/pull/2985): Improve sourcemap types (@jridgewell)
- [#2986](https://github.com/rollup/rollup/pull/2986): Only overwrite content when resolving import.meta properties ( @lukastaegert)

## 1.16.6

_2019-07-04_

### Bug Fixes

- Do not pass undefined to resolveDynamicImport for unresolvable template literals (#2984)

### Pull Requests

- [#2984](https://github.com/rollup/rollup/pull/2984): Always forward AST nodes for unresolvable dynamic imports ( @lukastaegert)

## 1.16.5

_2019-07-04_

### Bug Fixes

- onwarn should still be called when --silent is used (#2982)
- Properly clean up watchers for files that are deleted between builds (#2982)

### Pull Requests

- [#2981](https://github.com/rollup/rollup/pull/2981): Do not skip onwarn handler when --silent is used (@lukastaegert)
- [#2982](https://github.com/rollup/rollup/pull/2982): Make tests run on Node 12, fix watcher cleanup issue ( @lukastaegert)

## 1.16.4

_2019-07-02_

### Bug Fixes

- Do not show a TypeScript error when providing a location as number to this.warn and this.error (#2974)
- Use the correct TypeScript type for Sourcemap.version (#2976)

### Pull Requests

- [#2965](https://github.com/rollup/rollup/pull/2965): Use async readFile in getRollupDefaultPlugin (@kaksmet)
- [#2974](https://github.com/rollup/rollup/pull/2974): Align TS types, docs and implementation for this.warn and this.error (@lukastaegert)
- [#2976](https://github.com/rollup/rollup/pull/2976): Fix sourcemap type and update dependencies (@lukastaegert)

## 1.16.3

_2019-06-29_

### Bug Fixes

- Prevent name conflicts with unused function parameters (#2972)

### Pull Requests

- [#2972](https://github.com/rollup/rollup/pull/2972): Deconflict unused parameters (@lukastaegert)

## 1.16.2

_2019-06-22_

### Bug Fixes

- Properly wrap dynamic imports in Promises that can be caught when generating CJS output (#2958)

### Pull Requests

- [#2958](https://github.com/rollup/rollup/pull/2958): Make sure errors from dynamic imports can be caught ( @lukastaegert)

## 1.16.1

_2019-06-21_

### Pull Requests

- [#2956](https://github.com/rollup/rollup/pull/2956): Add missing CLI docs for strictDeprecations (@lukastaegert)

## 1.16.0

_2019-06-21_

### Features

- Add strictDeprecations option to throw when currently or upcoming deprecated features are used (#2945)
- Keep annotations and comments when simplifying logical and conditional expressions (#2955)

### Bug Fixes

- Generate proper namespace objects when dynamically importing external dependencies for AMD or CJS formats (#2954)
- Fix dynamically imported variables not being resolved correctly when importing from an entry chunk with only a default export (#2954)
- Do not reexport default when reexporting a namespace (#2954)

### Pull Requests

- [#2945](https://github.com/rollup/rollup/pull/2945): Add option to handle use of features marked for deprecation as errors (@lukastaegert)
- [#2954](https://github.com/rollup/rollup/pull/2954): Improve dynamic import interop (@lukastaegert)
- [#2955](https://github.com/rollup/rollup/pull/2955): Keep annotations and comments when simplifying logical and conditional expressions (@lukastaegert)

## 1.15.6

_2019-06-16_

### Bug Fixes

- No longer use an alternate screen in watch mode to allow scrolling (#2942)
- Prioritize non-external imports over external ones when resolving conflicting namespace re-exports (#2893)

### Pull Requests

- [#2893](https://github.com/rollup/rollup/pull/2893): Improve handling of conflicting namespace exports (@aleclarson)
- [#2942](https://github.com/rollup/rollup/pull/2942): Get rid of alternate screen and simplify screen clearing ( @lukastaegert)

## 1.15.5

_2019-06-14_

### Bug Fixes

- Do not include any comments for completely tree-shaken files so that `renderedLength === 0` is a reliable check ( #2940)
- Do not cause type errors when returning `null` from `resolveId` (#2941)

### Pull Requests

- [#2940](https://github.com/rollup/rollup/pull/2940): Completely omit files that do not have any included statements ( @lukastaegert)
- [#2941](https://github.com/rollup/rollup/pull/2941): Explicitly allow null as return value for various hooks ( @lukastaegert)

## 1.15.4

_2019-06-14_

### Bug Fixes

- Improve how asset and chunk URLs are resolved for UMD, IIFE and CJS output (#2937)

### Pull Requests

- [#2937](https://github.com/rollup/rollup/pull/2937): Fix URL resolution to work when the current script contains query parameters (@lukastaegert)

## 1.15.3

_2019-06-13_

### Bug Fixes

- Always reemit assets and chunks from cached transform hooks (#2936)

### Pull Requests

- [#2936](https://github.com/rollup/rollup/pull/2936): Fix repeated re-emission of files emitted from a transform hook ( @lukastaegert)

## 1.15.2

_2019-06-13_

### Bug Fixes

- Make sure chunks emitted from transform hooks are also emitted for incremental builds in watch mode (#2933)

### Pull Requests

- [#2933](https://github.com/rollup/rollup/pull/2933): Reemit chunks emitted from transform hooks (@lukastaegert)

## 1.15.1

_2019-06-11_

### Bug Fixes

- Do not fail when reexporting variables in dynamic entry points from other chunks (#2928)

### Pull Requests

- [#2928](https://github.com/rollup/rollup/pull/2928): Handle reexports from dynamic entries across chunk ( @lukastaegert)

## 1.15.0

_2019-06-11_

### Features

- Tone down try-catch deoptimization while maintaining polyfill support (#2918)

### Bug Fixes

- Handle feature detection with "typeof" for regular expressios (#2916)
- Deoptimize `'' + variable'` type coercion as expression statement for feature detection (#2917)
- Always observe argument side-effects when tree-shaking (#2924)

### Pull Requests

- [#2916](https://github.com/rollup/rollup/pull/2916): Deoptimize typeof for regular expression literals to better support es6-shim (@lukastaegert)
- [#2917](https://github.com/rollup/rollup/pull/2917): Support implicit type coercion errors in es5-shim (@lukastaegert)
- [#2918](https://github.com/rollup/rollup/pull/2918): Deoptimize try-catch less radically (@lukastaegert)
- [#2924](https://github.com/rollup/rollup/pull/2924): Do not tree-shake arguments with side-effects (@lukastaegert)

## 1.14.6

_2019-06-10_

### Bug Fixes

- Fix an issue where call arguments were not included in try statements (#2914)

### Pull Requests

- [#2914](https://github.com/rollup/rollup/pull/2914): Properly include try statements for each pass when deoptimization is deactivated (@lukastaegert)

## 1.14.5

_2019-06-09_

### Bug Fixes

- Keep external ids unmodified when using the object form of resolveId (#2907)
- Cache dynamic import resolutions when using Rollup cache (#2908)
- Keep all necessary parentheses when tree-shaking call arguments (#2911)

### Pull Requests

- [#2906](https://github.com/rollup/rollup/pull/2906): Update dependencies (@lukastaegert)
- [#2907](https://github.com/rollup/rollup/pull/2907): Do not renormalize external ids when using the object form ( @lukastaegert)
- [#2908](https://github.com/rollup/rollup/pull/2908): Cache dynamic ids if possible (@lukastaegert)
- [#2911](https://github.com/rollup/rollup/pull/2911): Fix treeshaken parameters around parentheses (@manucorporat)

## 1.14.4

_2019-06-07_

### Bug Fixes

- Do not omit external re-exports for `moduleSideEffects: false` (#2905)

### Pull Requests

- [#2905](https://github.com/rollup/rollup/pull/2905): Make sure external re-exports are included for moduleSideEffects: false (@lukastaegert)

## 1.14.3

_2019-06-06_

### Bug Fixes

- Generate correct external imports when importing from a directory that would be above the root of the current working directory (#2902)

### Pull Requests

- [#2902](https://github.com/rollup/rollup/pull/2902): Use browser relative path algorithm for chunks (@lukastaegert)

## 1.14.2

_2019-06-05_

### Bug Fixes

- Prevent unnecessary inclusion of external namespace import in certain situations (#2900)

### Pull Requests

- [#2900](https://github.com/rollup/rollup/pull/2900): Handle early bind for member expressions (@lukastaegert)

## 1.14.1

_2019-06-05_

### Bug Fixes

- Fix an issue where try-statements were not included properly when a variable declared inside the statement was accessed outside it (#2898)
- Fix an issue where `await` expressions were not included properly (#2899)

### Pull Requests

- [#2898](https://github.com/rollup/rollup/pull/2898): Properly include try-catch-statements even if they have already been included in some way (@lukastaegert)
- [#2899](https://github.com/rollup/rollup/pull/2899): Fix unintended early return in await inclusion handling ( @lukastaegert)

## 1.14.0

_2019-06-05_

### Features

- Deoptimize code inside and called from try-statements for feature detection (#2892)
- Tree-shake unused call arguments (#2892)

### Pull Requests

- [#2892](https://github.com/rollup/rollup/pull/2892): Implement try-statement-deoptimization for feature detection, tree-shake unused arguments (@lukastaegert)

## 1.13.1

_2019-06-01_

### Bug Fixes

- Avoid conflicts between top-level module, require etc. and CommonJS runtimes (#2889)

### Pull Requests

- [#2888](https://github.com/rollup/rollup/pull/2888): Enable full TypeScript strict mode (@lukastaegert)
- [#2889](https://github.com/rollup/rollup/pull/2889): Protect all module globals for CJS output from being redefined ( @lukastaegert)

## 1.13.0

_2019-05-31_

### Features

- Omit `exports` and `module` from SystemJS wrapper if possible (#2880)
- Try to use the first letters of names when mangling exports (#2885)

### Bug Fixes

- Avoid conflicts with local variables when using format specific globals to render dynamic imports and file URLs ( #2880)
- Do not produce undefined reexports when reexporting from entry points (#2885)

### Pull Requests

- [#2880](https://github.com/rollup/rollup/pull/2880): Deconflict global variables used inside format-specific code ( @lukastaegert)
- [#2885](https://github.com/rollup/rollup/pull/2885): Do not produce undefined reexports when reexporting from entry points and refactor chunk linking (@lukastaegert)

## 1.12.5

_2019-05-30_

### Pull Requests

- [#2884](https://github.com/rollup/rollup/pull/2884): Update pluginutils for new micormatch and reduced bundle size ( @lukastaegert)

## 1.12.4

_2019-05-27_

### Bug Fixes

- Show correct error stack trace for errors throw in "load" hooks (#2871)

### Pull Requests

- [#2875](https://github.com/rollup/rollup/pull/2875): Mention subfolders in docs (@lukastaegert)
- [#2871](https://github.com/rollup/rollup/pull/2871): Reserve error stack information (@LongTengDao)

## 1.12.3

_2019-05-19_

### Bug Fixes

- Prevent duplicate imports when exports are reexported as default exports (#2866)

### Pull Requests

- [#2755](https://github.com/rollup/rollup/pull/2755): Enable TypeScript strictNullChecks (@edsrzf)
- [#2866](https://github.com/rollup/rollup/pull/2866): Properly deduplicate reexported default exports (@lukastaegert)

## 1.12.2

_2019-05-17_

### Bug Fixes

- Do not fail when using clearScreen:false in watchMode (#2858)
- Properly resolve star reexports when preserving modules (#2860)

### Pull Requests

- [#2858](https://github.com/rollup/rollup/pull/2858): Declare processConfigsErr before use (@humphd)
- [#2860](https://github.com/rollup/rollup/pull/2860): Keep nested exports with preserveModules (@TomCaserta)
- [#2864](https://github.com/rollup/rollup/pull/2864): Cache transitive reexport detection (@lukastaegert)

## 1.12.1

_2019-05-16_

### Bug Fixes

- Extend file name sanitation to also replace "?" and "\*" e.g. when preserving modules with the updated commonjs plugin (#2860)
- Do not ignore module transformer that return an empty string (#2861)

### Pull Requests

- [#2860](https://github.com/rollup/rollup/pull/2860): Update to latest plugins and extend file name sanitation ( @lukastaegert)
- [#2861](https://github.com/rollup/rollup/pull/2861): Allow transformers to return an empty string (@lukastaegert)

## 1.12.0

_2019-05-15_

### Features

- Add `treeshake.moduleSideEffects` option to allow removing empty imports without a side-effect check (#2844)
- Extend plugin API to allow marking modules as side-effect-free (#2844)
- Extend `this.resolve` plugin context function with an option to skip the `resolveId` hook of the calling plugin ( #2844)
- Add `isEntry` flag to `this.getModuleInfo` plugin context function (#2844)
- Distribute Rollup as optimized ES2015 code (#2851)

### Pull Requests

- [#2844](https://github.com/rollup/rollup/pull/2844): Add options and hooks to control module side effects ( @lukastaegert)
- [#2851](https://github.com/rollup/rollup/pull/2851): Switch to ES2015 output (@lukastaegert)

## 1.11.3

_2019-05-05_

### Bug Fixes

- Quote es3 keywords in namespace objects (#2825)

### Pull Requests

- [#2825](https://github.com/rollup/rollup/pull/2825): Add es3 support for namespace object import (@sormy)

## 1.11.2

_2019-05-04_

### Bug Fixes

- Prevent a crash when handling circular namespace exports (#2836)

### Pull Requests

- [#2836](https://github.com/rollup/rollup/pull/2836): Make sure circular `export * from X` does not stack overflow ( @Swatinem)

## 1.11.1

_2019-05-04_

### Bug Fixes

- Fix an issue where rendered exports were reported as "removed" in the bundle information (#2835)

### Pull Requests

- [#2835](https://github.com/rollup/rollup/pull/2835): Fix `removedExports` to correctly track the exported item ( @Swatinem)

## 1.11.0

_2019-05-03_

### Features

- Add `emitChunk` plugin context function to emit additional entry chunks that can be referenced from the code (#2809)
- Allow `manualChunks` to be a function (#2831)
- Omit `.js` extensions in AMD imports to make sure an AMD `baseUrl` would work (#2809)
- Automatically use the name of the imported module as a base for dynamically imported chunks (#2809)
- Add `resolveFileUrl` plugin hook to replace `resolveAssetUrl` and handle emitted chunks as well (#2809)
- Add `resolve` plugin hook to replace `resolveId` and `isExternal` that returns an object (#2829)
- Allow `resolveDynamicImport` to return an `{id, external}` object to also resolve unresolvable dynamic imports to a module (#2829)

### Bug Fixes

- Do not create invalid code if a dynamic import contains nothing but reexports (#2809)
- Do not fail if modules that define a manual chunk depend on each other (#2809)
- Do not fail if a module that defines a manual chunk is the dependency of a module defining a different manual chunk ( #2809)
- No longer fail for unnamed duplicate entry points but combine them (#2809)
- Always return `string | null` from `this.resolveId` even if some `resolveId` hooks return objects (#2829)
- Show proper warnings when `resolveDynamicImport` resolves to a non-external module that does not exist (#2829)

### Pull Requests

- [#2809](https://github.com/rollup/rollup/pull/2809): Add hook for dynamic entry chunk emission (@lukastaegert)
- [#2821](https://github.com/rollup/rollup/pull/2821): Fix syntax error in documentation (@FFxSquall)
- [#2829](https://github.com/rollup/rollup/pull/2829): Improve id resolution (@lukastaegert)
- [#2831](https://github.com/rollup/rollup/pull/2831): Allow manualChunks to be a function (@lukastaegert)
- [#2832](https://github.com/rollup/rollup/pull/2832): Improve `generateBundle` documentation (@lukastaegert)
- [#2833](https://github.com/rollup/rollup/pull/2833): Update dependencies (@lukastaegert)

## 1.10.1

_2019-04-19_

### Bug Fixes

- Invalid options.format values will now trigger a helpful error (#2813)

### Pull Requests

- [#2812](https://github.com/rollup/rollup/pull/2812): Minor documentation update (@dnalborczyk)
- [#2813](https://github.com/rollup/rollup/pull/2813): Catch invalid options.format values (@marijnh)
- [#2816](https://github.com/rollup/rollup/pull/2816): Update all dependencies to fix security issues (@lukastaegert)

## 1.10.0

_2019-04-11_

### Features

- Improve generated code to polyfill `import.meta.url` (#2785)
- Add plugin hook to configure handling of `import.meta` (#2785)
- Improve generated code when accessing URLs of emitted assets (#2796)
- Add plugin hook to configure the generated code when accessing URLs of emitted assets (#2796)

### Bug Fixes

- No longer resolve assets to their parent URL in some cases (#2796)

### Pull Requests

- [#2785](https://github.com/rollup/rollup/pull/2785): Refactor handling of import.meta.url and add option to configure behaviour (@lukastaegert)
- [#2796](https://github.com/rollup/rollup/pull/2796): Improve and fix asset emission (@lukastaegert)

## 1.9.3

_2019-04-10_

### Bug Fixes

- Simplify return expressions that are evaluated before the surrounding function is bound (#2803)

### Pull Requests

- [#2803](https://github.com/rollup/rollup/pull/2803): Handle out-of-order binding of identifiers to improve tree-shaking (@lukastaegert)

## 1.9.2

_2019-04-10_

### Bug Fixes

- Allowing replacing `output.file` with `output.dir` in the `outputOptions` hook (#2802)

### Pull Requests

- [#2802](https://github.com/rollup/rollup/pull/2802): Observe modified output options in bundle.write (@lukastaegert)

## 1.9.1

_2019-04-10_

### Bug Fixes

- Make sure inline comments in dynamic imports are preserved (#2797)

### Pull Requests

- [#2797](https://github.com/rollup/rollup/pull/2797): Emit inline comments inside dynamic import (@manucorporat)

## 1.9.0

_2019-04-05_

### Features

- Add built-in support for bigint (#2789)

### Pull Requests

- [#2789](https://github.com/rollup/rollup/pull/2789): Ship with bigint support built-in (@danielgindi)
- [#2791](https://github.com/rollup/rollup/pull/2791): Use shared extractAssignedNames from rollup-pluginutils ( @lukastaegert)
- [#2792](https://github.com/rollup/rollup/pull/2792): Test that rollup-plugin-commonjs works with preserveModules ( @lukastaegert)

## 1.8.0

_2019-04-02_

### Features

- Support `module` as alias for `esm` and `commonjs` for `cjs` to match Node (#2783)

### Pull Requests

- [#2782](https://github.com/rollup/rollup/pull/2782): Inline interopDefault in config loading (@guybedford)
- [#2783](https://github.com/rollup/rollup/pull/2783): Support Node-style format aliases (@guybedford)

## 1.7.4

_2019-03-28_

### Bug Fixes

- Improve TypeScript type of the treeshaking options (#2779)

### Pull Requests

- [#2779](https://github.com/rollup/rollup/pull/2779): Make all properties in TreeshakingOptions optional (@ndelangen)

## 1.7.3

_2019-03-24_

### Bug Fixes

- Use getters when re-exporting live-bindings (#2765)

### Pull Requests

- [#2765](https://github.com/rollup/rollup/pull/2765): Support exporting live-bindings from other chunks or external dependencies (@lukastaegert)

## 1.7.2

_2019-03-24_

### Bug Fixes

- Make sure relative external ids are resolved correctly (#2774)

### Pull Requests

- [#2774](https://github.com/rollup/rollup/pull/2774): Resolve relative external ids (@lukastaegert)

## 1.7.1

_2019-03-24_

### Bug Fixes

- Prevent invalid code when exporting several hundred identifiers from a chunk (#2768)
- Do not wrongly deconflict labels (#2776)

### Pull Requests

- [#2768](https://github.com/rollup/rollup/pull/2768): Sanitize shortened internal export names (@lukastaegert)
- [#2769](https://github.com/rollup/rollup/pull/2769): Update dependencies and fix security issue (@lukastaegert)
- [#2776](https://github.com/rollup/rollup/pull/2776): Do not treat break labels as identifiers (@lukastaegert)

## 1.7.0

_2019-03-20_

### Features

- Sort chunk exports by name for greater consistency (#2757)

### Bug Fixes

- Fix a situation where tree-shakeable code would not be removed in an indeterminate manner (#2757)

### Pull Requests

- [#2757](https://github.com/rollup/rollup/pull/2757): Sort modules before binding, sort exports (@lukastaegert)

## 1.6.1

_2019-03-20_

### Bug Fixes

- Avoid name clashes of unused default exports when tree-shaking is false (#2758)
- Do not crash when generating SystemJS bundles containing array patterns with member expressions (#2760)

### Pull Requests

- [#2758](https://github.com/rollup/rollup/pull/2758): Make sure unused default exports are deconflicted when tree-shaking is false (@lukastaegert)
- [#2760](https://github.com/rollup/rollup/pull/2760): Handle member expressions in array patterns (@lukastaegert)

## 1.6.0

_2019-03-08_

### Features

- Add plugin hook to modify output options (#2736)

### Pull Requests

- [#2736](https://github.com/rollup/rollup/pull/2736): Add hook for modifying OutputOptions (@Comandeer)

## 1.5.0

_2019-03-07_

### Features

- Allow resolving to a different id while marking it as external at the same time (#2734)

### Pull Requests

- [#2734](https://github.com/rollup/rollup/pull/2734): Allow resolveId to return an object (@lukastaegert)

## 1.4.2

_2019-03-07_

### Bug Fixes

- Respect variable identity of exports when hashing (#2741)
- Resolve a situations where a variable was imported twice with the same name (#2737)

### Pull Requests

- [#2741](https://github.com/rollup/rollup/pull/2741): Fix hashing when different variable are exported using the same name (@lukastaegert)
- [#2737](https://github.com/rollup/rollup/pull/2737): Fix duplicate imports with conflicting names (@lukastaegert)

## 1.4.1

_2019-03-04_

### Bug Fixes

- Do not treat the import target "" as external by default (#2733)

### Pull Requests

- [#2733](https://github.com/rollup/rollup/pull/2733): Do not treat the import target "" as external by default ( @LongTengDao)

## 1.4.0

_2019-03-01_

### Features

- Add option to change the name of the dynamic import function to allow polyfilling it (#2723)

### Pull Requests

- [#2723](https://github.com/rollup/rollup/pull/2723): Add dynamicImportFunction option (@keithamus)

## 1.3.3

_2019-03-01_

### Bug Fixes

- Fix performance regression when handling long chains of calls to property methods (#2732)

### Pull Requests

- [#2730](https://github.com/rollup/rollup/pull/2730): Order types, interfaces, classes, and object members ( @lukastaegert)
- [#2732](https://github.com/rollup/rollup/pull/2732): Take chunk export mode into account when reexporting default ( @lukastaegert)

## 1.3.2

_2019-02-27_

### Bug Fixes

- Allow ids of default exported classes to be exported separately (#2728)

### Pull Requests

- [#2728](https://github.com/rollup/rollup/pull/2728): Update dependencies (@lukastaegert)

## 1.3.1

_2019-02-27_

### Bug Fixes

- Correctly reexport the default export from entry chunks (#2727)

### Pull Requests

- [#2727](https://github.com/rollup/rollup/pull/2727): Take chunk export mode into account when reexporting default ( @lukastaegert)

## 1.3.0

_2019-02-26_

### Features

- Treeshake call expressions prefixed with UglifyJS style `@__PURE__` annotations (#2429)

### Pull Requests

- [#2429](https://github.com/rollup/rollup/pull/2429): Add support for /_#**PURE**_/ comments (@conartist6 and @lukastaegert)

## 1.2.5

_2019-02-26_

### Bug Fixes

- Store external ids reported by plugins in watch mode (#2718)

### Pull Requests

- [#2718](https://github.com/rollup/rollup/pull/2718): Incremental external (@andreas-karlsson)

## 1.2.4

_2019-02-26_

### Bug Fixes

- Fix an issue where a variable was imported twice under the same name (#2715)

### Pull Requests

- [#2715](https://github.com/rollup/rollup/pull/2715): Deduplicate imports referencing default exports and their original variables (@lukastaegert)

## 1.2.3

_2019-02-23_

### Bug Fixes

- Use correct path when rendering dynamic imports where the entry module is empty (#2714)

### Pull Requests

- [#2714](https://github.com/rollup/rollup/pull/2714): Properly render dynamic imports when imported module is empty ( @lukastaegert)

## 1.2.2

_2019-02-19_

### Bug Fixes

- Fix wrong external imports when using the `paths` options only for some outputs (#2706)

### Pull Requests

- [#2706](https://github.com/rollup/rollup/pull/2706): Always recreate paths for external modules (@lukastaegert)

## 1.2.1

_2019-02-17_

### Bug Fixes

- Fix ESM version of Rollup (#2705)

### Pull Requests

- [#2705](https://github.com/rollup/rollup/pull/2705): Fix ESM version of Rollup (@lukastaegert)

## 1.2.0

_2019-02-17_

### Features

- Fewer renamed variables due to a completely reimplemented deconflicting logic (#2689)

### Bug Fixes

- Respect rendered and tree-shaken exports when determining chunk hashes (#2695)
- Fix an error when dynamic imports end up in the same chunk as one of their importees (#2677)
- Do not generate invalid code when expressions containing IIFEs are simplified (#2696)
- Do not throw an error when more than ten bundles are watched (#2700)
- Treat re-exported globals in a spec-compliant way (#2691)
- Fix issues related to wrongly renamed variables (#2689)
- Do not throw an error if config files contain non-default exports (#2673)
- Improve type of `RollupOutput.output` to guarantee at least one chunk (#2679)

### Pull Requests

- [#2673](https://github.com/rollup/rollup/pull/2673): Allow config files to have non-default exports (@swansontec)
- [#2677](https://github.com/rollup/rollup/pull/2677): Prevent final resolution and facade creation for inlined dynamic imports (@Rich-Harris and @lukastaegert)
- [#2679](https://github.com/rollup/rollup/pull/2679): Improve type of `RollupOutput.output` (@MattiasBuelens)
- [#2689](https://github.com/rollup/rollup/pull/2689): Reimplement variable deconflicting logic (@lukastaegert)
- [#2691](https://github.com/rollup/rollup/pull/2691): Fix CI issues and update acorn dependency (@lukastaegert)
- [#2693](https://github.com/rollup/rollup/pull/2693): Fix typo in export-globals test (@MattiasBuelens)
- [#2695](https://github.com/rollup/rollup/pull/2695): Respect rendered exports when generating chunk hashes ( @lukastaegert)
- [#2696](https://github.com/rollup/rollup/pull/2696): Correctly render function expression inside simplified expression statements (@lukastaegert)
- [#2700](https://github.com/rollup/rollup/pull/2700): Add a fix for MaxListenersExceededWarning (@luwes)
- [#2703](https://github.com/rollup/rollup/pull/2703): Update rollup-pluginutils (@lukastaegert)

## 1.1.2

_2019-01-21_

### Bug Fixes

- Tree-shaken dynamic imports no longer leave behind `undefined` entries in the bundle information (#2663)
- Dynamic imports in dynamically imported files could lead to crashes and would not always create new chunks (#2664)

### Pull Requests

- [#2663](https://github.com/rollup/rollup/pull/2663): Do not include tree-shaken dynamic imports in bundle information (@lukastaegert)
- [#2664](https://github.com/rollup/rollup/pull/2664): Properly handle dynamic imports declared in dynamically imported files (@everdimension)

## 1.1.1

_2019-01-19_

### Bug Fixes

- Make sure object prototype methods are not considered to be falsy when tree-shaking (#2652)

### Pull Requests

- [#2652](https://github.com/rollup/rollup/pull/2652): Make sure object prototype methods are not considered to be falsy (@lukastaegert)
- [#2654](https://github.com/rollup/rollup/pull/2654): Use correct signature for `this.setAssetSource` in docs ( @everdimension)
- [#2656](https://github.com/rollup/rollup/pull/2656): Swap descriptions for `[extname]` and `[ext]` in docs (@tivac)

## 1.1.0

_2019-01-09_

### Features

- Make `this.meta` available from the `options` plugin hook (#2642)
- Add a new `writeBundle` plugin hook that is called _after_ all files have been written (#2643)

### Bug Fixes

- Make sure the `acorn` import of the bundled non-ESM acorn plugins is correctly translated to ESM (#2636)
- Make sure input options are actually passed to the `buildStart` hook (#2642)

### Pull Requests

- [#2636](https://github.com/rollup/rollup/pull/2636): Improve how acorn is imported, update dependencies ( @lukastaegert)
- [#2642](https://github.com/rollup/rollup/pull/2642): Make this.meta available in options hook, pass input options to buildStart (@lukastaegert)
- [#2643](https://github.com/rollup/rollup/pull/2643): Implement writeBundle hook (@lukastaegert)

## 1.0.2

_2019-01-05_

### Bug Fixes

- Make sure the transform hook is always reevaluated when a file watched by the hook changes (#2633)
- Fix a crash when generating hashes for tree-shaken dynamic imports (#2638)
- Fix a crash and some inconsistencies when using the acorn-bigint plugin (#2640)

### Pull Requests

- [#2633](https://github.com/rollup/rollup/pull/2633): Document `this.addWatchFile` and make sure it also declares transform dependencies (@lukastaegert)
- [#2635](https://github.com/rollup/rollup/pull/2635): Make sure `code` is optional in warning type (@lukastaegert)
- [#2638](https://github.com/rollup/rollup/pull/2638): Do not fail when generating hashes for tree-shaken dynamic imports (@lukastaegert)
- [#2640](https://github.com/rollup/rollup/pull/2640): Always treat bigints as unknown (@lukastaegert)
- [#2641](https://github.com/rollup/rollup/pull/2641): Make sure all CLI options are listed in the summary ( @lukastaegert)

## 1.0.1

_2019-01-03_

### Bug Fixes

- Properly handle reexporting an external default export for non-ESM targets when using named exports mode (#2620)
- Do not (wrongly) re-declare input options in the merged `RollupOptions` type (#2622)

### Pull Requests

- [#2620](https://github.com/rollup/rollup/pull/2620): Fixed issue with reexporting default as default with `{exports: named, interop: true}` options (@Andarist)
- [#2622](https://github.com/rollup/rollup/pull/2622): Simplify RollupOptions (@Kinrany)
- [#2627](https://github.com/rollup/rollup/pull/2627): Show how to skip imports for optional plugins (@chris-morgan)

## 1.0.0

_2018-12-28_

### Breaking Changes

- Several (mostly deprecated) options have been removed or renamed (#2293, #2409):
  - banner -> output.banner
  - dest -> output.file
  - entry -> input
  - experimentalCodeSplitting -> now always active
  - experimentalDynamicImport -> now always active
  - experimentalPreserveModules -> preserveModules
  - exports -> output.exports
  - extend -> output.extend
  - footer -> output.footer
  - format -> output.format
  - freeze -> output.freeze
  - globals -> output.globals
  - indent -> output.indent
  - interop -> output.interop
  - intro -> output.intro
  - load -> use plugin API
  - moduleName -> output.name
  - name -> output.name
  - noConflict -> output.noConflict
  - output.moduleId -> output.amd.id
  - outro -> output.outro
  - paths -> output.paths
  - preferConst -> output.preferConst
  - pureExternalModules -> treeshake.pureExternalModules
  - resolveExternal -> use plugin API
  - resolveId -> use plugin API
  - sourcemap -> output.sourcemap
  - sourceMap -> output.sourcemap
  - sourceMapFile -> output.sourcemapFile
  - strict -> output.strict
  - targets -> use output as an array
  - transform -> use plugin API
  - useStrict -> output.strict
- In general, output options can no longer be used as input options (#2409)
- `bundle.generate` and `bundle.write` now return a new format (#2293)
- Several plugin hooks have become deprecated and will display warnings when used (#2409):
  - transformBundle
  - transformChunk
  - ongenerate
  - onwrite
- Plugin transform dependencies are deprecated in favour of using the `this.addWatchFile` plugin context function ( #2409)
- Accessing `this.watcher` in plugin hooks is deprecated in favour of the `watchChange` plugin hook and the `this.addWatchFile` plugin context function (#2409)
- Using dynamic import statements will by default create a new chunk unless `inlineDynamicImports` is used (#2293)
- Rollup now uses acorn@6 which means that acorn plugins must be compatible with this version; acorn is now external for non-browser builds to make plugins work (#2293)

### Features

- The `--dir` ClI option can now be aliased as `-d` (#2293)
- The `--input` option now supports named entry points via `=` (#2293)

### Bug Fixes

- Both the `--input` option as well as the default CLI option now support named inputs (#2293)

### Pull Requests

- [#2293](https://github.com/rollup/rollup/pull/2293): Unify code paths for 1.0 relase and update documentation ( @guybedford and @lukastaegert)
- [#2409](https://github.com/rollup/rollup/pull/2409): Remove old deprecated features and add new deprecation warnings ( @guybedford)
- [#2486](https://github.com/rollup/rollup/pull/2486): Upgrade to acorn 6 (@marijnh)
- [#2611](https://github.com/rollup/rollup/pull/2611): Fix hook's name in test description (@Andarist)
- [#2612](https://github.com/rollup/rollup/pull/2612): Fix a self-contradicting comment in the docs (@LongTengDao)

## 0.68.2

_2018-12-23_

### Bug Fixes

- Do not assume hoisted variables to have been initialized (#2607)

### Pull Requests

- [#2607](https://github.com/rollup/rollup/pull/2607): Fix an issues where hoisted variables were assumed to have been initialized (@lye)

## 0.68.1

_2018-12-19_

### Bug Fixes

- Fix an issue with UMD wrappers where a variable is used without being defined (#2600)

### Pull Requests

- [#2600](https://github.com/rollup/rollup/pull/2600): Fix UMD and IIFE wrapper issues and add comprehensive functional wrapper tests (@lukastaegert)

## 0.68.0

_2018-12-16_

### Breaking Changes

- `optimizeChunks` is renamed to `experimentalOptimizeChunks` to reflect this feature is not production-ready yet ( #2575)

### Features

- Plugins can iterate all module ids via `this.moduleIds` (#2565)
- Plugins can get graph information about a module via `this.getModuleInfo(id)` (#2565)
- Plugins and JS API users get more information about the generated chunks: `dynamicImports`, `facadeModuleId`, `isDynamicEntry`, `name` (#2575)
- Tree-shaken dynamic imports will no longer create chunks or influence chunking in any way (#2575)
- Dynamic imports will no longer follow the `entryFileNames` but the `chunkFileNames` property reflecting those are solely internally used (#2575)
- If there are chunk naming conflicts, entry chunks will always take precedence (#2575)
- If an entry facade is created, only the facade chunk is marked as `isEntry` (#2575)
- Dynamic chunks will only be marked as `isEntry` if they are actually entry chunks as well; thus there is now a 1-to-1 correspondence between modules listed in `input` and chunks marked as `isEntry` (#2575)
- Chunks no longer contain imports for variables that are tree-shaken in the chunk but used in other chunks (#2584)
- Chunks will always import re-exported variables directly from the chunk where they are originally exported from ( #2584)
- Null characters will be pruned from chunk ids to allow for virtually created chunks and make `rollup-plugin-multi-entry` compatible with code-splitting and thus the upcoming 1.0 version (#2590)
- Simplify the UMD wrapper code as much as possible, especially if there are no exports (#2594)
- The UMD wrapper will now work in strict mode by checking for `self` before `this` when determining the global variable (#2594)

### Bug Fixes

- If a facade is created for a dynamic entry point, this facade will be imported instead of the facaded chunk (#2575)
- Manual chunks that include multiple entry points will have proper facades created for all entry points if necessary ( #2575)
- If missing exports are shimmed, the shim variable will not be global but created on a per-module basis and is deconflicted with variables having the same name (#2584)
- Missing export shims work properly in SystemJS (#2584)
- `preserveModules` now handles dynamic namespace imports (#2584)
- Fix chunk execution order in certain scenarios (#2584)
- Exports and assignments using destructuring syntax will properly update the exported variables when generating SystemJS output (#2587)
- Hashes in chunk names will now also take dynamic imports into account (#2596)

### Pull Requests

- [#2565](https://github.com/rollup/rollup/pull/2565): Provide module graph information on the plugin context ( @samccone)
- [#2575](https://github.com/rollup/rollup/pull/2575): Extend bundle information, tree-shake dynamic imports, fix dynamic import facade creation, support manual chunks with multiple entry points, make `optimizeChunks` experimental ( @lukastaegert)
- [#2577](https://github.com/rollup/rollup/pull/2577): Update dependencies (@lukastaegert)
- [#2584](https://github.com/rollup/rollup/pull/2584): Prune tree-shaken chunk imports, fix missing export shimming, support dynamic namespaces when preserving modules, improve chunk execution order (@lukastaegert)
- [#2587](https://github.com/rollup/rollup/pull/2587): Support exports using destructuring declarations and assignments in SystemJS (@lukastaegert)
- [#2590](https://github.com/rollup/rollup/pull/2590): Make sure chunk ids do not contain invalid characters to allow for chunks to correspond to virtual modules (@lukastaegert)
- [#2594](https://github.com/rollup/rollup/pull/2594): Simplify UMD wrapper code and make sure it works in strict mode ( @lukastaegert)
- [#2596](https://github.com/rollup/rollup/pull/2596): Take both static and dynamic dependencies into account when calculating hashes (@lukastaegert)

## 0.67.4

_2018-12-03_

### Bug Fixes

- Prevent corrupt source maps for files with very long lines (#2571)

### Pull Requests

- [#2571](https://github.com/rollup/rollup/pull/2571): Fix an issue with long lines in sourcemaps (@mislav)

## 0.67.3

_2018-11-17_

### Bug Fixes

- Make sure the ESM browser build is actually published to npm (#2560)
- Throw proper error when using `inlineDynamicImports` with `experimentalPreserveModules` (#2560)

### Pull Requests

- [#2552](https://github.com/rollup/rollup/pull/2552): Properly include ESM browser build in package (@lukastaegert)
- [#2560](https://github.com/rollup/rollup/pull/2560): Show proper error when using `inlineDynamicImports` with `experimentalPreserveModules` (@clarkdo)

## 0.67.2

_2018-11-17_

### Bug Fixes

- Prevent crash when not returning sourcemaps from `renderChunk` plugin hook (#2558)

### Pull Requests

- [#2558](https://github.com/rollup/rollup/pull/2558): Prevent crash when not returning sourcemaps from `renderChunk` ( @kyle1320)

## 0.67.1

_2018-11-11_

### Bug Fixes

- Deconflict CLI entry points with same name but on different paths if no explicit naming is used (#2548)

### Pull Requests

- [#2548](https://github.com/rollup/rollup/pull/2548): Deconflict CLI entry points with same name but on different paths if no explicit naming is used (@lukastaegert)

## 0.67.0

_2018-11-04_

### Breaking Changes

none

### Features

- Do not resolve external dynamic imports via plugins to match the logic for static external imports again (#2505)
- Support virtual modules created by plugins when preserving modules (#2511)
- Add new `output.sourcemapExcludeSources` option to exclude the actual sources from sourcemaps (#2531)

### Bug Fixes

- Fix TypeScript type for sourcemaps (#2507)
- Fix order of external and inter-chunk imports to match the proper execution order (#2508)
- Do not tree-shake children of unknown nodes to e.g. properly handle do-expressions via acorn plugin (#2510)
- Prevent memory leak when using the bundle as cache (#2522)
- Fix mis-placed semicolons for certain SystemJS exports (#2529)

### Pull Requests

- [#2505](https://github.com/rollup/rollup/pull/2505): Do not resolve external dynamic imports via plugins ( @lukastaegert)
- [#2507](https://github.com/rollup/rollup/pull/2507): Fix public sourcemap type (@aMarCruz)
- [#2508](https://github.com/rollup/rollup/pull/2508): Improve execution order of chunks and externals (@lukastaegert)
- [#2510](https://github.com/rollup/rollup/pull/2510): Do not tree-shake children of unknown nodes to e.g. properly handle do-expressions via acorn plugin (@devsnek)
- [#2511](https://github.com/rollup/rollup/pull/2511): Create chunks for virtual modules when preserving modules ( @lukastaegert)
- [#2522](https://github.com/rollup/rollup/pull/2522): Prevent memory leak when using the bundle as cache (@kyle1320)
- [#2529](https://github.com/rollup/rollup/pull/2529): Fix mis-placed semicolons for certain SystemJS exports ( @kyle1320)
- [#2531](https://github.com/rollup/rollup/pull/2531): add `sourcemapExcludeSources` option to exclude the source content from sourcemaps (@kitsonk)

## 0.66.6

_2018-10-10_

- Properly deconflict function and class declaration ids of reassigned default exports ([#2502](https://github.com/rollup/rollup/pull/2502))

## 0.66.5

_2018-10-09_

- Remove cache from memory once no longer needed ([#2496](https://github.com/rollup/rollup/pull/2496))
- Provide better error message when reexporting external namespace reexports ([#2499](https://github.com/rollup/rollup/pull/2499))

## 0.66.4

_2018-10-04_

- Fix links in warnings and errors ([#2471](https://github.com/rollup/rollup/pull/2471))

## 0.66.3

_2018-10-03_

- Detect side-effects in string.replace function arguments ([#2476](https://github.com/rollup/rollup/pull/2476))
- Make sure chunk ids are assigned before creating output bundle ([#2483](https://github.com/rollup/rollup/pull/2483))
- Use proper plugin name in error ([#2470](https://github.com/rollup/rollup/pull/2470))
- Update TypeScript version and fix type errors ([#2488](https://github.com/rollup/rollup/pull/2488))

## 0.66.2

_2018-09-21_

- Add additional information to parse errors messages in JSON and other non-JS files ([#2466](https://github.com/rollup/rollup/pull/2466))

## 0.66.1

_2018-09-19_

- Ignore falsy plugins ([#2464](https://github.com/rollup/rollup/pull/2464))
- Switch back to official TypeScript plugin ([#2465](https://github.com/rollup/rollup/pull/2465))

## 0.66.0

_2018-09-16_

- Support ES2019 optional catch bindings ([#2455](https://github.com/rollup/rollup/pull/2455))
- Add option to transform paths within sourcemaps ([#2430](https://github.com/rollup/rollup/pull/2430))
- Add renderStart and renderEnd plugin hooks ([#2438](https://github.com/rollup/rollup/pull/2438))
- Expose ESM browser build and minify browser builds ([#2437](https://github.com/rollup/rollup/pull/2437)
- Associate hoisted variables in function bodys with function parameters ([#2456](https://github.com/rollup/rollup/pull/2456))
- Fix issue when deconflicting variables used as pattern defaults ([#2446](https://github.com/rollup/rollup/pull/2446))
- Properly deconflict default exported class and function expressions with ids ([#2458](https://github.com/rollup/rollup/pull/2458))
- Faster internal test builds ([#2457](https://github.com/rollup/rollup/pull/2457))
- Switch to rollup-plugin-typescript2 ([#2460](https://github.com/rollup/rollup/pull/2460))
- Fix internal "perf" script ([#2433](https://github.com/rollup/rollup/pull/2433))
- Test that errors are passed to the buildEnd hook ([#2450](https://github.com/rollup/rollup/pull/2450))

## 0.65.2

_2018-09-05_

- Prevent watch mode memory leak ([#2441](https://github.com/rollup/rollup/pull/2441))

## 0.65.1

_2018-09-05_

- Prevent globbing when using chokidar ([#2432](https://github.com/rollup/rollup/pull/2432))

## 0.65.0

_2018-08-25_

- Refactor and unify plugin system ([#2382](https://github.com/rollup/rollup/pull/2382))
- Implement plugin cache API ([#2389](https://github.com/rollup/rollup/pull/2389))
- Add watchChange plugin hook to watch changed files, deprecate asset dependencies ([#2405](https://github.com/rollup/rollup/pull/2405))
- Refine asset handling ([#2369](https://github.com/rollup/rollup/pull/2369))
- Implement `renderChunk` hook to replace `transformChunk` and `transformBundle` hooks ([#2406](https://github.com/rollup/rollup/pull/2406))
- Add rollup version to plugin context ([#2394](https://github.com/rollup/rollup/pull/2394))
- Do not resume stdin in watch mode to fix it for Lerna users ([#2410](https://github.com/rollup/rollup/pull/2410))
- Allow `[format]` placeholder for id generation ([#2387](https://github.com/rollup/rollup/pull/2387))
- Always log error stacks even when a code frame is given ([#2417](https://github.com/rollup/rollup/pull/2417))
- Do not test module ids starting with `\0` as external ([#2400](https://github.com/rollup/rollup/pull/2400))
- Fix tracing of namespace variables ([#2408](https://github.com/rollup/rollup/pull/2408))
- Fix re-tracing of namespace variables ([#2420](https://github.com/rollup/rollup/pull/2420))
- Properly wrap comment annotations in SystemJS exports ([#2408](https://github.com/rollup/rollup/pull/2408))
- Fix renaming of destructured parameters ([#2419](https://github.com/rollup/rollup/pull/2419))
- Do not display version in watch mode when using `--silent` ([#2392](https://github.com/rollup/rollup/pull/2392))
- Make `cacheExpiry` an experimental option for now ([#2401](https://github.com/rollup/rollup/pull/2401))
- Lint test configs on commit ([#2402](https://github.com/rollup/rollup/pull/2402))
- Add code of conduct ([#2388](https://github.com/rollup/rollup/pull/2388))
- Move to CircleCI ([#2390](https://github.com/rollup/rollup/pull/2390))
- Update pull request template ([#2404](https://github.com/rollup/rollup/pull/2404))

## 0.64.1

_2018-08-07_

- Do not render initializers of hoisted variables in dead branches ([#2384](https://github.com/rollup/rollup/pull/2384))

## 0.64.0

_2018-08-07_

- Print memory consumption together with performance timings ([#2370](https://github.com/rollup/rollup/pull/2370))
- Enable plugins to mark imports as external by returning false for resolveId ([#2351](https://github.com/rollup/rollup/pull/2351))
- Always retain empty manual chunks ([#2362](https://github.com/rollup/rollup/pull/2362))
- Ensure CLI warnings are shown on errors and add error for external id collisions ([#2334](https://github.com/rollup/rollup/pull/2334))
- Remove unnecessary dependency, update dependencies, fix linting of test config ([#2376](https://github.com/rollup/rollup/pull/2376))
- Add targeted Github issue templates ([#2356](https://github.com/rollup/rollup/pull/2356))

## 0.63.5

_2018-08-01_

- Ensure onwrite plugin hooks execute in sequence ([#2364](https://github.com/rollup/rollup/pull/2364))
- Always warn when no name is provided for a global module ([#2359](https://github.com/rollup/rollup/pull/2359))
- Add utility type for user created plugins ([#2355](https://github.com/rollup/rollup/pull/2355))
- Remove deprecated es6 format from types ([#2349](https://github.com/rollup/rollup/pull/2349))
- Mark inlineDynamicImports as optional in types ([#2348](https://github.com/rollup/rollup/pull/2348))

## 0.63.4

_2018-07-20_

- Use turbocolor instead of chalk ([#2339](https://github.com/rollup/rollup/pull/2339))

## 0.63.3

_2018-07-20_

- Handle expressions where "in" and "instanceof" are applied to primitive values ([#2344](https://github.com/rollup/rollup/pull/2344))

## 0.63.2

_2018-07-18_

- Fix bind order in for-of loops ([#2338](https://github.com/rollup/rollup/pull/2338))

## 0.63.1

_2018-07-18_

## 0.63.0

_2018-07-17_

- Fix many tree-shaking related issues ([#2315](https://github.com/rollup/rollup/pull/2315))
- Add experimental support for top-level await ([#2235](https://github.com/rollup/rollup/pull/2235))
- Prevent duplicate version printout in watch mode ([#2325](https://github.com/rollup/rollup/pull/2325))
- Respect error frames provided by plugins ([#2309](https://github.com/rollup/rollup/pull/2309))
- Add `esm` format alias to types ([#2327](https://github.com/rollup/rollup/pull/2327))
- Further unify internal test setup ([#2329](https://github.com/rollup/rollup/pull/2329))

## 0.62.0

_2018-06-27_

- Add option to automatically shim missing exports ([#2118](https://github.com/rollup/rollup/pull/2118))
- Inline dynamic imports that are also imported statically and only used in a single chunk ([#2295](https://github.com/rollup/rollup/pull/2295))
- Handle caching and invalidation of assets ([#2267](https://github.com/rollup/rollup/pull/2267))
- Fix plugin related types ([#2299](https://github.com/rollup/rollup/pull/2299))

## 0.61.2

_2018-06-23_

- Improve watcher error handling, only rebuild invalidated outputs ([#2296](https://github.com/rollup/rollup/pull/2296))
- Update dependencies, make watcher more stable ([#2297](https://github.com/rollup/rollup/pull/2297))

## 0.61.1

_2018-06-21_

- Do not try to deconflict "undefined" ([#2291](https://github.com/rollup/rollup/pull/2291))
- Properly track values for loop interator declarations and reassigned namespaces, add smoke test ([#2292](https://github.com/rollup/rollup/pull/2292))

## 0.61.0

_2018-06-20_

- Declare file dependencies via transform plugin hooks ([#2259](https://github.com/rollup/rollup/pull/2259))
- Handle undefined values when evaluating conditionals ([#2264](https://github.com/rollup/rollup/pull/2264))
- Handle known undefined properties when evaluating conditionals ([#2265](https://github.com/rollup/rollup/pull/2265))
- Access watch events via the plugin context ([#2261](https://github.com/rollup/rollup/pull/2261))
- Add option to suppress `__esModule` flag in output ([#2287](https://github.com/rollup/rollup/pull/2287))
- Fix issue when re-declaring variables, track reassignments in more cases ([#2279](https://github.com/rollup/rollup/pull/2279))
- Add VSCode debug settings ([#2276](https://github.com/rollup/rollup/pull/2276))

## 0.60.7

_2018-06-14_

- Fix typing issue ([#2269](https://github.com/rollup/rollup/pull/2269))

## 0.60.6

_2018-06-14_

- Track mutations of included virtual arrays ([#2263](https://github.com/rollup/rollup/pull/2263))
- Update readme ([#2266](https://github.com/rollup/rollup/pull/2266))

## 0.60.5

_2018-06-14_

- Track deep reassignments of global and exported variables and improve performance ([#2254](https://github.com/rollup/rollup/pull/2254))

## 0.60.4

_2018-06-13_

- Properly handle initially uninitialized exports and exports of globals in SystemJS output ([#2258](https://github.com/rollup/rollup/pull/2258))

## 0.60.3

_2018-06-13_

- Fix types to allow watching an array of outputs ([#2262](https://github.com/rollup/rollup/pull/2262))

## 0.60.2

_2018-06-11_

- Permit setting an asset's source in `generateBundle` ([#2256](https://github.com/rollup/rollup/pull/2256))
- Add automatic linting ([#2242](https://github.com/rollup/rollup/pull/2242))

## 0.60.1

_2018-06-07_

- Fix plugin regressions ([#2246](https://github.com/rollup/rollup/pull/2246))
- Avoid conflicts for large numbers of variables ([#2244](https://github.com/rollup/rollup/pull/2244))

## 0.60.0

_2018-06-06_

- New plugin hooks: transformChunk, buildStart, buildEnd; extended plugin context with warn, error, resolveId, isExternal, emitAsset, setAssetSource and getAssetFileName available to any hook ([#2208](https://github.com/rollup/rollup/pull/2208))
- [BREAKING] Deprecate the `legacy` option and thus IE8 support ([#2141](https://github.com/rollup/rollup/pull/2141))
- Detect more known extensions and load .mjs without extension ([#2211](https://github.com/rollup/rollup/pull/2211))
- Add compact output mode ([#2151](https://github.com/rollup/rollup/pull/2151))
- Significantly improve sourcemap generation performance ([#2228](https://github.com/rollup/rollup/pull/2228))
- Enable naming SystemJS modules ([#2028](https://github.com/rollup/rollup/pull/2028))
- Do not use alternate screen if clearScreen is set in watch mode ([#2125](https://github.com/rollup/rollup/pull/2125))
- Allow object input form for code-splitting in watch mode ([#2217](https://github.com/rollup/rollup/pull/2217))
- Track reassignments of methods of exports from outside ([#2240](https://github.com/rollup/rollup/pull/2240))
- Preserve id of default exported functions and classes ([#2234](https://github.com/rollup/rollup/pull/2234))
- Add semicolons after default exports ([#2209](https://github.com/rollup/rollup/pull/2209))
- Fix build problems on Windows ([#2232](https://github.com/rollup/rollup/pull/2232))
- Display install size in readme ([#2196](https://github.com/rollup/rollup/pull/2196))
- Improve preserve modules test ([#2236](https://github.com/rollup/rollup/pull/2236))

## 0.59.4

_2018-05-28_

- Fix performance regression when many return statements are used ([#2218](https://github.com/rollup/rollup/pull/2218))

## 0.59.3

_2018-05-24_

- Fix reassignment tracking for constructor parameters ([#2214](https://github.com/rollup/rollup/pull/2214))

## 0.59.2

_2018-05-21_

- Fix reassignment tracking in for-in loops ([#2205](https://github.com/rollup/rollup/pull/2205))

## 0.59.1

_2018-05-16_

- Fix infinite recursion when determining literal values of circular structures ([#2193](https://github.com/rollup/rollup/pull/2193))
- Fix invalid code when simplifying expressions without spaces ([#2194](https://github.com/rollup/rollup/pull/2194))

## 0.59.0

_2018-05-15_

- Tree-shake statically analysable dynamic conditionals ([#2167](https://github.com/rollup/rollup/pull/2167))
- Do not emit empty chunks when code-splitting or empty files when preserving modules ([#2128](https://github.com/rollup/rollup/pull/2128))
- Support `import.meta.url` ([#2164](https://github.com/rollup/rollup/pull/2164))
- Add `esm` format alias ([#2102](https://github.com/rollup/rollup/pull/2102))
- Use alphanumeric base64 characters when deconflicting variables ([#2188](https://github.com/rollup/rollup/pull/2188))
- Improve handling of external modules imported as both default and named imports ([#2136](https://github.com/rollup/rollup/pull/2136))
- Properly deconflict named imports from other chunks ([#2177](https://github.com/rollup/rollup/pull/2177))
- Fix an issue with namespaces containing reexports ([#2157](https://github.com/rollup/rollup/pull/2157))
- Fix an issue with with incorrectly mapped default exports when code-splitting CJS or AMD modules ([#2178](https://github.com/rollup/rollup/pull/2178))
- Fix an issue with wrong paths of relative external imports ([#2160](https://github.com/rollup/rollup/pull/2160))
- Fix an issue when using default exports and `interop: false` ([#2149](https://github.com/rollup/rollup/pull/2149))
- Fix in issue with invalid syntax in SystemJS output ([#2187](https://github.com/rollup/rollup/pull/2187))
- Fix an issue when tree-shaking call expressions and reassigned variables ([#2186](https://github.com/rollup/rollup/pull/2186))
- Fix file paths in source maps ([#2161](https://github.com/rollup/rollup/pull/2161))
- Fix wrong file name in error message ([#2137](https://github.com/rollup/rollup/pull/2137))
- Always use npm 5 on CI ([#2185](https://github.com/rollup/rollup/pull/2185))

## 0.58.2

_2018-04-23_

- Fix rendering of certain statically resolvable if statements ([#2146](https://github.com/rollup/rollup/pull/2146))

## 0.58.1

_2018-04-18_

- Fix comment detection ([#2129](https://github.com/rollup/rollup/pull/2129))

## 0.58.0

_2018-04-16_

- Support individual chunk names with optional content hashes ([#2068](https://github.com/rollup/rollup/pull/2068))
- Support manually created chunks ([#2084](https://github.com/rollup/rollup/pull/2084))
- Automatically import deep dependencies when code splitting for better performance ([#2073](https://github.com/rollup/rollup/pull/2073))
- Automatically minify internal export/import names for esm and system output ([#2087](https://github.com/rollup/rollup/pull/2087))
- Add option to automatically merge small chunks ([#2090](https://github.com/rollup/rollup/pull/2090))
- Significantly improve tree-shaking performance ([#2119](https://github.com/rollup/rollup/pull/2119))
- Enable tree-shaking for logical expressions ([#2098](https://github.com/rollup/rollup/pull/2098))
- Rework external types and reduce type related dependencies ([#2108](https://github.com/rollup/rollup/pull/2108))
- Support parallel dependency resolution ([#2116](https://github.com/rollup/rollup/pull/2116))
- Improve deprecation handling ([#2076](https://github.com/rollup/rollup/pull/2076))
- Enable `--perf` timings in watch mode ([#2065](https://github.com/rollup/rollup/pull/2065))
- Improve performance timers ([#2111](https://github.com/rollup/rollup/pull/2111))
- Improve error handling for plugins ([#2100](https://github.com/rollup/rollup/pull/2100))
- Improve error when using `--dir` in a single file build ([#2123](https://github.com/rollup/rollup/pull/2123))
- Do not warn for external imports that are unused due to tree-shaking ([#2124](https://github.com/rollup/rollup/pull/2124))
- Update mixed export warning message ([#2107](https://github.com/rollup/rollup/pull/2107))
- Remove duplicate badges from readme ([#2083](https://github.com/rollup/rollup/pull/2083))
- Update readme examples ([#2086](https://github.com/rollup/rollup/pull/2086))

## 0.57.1

_2018-03-17_

- Improve sourcemap generation performance ([#2062](https://github.com/rollup/rollup/pull/2062))
- Add reserved config option namespace and improve CLI interface ([#2063](https://github.com/rollup/rollup/pull/2063))
- Fix issue with default exported function and class expressions ([#2059](https://github.com/rollup/rollup/pull/2059))
- Replace `forEach` with faster `for` loops in some places ([#2064](https://github.com/rollup/rollup/pull/2064))

## 0.57.0

_2018-03-15_

- Add option to preserve the module structure instead of bundling ([#1922](https://github.com/rollup/rollup/pull/1922))
- Enable watch mode when code-splitting ([#2035](https://github.com/rollup/rollup/pull/2035))
- Optionally pass CLI commands to config file ([#1926](https://github.com/rollup/rollup/pull/1926))
- Option to add correct `.toString` tags to namespaces ([#2041](https://github.com/rollup/rollup/pull/2041))
- Option and scripts to display performance timings ([#2045](https://github.com/rollup/rollup/pull/2045))
- Fixes for exported or early accessed namespaces + improved namespace indentation ([#2041](https://github.com/rollup/rollup/pull/2041))
- Include missing TypeScript dependencies ([#1965](https://github.com/rollup/rollup/pull/1965))
- Add #\_PURE annotation to frozen namespaces ([#2044](https://github.com/rollup/rollup/pull/2044))
- Improve sourcemap and tree-shaking performance ([#2052](https://github.com/rollup/rollup/pull/2052))
- Inline sourcemap lookups and make rollup smaller ([#2055](https://github.com/rollup/rollup/pull/2055))
- Use updated magic-string types ([#2057](https://github.com/rollup/rollup/pull/2057))
- [BREAKING] Revert class id preservation from #2025 ([#2048](https://github.com/rollup/rollup/pull/2048))
- [BREAKING] Refactor missing export plugin hook ([#1987](https://github.com/rollup/rollup/pull/1987))

## 0.56.5

_2018-03-07_

- Preserve ids when deconflicting classes ([#2025](https://github.com/rollup/rollup/pull/2025))
- Fix an issue with re-exported namespace imports ([#2034](https://github.com/rollup/rollup/pull/2034))
- Prevent an infinite loop when binding member expressions ([#1963](https://github.com/rollup/rollup/pull/1963))
- Convert code style via prettier ([#2031](https://github.com/rollup/rollup/pull/2031))
- Fix links in documentation ([#2026](https://github.com/rollup/rollup/pull/2026))

## 0.56.4

_2018-03-05_

- Make rollup builds reproducible ([#2024](https://github.com/rollup/rollup/pull/2024))
- Improve error handling for source maps ([#2012](https://github.com/rollup/rollup/pull/2012))
- Properly handle SystemJS default exports without semicolons ([#2019](https://github.com/rollup/rollup/pull/2019))
- Properly handle importing the same variable several times when code-splitting ([#2020](https://github.com/rollup/rollup/pull/2020))
- Improve re-export tracing ([#2021](https://github.com/rollup/rollup/pull/2021))
- Apply "prettier" on commit ([#2017](https://github.com/rollup/rollup/pull/2017))
- Automatically clean up outdated tests ([#2009](https://github.com/rollup/rollup/pull/2009))
- Add SystemJS output to form tests ([#2022](https://github.com/rollup/rollup/pull/2022))
- Improve internal build configuration ([#2016](https://github.com/rollup/rollup/pull/2016))

## 0.56.3

_2018-02-25_

- Fix issues around default exports and module facades ([#2001](https://github.com/rollup/rollup/pull/2001))
- Improve and fix internal chunk interface ([#1994](https://github.com/rollup/rollup/pull/1994))
- Fix superfluous semicolons added after declarations ([#1999](https://github.com/rollup/rollup/pull/1999))
- Improve code-splitting tests ([#1990](https://github.com/rollup/rollup/pull/1990))

## 0.56.2

_2018-02-19_

- Fix handling of reassigned default exports ([#1975](https://github.com/rollup/rollup/pull/1975))
- Fix handling of renamed exports in entry points ([#1977](https://github.com/rollup/rollup/pull/1977))
- Update internal TypeScript version ([#1980](https://github.com/rollup/rollup/pull/1980))
- Omit compiled source files from published types ([#1981](https://github.com/rollup/rollup/pull/1981))
- Fix example in readme file ([#1984](https://github.com/rollup/rollup/pull/1984))
- Fix non-replaced dynamic imports in non-ESM output ([#1985](https://github.com/rollup/rollup/pull/1985))

## 0.56.1

_2018-02-16_

- Fix regression when rendering switch statements ([#1971](https://github.com/rollup/rollup/pull/1971))

## 0.56.0

_2018-02-15_

- Update to ECMAScript 2018 ([#1953](https://github.com/rollup/rollup/pull/1953))
- Rework tree-shaking rendering algorithm ([#1949](https://github.com/rollup/rollup/pull/1949))
- Tree-shake pure prototype calls on literals ([#1916](https://github.com/rollup/rollup/pull/1916))
- Expose AST parser to plugins ([#1945](https://github.com/rollup/rollup/pull/1945))
- Fix namespace re-export deconflicting ([#1960](https://github.com/rollup/rollup/pull/1960))
- Allow globals to be re-exported ([#1959](https://github.com/rollup/rollup/pull/1959))
- Fix internal performance timers ([#1966](https://github.com/rollup/rollup/pull/1966))

## 0.55.5

_2018-02-10_

- Remove OpenCollective dependency ([#1915](https://github.com/rollup/rollup/pull/1915))

## 0.55.4

_2018-02-09_

- Improve name deconflicting of external variables ([#1930](https://github.com/rollup/rollup/pull/1930))
- Improve re-export handling ([#1947](https://github.com/rollup/rollup/pull/1947))
- Mark preserveSymlinks option as optional ([#1939](https://github.com/rollup/rollup/pull/1939))
- Enable code-splitting tests to check directory structures ([#1924](https://github.com/rollup/rollup/pull/1924))
- Improve TypeScript definition test ([#1954](https://github.com/rollup/rollup/pull/1954))

## 0.55.3

_2018-02-01_

- Remove OpenCollective dependency ([#1915](https://github.com/rollup/rollup/pull/1915))

## 0.55.2

_2018-02-01_

- Add option to not follow symlinks ([#1819](https://github.com/rollup/rollup/pull/1819))
- Fix crash in windows shell ([#1928](https://github.com/rollup/rollup/pull/1928))
- Fix and test for external TypeScript errors ([#1903](https://github.com/rollup/rollup/pull/1903))
- Activate OpenCollective ([#1915](https://github.com/rollup/rollup/pull/1915))
- Optimize CI scripts ([#1921](https://github.com/rollup/rollup/pull/1921))

## 0.55.1

_2018-01-26_

- Improve dynamic import workflow ([#1907](https://github.com/rollup/rollup/pull/1907))
- Properly handle multiple dynamic imports of the same module ([#1911](https://github.com/rollup/rollup/pull/1911))
- Fix import specifier deshadowing ([#1912](https://github.com/rollup/rollup/pull/1912))
- Allow plugin load hook to return an empty string ([#1908](https://github.com/rollup/rollup/pull/1908))
- Let onwarn handler accept strings ([#1905](https://github.com/rollup/rollup/pull/1905))

## 0.55.0

_2018-01-23_

- Support code splitting ([#1841](https://github.com/rollup/rollup/pull/1841))
- Support SystemJS as output format ([#1897](https://github.com/rollup/rollup/pull/1897))
- Allow injecting acorn plugins ([#1857](https://github.com/rollup/rollup/pull/1857))
- Add `missingExport` plugin hook ([#1845](https://github.com/rollup/rollup/pull/1845))
- No longer parse config files via bublé ([#1899](https://github.com/rollup/rollup/pull/1899))
- Use externally maintained dynamic import acorn plugin ([#1891](https://github.com/rollup/rollup/pull/1891))
- Fix an error message ([#1886](https://github.com/rollup/rollup/pull/1886))
- Refactor internal rendering options ([#1900](https://github.com/rollup/rollup/pull/1900))
- Extract internal path resolution ([#1879](https://github.com/rollup/rollup/pull/1879))
- Extract internal bundle option handling ([#1880](https://github.com/rollup/rollup/pull/1880))
- Add import description type ([#1884](https://github.com/rollup/rollup/pull/1884))
- Clean up watch options types ([#1860](https://github.com/rollup/rollup/pull/1860))
- Clean up some tests ([#1888](https://github.com/rollup/rollup/pull/1888))

## 0.54.1

_2018-01-17_

- Fix TypeScript errors in emitted type definitions ([#1871](https://github.com/rollup/rollup/pull/1871))

## 0.54.0

_2018-01-12_

- Automatically inline locally resolvable dynamic imports ([#1816](https://github.com/rollup/rollup/pull/1816))
- Preserve directives in function bodies ([#1856](https://github.com/rollup/rollup/pull/1856))
- Refactor an error notification ([#1846](https://github.com/rollup/rollup/pull/1846))
- Refactor a wrong import ([#1863](https://github.com/rollup/rollup/pull/1863))
- Improve emitted TypeScript definitions ([#1864](https://github.com/rollup/rollup/pull/1864))
- Refactor unused import ([#1866](https://github.com/rollup/rollup/pull/1866))

## 0.53.4

_2018-01-10_

- More type cleanup ([#1858](https://github.com/rollup/rollup/pull/1858))
- Use chalks internal helper to detect if colors should be used ([#1853](https://github.com/rollup/rollup/pull/1853))
- Refactor entity handling to use interfaces ([#1840](https://github.com/rollup/rollup/pull/1840))
- Use immutable.js internal types ([#1844](https://github.com/rollup/rollup/pull/1844))
- Ship `TypeScript` declaration files ([#1837](https://github.com/rollup/rollup/pull/1837))

## 0.53.3

_2018-01-02_

- Use correct name when re-exporting from external modules ([#1794](https://github.com/rollup/rollup/pull/1794))
- Disable warnings when `resolveId` returns false ([#1825](https://github.com/rollup/rollup/pull/1825))

## 0.53.2

_2017-12-30_

- Properly handle output arrays in the JavaScript API ([#1827](https://github.com/rollup/rollup/pull/1827))

## 0.53.1

_2017-12-28_

- Properly deprecate more config options ([#1812](https://github.com/rollup/rollup/pull/1812))
- Pass output options to `transformBundle` plugin hook ([#1813](https://github.com/rollup/rollup/pull/1813))

## 0.53.0

_2017-12-22_

- Experimental dynamic import support ([#1790](https://github.com/rollup/rollup/pull/1790))
- Unify config validation ([#1805](https://github.com/rollup/rollup/pull/1805))

## 0.52.3

_2017-12-19_

- Properly hoist default exported functions in more situations ([#1799](https://github.com/rollup/rollup/pull/1799))
- Allow plugin transformations to not overwrite source maps by returning null ([#1797](https://github.com/rollup/rollup/pull/1797))
- Provide more parameters to "external" handler ([#1792](https://github.com/rollup/rollup/pull/1792))

## 0.52.2

_2017-12-15_

- No longer ignore side-effects in JSON.parse and JSON.stringify ([#1785](https://github.com/rollup/rollup/pull/1785))
- Updated links in warnings ([#1776](https://github.com/rollup/rollup/pull/1776))
- No longer prevent self-imports ([#1777](https://github.com/rollup/rollup/pull/1777))
- Properly hoist default exported functions ([#1787](https://github.com/rollup/rollup/pull/1787))
- Prevent corruption when re-exporting default exports ([#1765](https://github.com/rollup/rollup/pull/1765))

## 0.52.1

_2017-12-05_

- Improve deprecation warnings ([#1765](https://github.com/rollup/rollup/pull/1765))
- Properly use stdin ([#1774](https://github.com/rollup/rollup/pull/1774))
- Let --environment be used multiple times ([#1768](https://github.com/rollup/rollup/pull/1768))
- Always transpile config files ([#1759](https://github.com/rollup/rollup/pull/1759))
- Respect globals option in headers of UMD and IIFE files ([#1747](https://github.com/rollup/rollup/pull/1747))

## 0.52.0

_2017-11-25_

- Accept config as promise ([#1731](https://github.com/rollup/rollup/pull/1731))
- Accept promises for intro/outro/banner/footer ([#1253](https://github.com/rollup/rollup/pull/1253))
- Option to prevent freezing of namespace imports ([#1696](https://github.com/rollup/rollup/pull/1696))
- Option to retain all output in watch mode ([#1688](https://github.com/rollup/rollup/pull/1688))
- Options to fine-tune treeshaking ([#1760](https://github.com/rollup/rollup/pull/1760))

## 0.51.8

_2017-11-19_

- Fix speed problems by simplifying treeshaking reassignment handling ([#1740](https://github.com/rollup/rollup/pull/1740))
- Update dependencies ([#1742](https://github.com/rollup/rollup/pull/1742))

## 0.51.7

_2017-11-17_

- Keep "this"-context when calling sequence expressions ([#1724](https://github.com/rollup/rollup/pull/1724))

## 0.51.6

_2017-11-16_

- Use sourcemaps to determine error locations ([#1728](https://github.com/rollup/rollup/pull/1728))

## 0.51.5

_2017-11-11_

- Fix regressions with uninitialised conditional expressions ([#1720](https://github.com/rollup/rollup/pull/1720))

## 0.51.4

_2017-11-11_

- Fix regressions preventing builds ([#1725](https://github.com/rollup/rollup/pull/1725))

## 0.51.3

_2017-11-10_

- Fix regression when treeshaking sequence expressions ([#1717](https://github.com/rollup/rollup/pull/1717))

## 0.51.2

_2017-11-09_

- Fix treeshaking regression when labels are used inside functions ([#1712](https://github.com/rollup/rollup/pull/1712))

## 0.51.1

_2017-11-08_

- Fix an issue with empty return statements ([#1704](https://github.com/rollup/rollup/pull/1704))

## 0.51.0

_2017-11-08_

- Massive improvements to the treeshaking algorithm ([#1667](https://github.com/rollup/rollup/pull/1667))

## 0.50.1

_2017-11-08_

- Fix treeshaking regression ([#1695](https://github.com/rollup/rollup/pull/1695))
- Treeshaking improvements ([#1650](https://github.com/rollup/rollup/pull/1650))
- Enable installation from Github ([#1670](https://github.com/rollup/rollup/pull/1670))
- Update documentation ([#1660](https://github.com/rollup/rollup/pull/1660))

## 0.50.0

_2017-09-16_

- Many treeshaking improvements ([#1624](https://github.com/rollup/rollup/pull/1624))
- Show finish time in watch mode ([#1620](https://github.com/rollup/rollup/pull/1620))

## 0.49.3

_2017-09-08_

- Respect `watch` options ([#1596](https://github.com/rollup/rollup/issues/1596))
- Fix treeshaking regressions ([#1604](https://github.com/rollup/rollup/pull/1604))
- Allow `-o` to work with `output.format` ([#1606](https://github.com/rollup/rollup/pull/1606))

## 0.49.2

_2017-08-29_

- Fix treeshaking regressions ([#1591](https://github.com/rollup/rollup/pull/1591))

## 0.49.1

_2017-08-28_

- Fix treeshaking regressions ([#1586](https://github.com/rollup/rollup/pull/1586))

## 0.49.0

_2017-08-27_

- Completely update the treeshaking algorithm ([#1582](https://github.com/rollup/rollup/pull/1582))
- Only flip screen buffer if appropriate ([#1574](https://github.com/rollup/rollup/pull/1574))
- Guard against two instances creating the same dir ([#1576](https://github.com/rollup/rollup/pull/1576))

## 0.48.2

- Paths is an output option ([#1569](https://github.com/rollup/rollup/pull/1569))

## 0.48.1

- Print deprecation warnings in watch mode, and fix options when watcher restarts ([#1568](https://github.com/rollup/rollup/pull/1568))

## 0.48.0

- Numerous changes to the `options` object and CLI arguments ([#1479](https://github.com/rollup/rollup/issues/1479)). See [this gist](https://gist.github.com/Rich-Harris/d472c50732dab03efeb37472b08a3f32) for a rundown.

## 0.47.6

- Set `process.env.ROLLUP_WATCH` _before_ loading config file

## 0.47.5

- Fix broken multi-bundle configs with `rollup.watch` ([#1532](https://github.com/rollup/rollup/issues/1532))

## 0.47.4

- Delete cached config file before reloading in watch mode

## 0.47.3

- Deshadow aliased imports ([#1550](https://github.com/rollup/rollup/issues/1550))

## 0.47.2

- Rebuild with dependency that npm randomly deleted

## 0.47.1

- Ignore external namespace imports when deshadowing ([#1547](https://github.com/rollup/rollup/issues/1547))

## 0.47.0

- Watch config file, restart `rollup.watch` on change ([#1535](https://github.com/rollup/rollup/issues/1535))
- Correctly render `export { foo } from` declarations in `es` output ([#1543](https://github.com/rollup/rollup/pull/1543))
- Reinstate missing `rollup.VERSION`

## 0.46.3

- init for/for-of loop section head with correct scopes ([#1538](https://github.com/rollup/rollup/issues/1538), [#1539](https://github.com/rollup/rollup/issues/1539))
- Fix namespace imports and re-exports in `es` output ([#1511](https://github.com/rollup/rollup/issues/1511))
- Deshadow indirectly imported namespaces ([#1488](https://github.com/rollup/rollup/issues/1488), [#1505](https://github.com/rollup/rollup/issues/1505))

## 0.46.2

- Pass options to `bundle.write` correctly in `rollup.watch` ([#1533](https://github.com/rollup/rollup/issues/1533))
- init for-in loop section head with correct scopes ([#1480](https://github.com/rollup/rollup/issues/1480))
- support `--no-interop` flag ([#1524](https://github.com/rollup/rollup/issues/1524))

## 0.46.1

- Remove `rollup.watch` from browser build ([#1530](https://github.com/rollup/rollup/issues/1530))
- Remove `source-map-support` dependency ([#1528](https://github.com/rollup/rollup/issues/1528))

## 0.46.0

- `options.format` is now required ([#1491](https://github.com/rollup/rollup/pull/1491))
- if `options.format` is `es6`, it will now throw an error (should be `es`) ([#1491](https://github.com/rollup/rollup/pull/1491))
- Add experimental `rollup.watch` method, replacing [rollup-watch](https://github.com/rollup/rollup-watch) ([#1491](https://github.com/rollup/rollup/pull/1491))
- Batch warnings together in CLI output ([#1491](https://github.com/rollup/rollup/pull/1491))
- Clear screen between rebuilds in `--watch` mode ([#1491](https://github.com/rollup/rollup/pull/1491))
- `onwarn` function's second argument is the default handler, allowing easier filtering without reimplementing any logic ([#1491](https://github.com/rollup/rollup/pull/1491))
- Prevent semi-colon removal after variable declaration that is for loop body ([#1275](https://github.com/rollup/rollup/issues/1275))
- Return `exports` for namespaced but non-extended IIFE bundles ([#1492](https://github.com/rollup/rollup/issues/1492))
- Fix scoping in switch statements ([#1498](https://github.com/rollup/rollup/pull/1498))
- Handle side-effects in tagged template expressions ([#1508](https://github.com/rollup/rollup/pull/1508))
- More descriptive error for missing options.format ([#1510](https://github.com/rollup/rollup/pull/1510))
- Refactor scope handling ([#1517](https://github.com/rollup/rollup/pull/1517))
- Handle failure of a config in multi-config build ([#1513](https://github.com/rollup/rollup/issues/1513))

## 0.45.2

- Fix interop when import is a string ([#1486](https://github.com/rollup/rollup/issues/1486))
- Separate `resolvedIds` from `resolvedExternalIds` ([#1490](https://github.com/rollup/rollup/pull/1490))
- Add `--extend` flag to CLI ([#1482](https://github.com/rollup/rollup/pull/1482))

## 0.45.1

- Remove `weak` from `optionalDependencies` ([#1483](https://github.com/rollup/rollup/issues/1483))

## 0.45.0

- [BREAKING] `bundle.generate(...)` returns a Promise, so that `transformBundle` plugin hooks can be asynchronous ([#1474](https://github.com/rollup/rollup/issues/1474))

## 0.44.0

- [BREAKING] Don't extend existing globals, unless `options.extend` is true ([#827](https://github.com/rollup/rollup/issues/827))
- Fix handling of catch clause parameters ([#1462](https://github.com/rollup/rollup/issues/1462))

## 0.43.1

- Fix memory leak on incremental rebuilds ([#883](https://github.com/rollup/rollup/issues/883))
- Allow `this.warn` and `this.error` to accept a `{line, column}` object as an alternative to a character index ([#1265](https://github.com/rollup/rollup/issues/1265))
- Print more useful error if entry module is 'external' ([#1264](https://github.com/rollup/rollup/issues/1264))
- Catch errors in `bundle.generate` options ([#1463](https://github.com/rollup/rollup/pull/1463))
- Fix magic-string deprecation warning ([#1445](https://github.com/rollup/rollup/pull/1445))

## 0.43.0

- Allow config files to import JSON ([#1426](https://github.com/rollup/rollup/issues/1426))
- Allow undefined imports in interop block ([#1341](https://github.com/rollup/rollup/issues/1341))
- Add `process.env.ROLLUP_WATCH = 'true'` in watch mode ([#1429](https://github.com/rollup/rollup/issues/1429))
- Add `pureExternalModules` option ([#1352](https://github.com/rollup/rollup/issues/1352))
- Allow plugins to specify `options.entry` ([#1270](https://github.com/rollup/rollup/issues/1270))
- Update dependencies

## 0.42.0

- Deprecate `options.moduleId` in favour of `options.amd.id` ([#1365](https://github.com/rollup/rollup/pull/1365))
- Add `options.amd.define` option to specify name of AMD `define` function ([#1365](https://github.com/rollup/rollup/pull/1365))
- Fix incorrect class removal with `treeshake: false` ([#1375](https://github.com/rollup/rollup/pull/1375))
- Deconflict module exports imported as namespaces ([#1384](https://github.com/rollup/rollup/issues/1384))
- Handle bare self-imports ([#1274](https://github.com/rollup/rollup/issues/1274))
- Allow config file to export an array of multiple configs ([#1389](https://github.com/rollup/rollup/pull/1389))
- Handle exponentiation operator, and fail gracefully on unknown operators ([#1416](https://github.com/rollup/rollup/issues/1416))
- Add `watch` option ([#1424](https://github.com/rollup/rollup/pull/1424))

## 0.41.6

- Preserve `originalSourceMap` on incremental rebuilds for loaders with sourcemaps ([#1336](https://github.com/rollup/rollup/issues/1336))

## 0.41.5

- Wrap ternary consequent/alternate sequences in parens ([#1273](https://github.com/rollup/rollup/issues/1273))
- Fix erroneous warning on multiple `export * from` declarations with defaults ([#1278](https://github.com/rollup/rollup/issues/1278))
- Prevent variable conflicts with `treeshake: false` ([#1268](https://github.com/rollup/rollup/issues/1268))
- Allow missing `source` when collapsing sourcemaps ([#1254](https://github.com/rollup/rollup/issues/1254))
- Allow plugins to log with strings ([#1316](https://github.com/rollup/rollup/pull/1316))

## 0.41.4

- Fix cases of multiple `export * from 'external'` declarations ([#1252](https://github.com/rollup/rollup/issues/1252))
- Fix 'TODO' error message ([#1257](https://github.com/rollup/rollup/issues/1257))

## 0.41.3

- Don't treat `this.foo` as possible namespace ([#1258](https://github.com/rollup/rollup/issues/1258))

## 0.41.2

- Optimize `namespace['foo']` references ([#1240](https://github.com/rollup/rollup/pull/1240))

## 0.41.1

- Include `new` expressions where callee is a class with side-effects ([#980](https://github.com/rollup/rollup/issues/980) [#1233](https://github.com/rollup/rollup/issues/1233))

## 0.41.0

- Add `this.warn(...)` and `this.error(...)` methods to plugin `transform` hook contexts ([#1140](https://github.com/rollup/rollup/issues/1140))
- `throw` always considered to be a side effect ([#1227](https://github.com/rollup/rollup/pull/1227))

## 0.40.2

- Add `file` property to sourcemaps for bundles with plugins ([#986](https://github.com/rollup/rollup/issues/986))
- Don't require globals for empty imports ([#1217](https://github.com/rollup/rollup/issues/1217))

## 0.40.1

- Allow missing space between `export default` and declaration ([#1218](https://github.com/rollup/rollup/pull/1218))

## 0.40.0

- [BREAKING] Better, more consistent error logging ([#1212](https://github.com/rollup/rollup/pull/1212))
- Don't use colours and emojis for non-TTY stderr ([#1201](https://github.com/rollup/rollup/issues/1201))

## 0.39.2

- Prevent mutation of cached ASTs (fixes stack overflow with rollup-watch) ([#1205](https://github.com/rollup/rollup/pull/1205))

## 0.39.1

- Ignore `var` initialisers in dead branches ([#1198](https://github.com/rollup/rollup/issues/1198))

## 0.39.0

- [BREAKING] Warnings are objects, rather than strings ([#1194](https://github.com/rollup/rollup/issues/1194))

## 0.38.3

- More informative warning for implicit external dependencies ([#1051](https://github.com/rollup/rollup/issues/1051))
- Warn when creating browser bundle with external dependencies on Node built-ins ([#1051](https://github.com/rollup/rollup/issues/1051))
- Statically analyse LogicalExpression nodes, for better dead code removal ([#1061](https://github.com/rollup/rollup/issues/1061))

## 0.38.2

- Preserve `var` declarations in dead branches ([#997](https://github.com/rollup/rollup/issues/997))
- Warn if exporting a call expression that looks like a function declaration ([#1011](https://github.com/rollup/rollup/issues/1011))
- Wrap function expressions in parentheses if necessary ([#1011](https://github.com/rollup/rollup/issues/1011))

## 0.38.1

- Fix sourcemap comment removal ([#1104](https://github.com/rollup/rollup/issues/1104))
- Warn if empty bundle is generated ([#444](https://github.com/rollup/rollup/issues/444))
- Support ES2017 syntax ([#492](https://github.com/rollup/rollup/issues/492))
- Remove unused imports from external modules ([#595](https://github.com/rollup/rollup/issues/595))
- Remove unused function and class declarations inside function bodies ([#1108](https://github.com/rollup/rollup/issues/1108), [#1178](https://github.com/rollup/rollup/issues/1178))
- Deconflict function expression IDs ([#1176](https://github.com/rollup/rollup/issues/1176))

## 0.38.0

- [BREAKING] `export { foo as default }` creates live binding ([#1078](https://github.com/rollup/rollup/issues/1078))
- Prevent sourceMappingURL removal edge case ([#988](https://github.com/rollup/rollup/issues/988))
- Bind function expression IDs to the correct scope ([#1083](https://github.com/rollup/rollup/issues/1083))
- Correctly deshadow destructured parameters with assignments ([#1008](https://github.com/rollup/rollup/issues/1008))

## 0.37.2

- Remove unused `new` expressions without side-effects ([#179](https://github.com/rollup/rollup/issues/179))
- Only remove valid sourceMappingURL comments ([#1132](https://github.com/rollup/rollup/issues/1132))
- Ensure blocks containing activated `var` declarations are included in output ([#1113](https://github.com/rollup/rollup/issues/1113))
- Support plugin outros ([#1116](https://github.com/rollup/rollup/issues/1116))

## 0.37.1

- Follow symlinks ([#447](https://github.com/rollup/rollup/issues/447))
- Fix tree-shaking of recursive functions and other cases ([#1120](https://github.com/rollup/rollup/issues/1120), [#1142](https://github.com/rollup/rollup/issues/1142))
- Support module names that require quotes ([#582](https://github.com/rollup/rollup/issues/582), [#584](https://github.com/rollup/rollup/issues/584))
- Fix [#957](https://github.com/rollup/rollup/issues/957)

## 0.37.0

- [BREAKING] Default exports are not included in reified namespaces ([#1028](https://github.com/rollup/rollup/issues/1028))
- Parentheses do not defeat tree-shaking ([#1101](https://github.com/rollup/rollup/issues/1101), [#1128](https://github.com/rollup/rollup/issues/1128))
- More `legacy` fixes: do not create getters ([#1069](https://github.com/rollup/rollup/pull/1069)), do not include `__esModule` ([#1068](https://github.com/rollup/rollup/pull/1068)), quote reserved property names ([#1057](https://github.com/rollup/rollup/pull/1057))
- Fix missing namespace member warnings ([#1045](https://github.com/rollup/rollup/issues/1045))
- Fix TypeError in arrow function without braces returning a function ([#1062](https://github.com/rollup/rollup/pull/1062))

## 0.36.4

- Only depend on program-level call expressions ([#977](https://github.com/rollup/rollup/issues/977))

## 0.36.3

- Add `legacy` option for IE8 support ([#989](https://github.com/rollup/rollup/pull/989))

## 0.36.2

- Insert semicolons where necessary to fix broken code ([#1004](https://github.com/rollup/rollup/issues/1004))
- Include module ID and location when warning about top-level `this` ([#1012](https://github.com/rollup/rollup/pull/1012))
- More informative error for missing exports ([#1033](https://github.com/rollup/rollup/issues/1033))
- `options.moduleContext` for per-module context overrides ([#1023](https://github.com/rollup/rollup/pull/1023))

## 0.36.1

- Include naked block statements ([#981](https://github.com/rollup/rollup/issues/981))
- Correctly include falsy alternate statements in optimised if blocks ([#973](https://github.com/rollup/rollup/issues/973))
- Prevent omission of default exports that are only used by the exporting module ([#967](https://github.com/rollup/rollup/pull/967))
- Prevent warning on `auto` exports with ES output ([#966](https://github.com/rollup/rollup/pull/966))

## 0.36.0

- `export { foo as default }` no longer creates a live binding ([#860](https://github.com/rollup/rollup/issues/860))

## 0.35.15

- Warn on missing unused imports in deshadowing phase ([#928](https://github.com/rollup/rollup/issues/928))
- Always add a newline to the end of bundles ([#958](https://github.com/rollup/rollup/issues/958))

## 0.35.14

- Include all parent statements of expression with effects, up to function boundary ([#930](https://github.com/rollup/rollup/issues/930))

## 0.35.13

- Include superclasses when including their subclasses ([#932](https://github.com/rollup/rollup/issues/932))

## 0.35.12

- Add `interop: false` option to disable unwrapping of external imports ([#939](https://github.com/rollup/rollup/issues/939))

## 0.35.11

- Deconflict reified namespaces with other declarations ([#910](https://github.com/rollup/rollup/issues/910))

## 0.35.10

- Only remove EmptyStatement nodes directly inside blocks ([#913](https://github.com/rollup/rollup/issues/931))

## 0.35.9

- Support Node 0.12 ([#909](https://github.com/rollup/rollup/issues/909))

## 0.35.8

- Correctly deshadow re-assigned module functions ([#910](https://github.com/rollup/rollup/issues/910))

## 0.35.7

- Refactor `flushTime.js` ([#922](https://github.com/rollup/rollup/pull/922))

## 0.35.6

- Fix browser build

## 0.35.5

- Allow empty for loop heads ([#919](https://github.com/rollup/rollup/issues/919))

## 0.35.4

- Preserve effects in for-of and for-in loops ([#870](https://github.com/rollup/rollup/issues/870))
- Remove empty statements ([#918](https://github.com/rollup/rollup/pull/918))

## 0.35.3

- Render identifiers inside template literals

## 0.35.2

- Fix broken build caused by out of date locally installed dependencies

## 0.35.1

- Rewrite deconflicted class identifiers ([#915](https://github.com/rollup/rollup/pull/915))
- Include `dependencies` in `bundle.modules` objects ([#903](https://github.com/rollup/rollup/issues/903))
- Update to Acorn 4 ([#914](https://github.com/rollup/rollup/pull/914))

## 0.35.0

- Rewrite analysis/tree-shaking code ([#902](https://github.com/rollup/rollup/pull/902))
- Include conditional mutations of global objects ([#901](https://github.com/rollup/rollup/issues/901))
- Only reify namespaces if necessary ([#898](https://github.com/rollup/rollup/issues/898))
- Track mutations of aliased globals ([#893](https://github.com/rollup/rollup/issues/893))
- Include duplicated var declarations ([#716](https://github.com/rollup/rollup/issues/716))

## 0.34.13

- Pass `{ format }` through to `transformBundle` ([#867](https://github.com/rollup/rollup/issues/867))

## 0.34.12

- Fix `rollup --watch` ([#887](https://github.com/rollup/rollup/issues/887))
- Case-sensitive paths ([#862](https://github.com/rollup/rollup/issues/862))

## 0.34.11

- Prevent leaky state when `bundle` is reused ([#875](https://github.com/rollup/rollup/issues/875))
- Ensure `intro` appears before interop block ([#880](https://github.com/rollup/rollup/issues/880))

## 0.34.10

- Allow custom `options.context` to replace top-level `this` ([#851](https://github.com/rollup/rollup/issues/851))
- Fix `noConflict` when used via `rollup --config` ([#846](https://github.com/rollup/rollup/issues/846))
- Place `outro` block _after_ export block ([#852](https://github.com/rollup/rollup/issues/852))

## 0.34.9

- Disable indentation by default, for faster bundle generation ([#812](https://github.com/rollup/rollup/pull/812))
- More helpful error on missing entry file ([#802](https://github.com/rollup/rollup/issues/802))
- Preserve comments before import declarations ([#815](https://github.com/rollup/rollup/pull/815))

## 0.34.8

- Wrap UMD factory function in parens to avoid lazy parsing ([#774](https://github.com/rollup/rollup/pull/774))

## 0.34.7

- Leave it up to resolveId to normalize the entry path ([#835](https://github.com/rollup/rollup/pull/835))
- Cache decoded mappings ([#834](https://github.com/rollup/rollup/pull/834))

## 0.34.5

- Fix circular export ([#813](https://github.com/rollup/rollup/issues/813))

## 0.34.4

- Module render performance tweak ([#823](https://github.com/rollup/rollup/pull/823))

## 0.34.3

- Avoid infinite recursion in `Bundle.sort()` ([#800](https://github.com/rollup/rollup/pull/800))

## 0.34.2

- resolveId calls are cached now to improve incremental build
- Fixed error message recursion in plugins

## 0.34.1

- Support `paths` config ([#754](https://github.com/rollup/rollup/issues/754))
- Allow `export *` from external module, internally

## 0.34.0

- Use resolved IDs for relative imports that are also external modules, to allow `options.globals` to work with them ([#763](https://github.com/rollup/rollup/issues/763))
- Ensure reassigned exports are declared in an ES bundle, and remove empty `exports.foo;` statements ([#755](https://github.com/rollup/rollup/issues/755))
- Add newline after sourcemap comment ([#756](https://github.com/rollup/rollup/issues/756))

## 0.33.2

- Add `bundle` as second argument to `ongenerate` and `onwrite` hooks ([#773](https://github.com/rollup/rollup/pull/773))
- Warn on top-level `this` ([#770](https://github.com/rollup/rollup/issues/770))

## 0.33.1

- Fix `--no-strict` option ([#751](https://github.com/rollup/rollup/pull/751))
- Fix Windows edge case with case-sensitive paths ([#760](https://github.com/rollup/rollup/pull/760))

## 0.33.0

- Downgrade missing transformer sourcemap to a warning, not an error, and print the name of the offending plugin if possible ([#746](https://github.com/rollup/rollup/issues/746))
- Warn if same name is re-exported from two modules ([#722](https://github.com/rollup/rollup/issues/722))

## 0.32.4

- Add `ongenerate` and `onwrite` plugin hooks ([#742](https://github.com/rollup/rollup/pull/742))

## 0.32.3

- Generated correct sourcemaps with reified namespaces ([#668](https://github.com/rollup/rollup/issues/668))
- Exclude plugin helper modules from sourcemaps ([#747](https://github.com/rollup/rollup/pull/747))

## 0.32.2

- Allow `--globals` to work with `--external` or `options.external` in whatever configuration ([#743](https://github.com/rollup/rollup/issues/743))

## 0.32.1

- Preserve side-effects to default exports that coincide with used named exports ([#733](https://github.com/rollup/rollup/issues/733))
- Support `rollup -c node:pkgname` ([#736](https://github.com/rollup/rollup/issues/736))

## 0.32.0

- Deprecate `es6` format in favour of `es` ([#468](https://github.com/rollup/rollup/issues/468))
- Add correct `jsnext:main` build ([#726](https://github.com/rollup/rollup/pull/726))

## 0.31.2

- Allow `load` plugins to provide sourcemap ([#715](https://github.com/rollup/rollup/pull/715))
- Allow `sourceMapFile` in config options ([#717](https://github.com/rollup/rollup/issues/717))

## 0.31.1

- Logging for errors emitted by `rollup-watch` ([#712](https://github.com/rollup/rollup/issues/712))

## 0.31.0

- Rewrite top-level `this` as `undefined` ([#707](https://github.com/rollup/rollup/pull/707))
- Pass `options.acorn` to Acorn ([#564](https://github.com/rollup/rollup/issues/564))

## 0.30.0

- Bundle CLI ([#700](https://github.com/rollup/rollup/issues/700))
- Ensure absolute paths are normalised ([#704](https://github.com/rollup/rollup/issues/704))
- Allow `rollup --watch` to work with targets

## 0.29.1

- Merge `target` options with main options ([#701](https://github.com/rollup/rollup/issues/701))
- Update magic-string ([#690](https://github.com/rollup/rollup/issues/690))

## 0.29.0

- `rollup --watch` ([#284](https://github.com/rollup/rollup/issues/284))

## 0.28.0

- Experimental support for incremental rebuilds ([#658](https://github.com/rollup/rollup/pull/658))

## 0.27.1

- Ensure names exported from a module are not replaced with reserved words ([#696](https://github.com/rollup/rollup/pull/696))
- Revert ([#692](https://github.com/rollup/rollup/pull/692)) – resolved IDs must be strings

## 0.27.0

- Use native promises instead of `es6-promise` ([#689](https://github.com/rollup/rollup/issues/689))
- Support multiple targets in config files ([#655](https://github.com/rollup/rollup/issues/655))
- Allow `resolveId` plugin functions to return non-strings ([#692](https://github.com/rollup/rollup/pull/692))

## 0.26.7

- Distinguish between default and namespace imports of external module ([#637](https://github.com/rollup/rollup/issues/637))
- Add `__esModule` property to named exports in AMD, CJS and UMD modes ([#650](https://github.com/rollup/rollup/issues/650))

## 0.26.6

- Deconflict named imports from external modules in ES bundles ([#659](https://github.com/rollup/rollup/issues/659))
- Support `options.preferConst` to generate `const` declarations for exports rather than `var` declarations ([#653](https://github.com/rollup/rollup/issues/653))

## 0.26.5

- Preserve `debugger` statements ([#664](https://github.com/rollup/rollup/issues/664))
- Allow `options.external` to be a function ([#522](https://github.com/rollup/rollup/issues/522))

## 0.26.4

- Prevent plugin-provided external IDs being normalised ([#630](https://github.com/rollup/rollup/issues/630), [#633](https://github.com/rollup/rollup/issues/633))
- Throw if module exports/re-exports the same name twice, or has multiple default exports ([#679](https://github.com/rollup/rollup/issues/679))
- Warn about `eval` security issue ([#675](<(https://github.com/rollup/rollup/issues/675)>))

## 0.26.3

- Ensure reference is not incorrectly marked as a reassignment ([#648](https://github.com/rollup/rollup/issues/648))

## 0.26.2

- Sanity check output of `load` hook ([#607](https://github.com/rollup/rollup/issues/607))
- Correct scoping for ID class expressions ([#626](https://github.com/rollup/rollup/issues/626))
- Warn if named and default exports are used together in auto mode ([#587](https://github.com/rollup/rollup/issues/587))
- Allow variable initialisers to be rewritten if necessary ([#632](https://github.com/rollup/rollup/issues/632))
- Prevent double `var` with no-treeshake option ([#639](https://github.com/rollup/rollup/pull/639))

## 0.26.1

- Add `treeshake: false`/`--no-treeshake` option for debugging ([#505](https://github.com/rollup/rollup/issues/505))
- Update build process to use Bublé ([#620](https://github.com/rollup/rollup/pull/620))

## 0.26.0

- Add `noConflict`/`--no-conflict` option for UMD builds ([#580](https://github.com/rollup/rollup/pull/580))
- Normalise relative external paths ([#591](https://github.com/rollup/rollup/pull/591))
- Report files causing transform errors ([#609](https://github.com/rollup/rollup/pull/609))
- Handle sourcemap segments with a single member ([#619](https://github.com/rollup/rollup/pull/619))
- Update dependencies

## 0.25.8

- Unixize entry path ([#586](https://github.com/rollup/rollup/pull/586))

## 0.25.7

- Expand deshadowed shorthand properties ([#575](https://github.com/rollup/rollup/issues/575))
- Allow external files to be non-existent ([#532](https://github.com/rollup/rollup/issues/532))

## 0.25.6

- Fix a regression introduced by #566 ([#569](https://github.com/rollup/rollup/issues/569))
- Prune dead conditional expressions more carefully ([#567](https://github.com/rollup/rollup/issues/567))

## 0.25.5

- Make sure shorthand destructuring assignments don't break ([#528](https://github.com/rollup/rollup/issues/528))
- Allow 'exports' key ([#542](https://github.com/rollup/rollup/issues/542))
- Ensure `foo. bar` where `foo` is a namespace import is rewritten correctly ([#566](https://github.com/rollup/rollup/issues/566))
- Fix an edge case for exported globals ( e.g. `export { document }`) ([#562](https://github.com/rollup/rollup/issues/562))

## 0.25.4

- Fix misnamed exports of default imports in ES bundles ([#513](https://github.com/rollup/rollup/issues/513))
- CLI: warn on missing config ([#515](https://github.com/rollup/rollup/pull/515))
- Detect side-effects in non-top-level member expression assignment ([#476](https://github.com/rollup/rollup/issues/476))
- Don't remove computed property class keys ([#504](https://github.com/rollup/rollup/issues/504))
- Augment existing global object rather than replacing ([#493](https://github.com/rollup/rollup/issues/493))
- Don't fail on `export {}`, warn instead ([#486](https://github.com/rollup/rollup/issues/486))

## 0.25.3

- Handle non-objects and `null` in `_interopDefault` ([#474](https://github.com/rollup/rollup/issues/474))

## 0.25.2

- Skip dead branches of a conditional expression (#[465](https://github.com/rollup/rollup/pull/465))
- Allow globals to be exported ([#472](https://github.com/rollup/rollup/pull/472))
- Ensure reassigned exports are exported ([#484](https://github.com/rollup/rollup/issues/484))

## 0.25.1

- Throw error if namespace is called ([#446](https://github.com/rollup/rollup/issues/446))
- Prevent shadowing bug in ES6 output ([#441](https://github.com/rollup/rollup/pull/441))
- Prevent `var exports.foo` ([#426](https://github.com/rollup/rollup/issues/426))
- Prevent double export of aliased symbols ([#438](https://github.com/rollup/rollup/issues/438))
- Provide more informative error if Rollup is used in-browser without appropriate `resolveId`/`load` hooks ([#275](https://github.com/rollup/rollup/issues/275))
- Use `_interopDefault` function to DRY out code with many external dependencies, in CommonJS output ([#458](https://github.com/rollup/rollup/pull/458))

## 0.25.0

- **breaking** Module order is determined according to spec, rather than in a way designed to prevent runtime errors. Rollup will warn if it detects runtime errors are likely ([#435](https://github.com/rollup/rollup/issues/435))
- Prevent overly aggressive tree-shaking with complex call expressions ([#440](https://github.com/rollup/rollup/issues/440))

## 0.24.1

- Handle calls to default exports other that are not function expressions or references to function declarations ([#421](https://github.com/rollup/rollup/issues/421))
- Ensure namespace blocks are created for chained imports ([#430](https://github.com/rollup/rollup/issues/430))
- Include references in computed property keys ([#434](https://github.com/rollup/rollup/issues/434))
- Use CLI `--external` option correctly ([#417](https://github.com/rollup/rollup/pull/417))
- Allow relative imports to be treated as external, if absolute paths are provided in `options.external` ([#410](https://github.com/rollup/rollup/issues/410))
- Make IIFE output adhere to Crockford style ([#415](https://github.com/rollup/rollup/pull/415))

## 0.24.0

- No longer attempts to resolve IDs in `options.external` ([#407](https://github.com/rollup/rollup/issues/407))
- Fix broken sourcemap resolution in cases where some modules are transformed and others aren't ([#404](https://github.com/rollup/rollup/issues/404))

## 0.23.2

- Ensure `dest` or `sourceMapFile` is resolved against CWD for purposes of sourcemap generation ([#344](https://github.com/rollup/rollup/issues/344))
- Support `banner`, `footer`, `intro` and `outro` options via CLI ([#330](https://github.com/rollup/rollup/issues/330))
- Allow `options.global` to be a function rather than an object, and warn on missing names ([#293](https://github.com/rollup/rollup/issues/293))
- Ensure side-effects are captured in cyclical call expressions ([#397](https://github.com/rollup/rollup/issues/397))
- Fix parse error with body-less arrow function expressions ([#403](https://github.com/rollup/rollup/issues/403))

## 0.23.1

- Reinstate missing fix from ([#392](https://github.com/rollup/rollup/pull/392))

## 0.23.0

- Add `bundleTransform` plugin hook and option ([#387](https://github.com/rollup/rollup/pull/387))
- Correctly store names in sourcemaps, regardless of transformers
- Add `--environment` option to CLI ([#388](https://github.com/rollup/rollup/pull/388))
- Handle destructuring in exports ([#374](https://github.com/rollup/rollup/issues/374))
- Fix UMD global exports bug introduced in 0.22.1 ([#392](https://github.com/rollup/rollup/pull/392))

## 0.22.2

- Prevent lost `var` keywords ([#390](https://github.com/rollup/rollup/issues/390))

## 0.22.1

- Update expected option keys ([#379](https://github.com/rollup/rollup/issues/379))
- Handle transformers that return stringified sourcemaps ([#377](https://github.com/rollup/rollup/issues/377))
- Automatically create missing namespaces if `moduleName` contains dots ([#378](https://github.com/rollup/rollup/issues/378))
- Ignore external dependency warnings coming from config file ([#333](https://github.com/rollup/rollup/issues/333))
- Update to latest magic-string for performance boost

## 0.22.0

- Duplicate warnings are squelched ([#362](https://github.com/rollup/rollup/issues/362))
- Plugins can manipulate or override the `options` object ([#371](https://github.com/rollup/rollup/pull/371))

## 0.21.3

- Validate option keys ([#348](https://github.com/rollup/rollup/pull/348))
- Allow namespaces imports to sit alongside named imports ([#355](https://github.com/rollup/rollup/issues/355))
- Count references inside destructured objects ([#364](https://github.com/rollup/rollup/issues/364))
- Preserve top-level `delete` statements ([#352](https://github.com/rollup/rollup/issues/352))

## 0.21.2

- Missing relative imports are an error, not a warning ([#321](https://github.com/rollup/rollup/issues/321))
- Fixed incorrectly renamed default exports in ES6 bundles ([#339](https://github.com/rollup/rollup/issues/339))
- Fixed infinite recursion bug ([#341](https://github.com/rollup/rollup/issues/341))

## 0.21.1

- Remove `aggressive: true` (was too aggressive) ([#309](https://github.com/rollup/rollup/pull/309))
- Handle top-level block statements ([#326](https://github.com/rollup/rollup/issues/326))
- Optimise namespaces with default exports ([#314](https://github.com/rollup/rollup/issues/314))

## 0.21.0

- Only include statements whose side-effects are relevant (i.e. contribute to exports or affect global state) ([#253](https://github.com/rollup/rollup/pull/253)) ([#253](https://github.com/rollup/rollup/pull/253))
- Exclude dead branches from analysis and inclusion ([#249](https://github.com/rollup/rollup/pull/249))
- Add `aggressive: true` option to eliminate all side-effects outside entry module
- More informative error when re-exporting non-existent binding ([#274](https://github.com/rollup/rollup/issues/274))
- Fix infinite recursion bug ([#291](https://github.com/rollup/rollup/issues/291))
- Log errors when using `rollup --config` ([#288](https://github.com/rollup/rollup/pull/288))
- Return rejected promises on startup instead of throwing error, if options are invalid ([#303](https://github.com/rollup/rollup/pull/303))

## 0.20.5

- Ensure re-exports don't create a local binding ([#270](https://github.com/rollup/rollup/pull/270))

## 0.20.4

- Check file exists at resolve time, to allow filenames with non-extension dots in them ([#250](https://github.com/rollup/rollup/pull/250))
- Import `Promise` where used, for Node 0.10 support ([#254](https://github.com/rollup/rollup/issues/254))
- Allow asynchronous transformer plugins ([#260](https://github.com/rollup/rollup/issues/260))
- Don't assume re-exported bindings are globals when deconflicting ([#267](https://github.com/rollup/rollup/issues/267))

## 0.20.3

- Fix bug where multiple `export *` declarations caused error ([#244](https://github.com/rollup/rollup/pulls/244))
- Missing namespace exports are a warning, not an error ([#244](https://github.com/rollup/rollup/pulls/244))
- Plugins can provide `banner` and `footer` options (string, or function that returns a string) ([#235](https://github.com/rollup/rollup/issues/235))
- Warn on encountering `eval` ([#186](https://github.com/rollup/rollup/issues/186))

## 0.20.2

- Handle errors in build config file
- More robust deconflicting, in cases where e.g. `foo$1` already exists
- Use Rollup CLI for own build process

## 0.20.1

- Support `--config` file to enable plugins with CLI ([#226](https://github.com/rollup/rollup/pulls/226))
- Prevent `default` being used as variable name ([#215](https://github.com/rollup/rollup/issues/215))
- Update deps

## 0.20.0

- Support for [plugins](https://github.com/rollup/rollup/wiki/Plugins) ([#207](https://github.com/rollup/rollup/pulls/207))
- BREAKING – `options.transform`, `options.load`, `options.resolveId`, `options.resolveExternal` and `options.external` are no longer supported, and should be handled by plugins. [More info](https://github.com/rollup/rollup/wiki/Plugins)
- BREAKING – the .js extension is only added if it looks like there's no extension, allowing e.g. `import data from 'data.json'` (with the appropriate transformer). For safety, always include the file extension – import `./foo.js`, not `./foo`

## 0.19.2

- Fix exporting namespaces to include all of their exports ([#204](https://github.com/rollup/rollup/issues/204))
- Namespace exotic objects are frozen to ensure that its properties cannot be modified, reconfigured, redefined or deleted ([#203](https://github.com/rollup/rollup/pulls/203))
- Fix `ReferenceError: Promise is not defined` in node v0.10 ([#189](https://github.com/rollup/rollup/issues/189))

## 0.19.1

- Fix `module.basename()` when used with custom `resolveId` function
- Use [rollup-babel](https://github.com/rollup/rollup-babel) to build self
- Exposed the version string through the API: `require( 'rollup' ).VERSION`

## 0.19.0

- **breaking** The `transform` option is no longer passed through to custom loaders. Loaders should only concern themselves with providing source code; transformation will _always_ take place
- `options.transform` functions can return a string, or a `{code, map, ast}` object. Where possible, sourcemap chains will be flattened ([#175](https://github.com/rollup/rollup/pull/175))
- `options.resolveId`, `options.resolveExternal` and `options.load` can each be a function or an array of functions. If an array, the first non-null/undefined return value is used. In both cases, failed resolution/loading will fall back to the defaults, unless an error is thrown. ([#174](https://github.com/rollup/rollup/pull/174))
- New `intro` and `outro` options – similar to `banner` and `footer` except inserted _inside_ any format-specific wrapper
- Multiple var declarations in an export block (e.g. `export let a = 1, b = 2`) are split up to facilitate tree-shaking ([#171](https://github.com/rollup/rollup/issues/171))
- More informative error when using a missing namespace property ([#169](https://github.com/rollup/rollup/pull/169))
- Update various dependencies

## 0.18.5

- Allow namespaces to be assigned to variables ([#168](https://github.com/rollup/rollup/issues/168))
- Promote `chalk` and `source-map-support` to `dependencies`, as they're used by the CLI ([#167](https://github.com/rollup/rollup/pull/167))

## 0.18.4

- Make external modules configurable (i.e. `external.config.foo = 'bar'`) without erroring

## 0.18.3

- Crop indent exclusion ranges to exclude enclosing quotes ([#166](https://github.com/rollup/rollup/issues/166))

## 0.18.2

- Include definitions of namespace members that are exported as defaults

## 0.18.1

- Include `acorn.parse` in bundle, remove `sander` from dependencies, simplify build

## 0.18.0

- Internal rewrite
- Reinstate statically-analysable namespace imports
- Avoid using getters in namespace blocks where possible ([#144](https://github.com/rollup/rollup/issues/144))
- Track variable aliases ([#96](https://github.com/rollup/rollup/issues/96))
- Prevent multiline strings being indented ([#164](https://github.com/rollup/rollup/issues/164))

## 0.17.4

- Allow imports from hidden directories (replay of [#133](https://github.com/rollup/rollup/issues/133))

## 0.17.3

- Handle parenthesised default exports ([#136](https://github.com/rollup/rollup/issues/136))

## 0.17.2

- Allow use of scoped npm packages ([#131](https://github.com/rollup/rollup/issues/131))

## 0.17.1

- Allow namespaces to be passed to a function ([#149](https://github.com/rollup/rollup/issues/149))

## 0.17.0

- Roll back to 0.15.0 and reapply subsequent fixes pending resolution of ([#132](https://github.com/rollup/rollup/issues/132)) and related issues

## 0.16.4

- Fix import paths with `.` ([#133](https://github.com/rollup/rollup/issues/133))
- Prevent sourceMappingURL confusion leading to broken sourcemap
- Add code coverage reporting [#130](https://github.com/rollup/rollup/pull/130))
- Add `modules` property to user-facing `bundle` – an array with `{id}` objects ([#128](https://github.com/rollup/rollup/issues/128))

## 0.16.3

- Prevent adjacent blocks of multiple var declarations causing magic-string failure ([#105](https://github.com/rollup/rollup/issues/105))

## 0.16.2

- Top-level function calls and assignments to globals are treated as side-effects, and always included
- Import files from subdirectories of external packages, e.g. `import mod from 'foo/sub/mod'` ([#126](https://github.com/rollup/rollup/issues/126))

## 0.16.1

- Handle assignment patterns, and destructured/rest parameters, when analysing scopes
- Fix bug preventing project from self-building (make base `Identifier` class markable)

## 0.16.0

- Internal refactoring ([#99](https://github.com/rollup/rollup/pull/99))
- Optimisation for statically-analysable namespace imports ([#99](https://github.com/rollup/rollup/pull/99))
- Windows support ( theoretically!) ([#117](https://github.com/rollup/rollup/pull/117) / [#119](https://github.com/rollup/rollup/pull/119))

## 0.15.0

- Load all modules specified by `import` statements, and do tree-shaking synchronously once loading is complete. This results in simpler and faster code, and enables future improvements ([#97](https://github.com/rollup/rollup/pull/97))
- Only rewrite `foo` as `exports.foo` when it makes sense to ([#92](https://github.com/rollup/rollup/issues/92))
- Fix bug with shadowed variables that are eventually exported ([#91](https://github.com/rollup/rollup/issues/91))
- Exclude unused function declarations that happen to modify a used name ([#90](https://github.com/rollup/rollup/pull/90))
- Simplify internal `Scope` model – scopes always attach to blocks, never function expressions/declarations

## 0.14.1

- `export { name } from './other'` does not create a local binding ([#16](https://github.com/rollup/rollup/issues/16))
- A single binding can be exported under multiple names ([#18](https://github.com/rollup/rollup/issues/18))
- `useStrict` option exposed to CLI as `--strict`/`--no-strict` ([#81](https://github.com/rollup/rollup/issues/81))
- Neater exports from ES6 bundles

## 0.14.0

- Internal refactoring
- Correctly deconflict generated default export names ([#72](https://github.com/rollup/rollup/issues/72))
- Handle `export { x } from 'y'` declarations ([#74](https://github.com/rollup/rollup/issues/74))
- Dedupe named imports from external modules in ES6 bundles ([#77](https://github.com/rollup/rollup/issues/77))

## 0.13.0

- Support `banner` and `footer` options ([#66](https://github.com/rollup/rollup/pull/66))
- Remove pre-existing sourcemap comments ([#66](https://github.com/rollup/rollup/pull/66))
- Deconflict external imports ([#66](https://github.com/rollup/rollup/pull/66))
- Use existing AST, if provided ([#66](https://github.com/rollup/rollup/pull/66))
- Rename internal namespace exports as appropriate ([#66](https://github.com/rollup/rollup/pull/66))
- Remove uninitialised var declarations that get exported ([#66](https://github.com/rollup/rollup/pull/66))
- Rename variables named `exports` to avoid conflicts ([#66](https://github.com/rollup/rollup/pull/66))

## 0.12.1

- Don't attempt to mark statements belonging to external modules ([#68](https://github.com/rollup/rollup/issues/68))
- Correctly deshadow variables that conflict with imports ([#68](https://github.com/rollup/rollup/issues/68))

## 0.12.0

- Internal re-architecting, resulting in more efficient bundling with reduced memory usage
- Shorthand properties are expanded if necessary ([#61](https://github.com/rollup/rollup/issues/61))
- Fixed various bugs with bundle external dependencies, particularly when generating ES6 bundles ([#59](https://github.com/rollup/rollup/issues/59))
- Add `--globals` option to CLI ([#60](https://github.com/rollup/rollup/pull/60))
- Allow imports of external modules for side-effects ([#55](https://github.com/rollup/rollup/pull/55))
- Prevent Rollup hanging on non-existent external module ([#54](https://github.com/rollup/rollup/pull/54))

## 0.11.4

- Side-effect preservation applies to internal default exports ([#43](https://github.com/rollup/rollup/issues/43))

## 0.11.3

- Class methods are not incorrectly renamed ([#42](https://github.com/rollup/rollup/issues/42))
- External modules are assigned names before canonical names are determined ([#42](https://github.com/rollup/rollup/issues/42))

## 0.11.2

- Correctly handle computed properties (e.g. `foo[bar]`) when discovering dependencies ([#47](https://github.com/rollup/rollup/pull/47))

## 0.11.1

- Support for `export * from '..'` ([#46](https://github.com/rollup/rollup/pull/46))

## 0.11.0

- Experimental browser-friendly build (`dist/rollup.browser.js`) ([#25](https://github.com/rollup/rollup/issues/25))
- Internal re-architecting to make discovery process simpler and more performant
- Preservation of side-effects that happen in a separate module to the affected definition ([#39](https://github.com/rollup/rollup/issues/39))

## 0.10.0

- Better sorting algorithm – sorting happens at the module level, rather than the statement level. This avoids certain edge cases
- IIFEs are ignored for the purposes of distinguishing between 'strong' and 'weak' dependencies
- Empty `var` declarations for exported bindings are omitted

## 0.9.1

- Much faster statement insertion (fixes major 0.9.0 performance regression)

## 0.9.0

- BREAKING - `resolvePath` is now `resolveId`. The returned `id` (which by default is a filepath) is passed to the `load` function, which can optionally be overridden, and which is applied to all modules including the entry module. This allows custom resolver and loading logic for integration with third party systems (e.g. JSPM) or, eventually, in-browser usage ([#30](https://github.com/rollup/rollup/issues/30))
- A statement cannot appear after later statements from the same bundle ([#34](https://github.com/rollup/rollup/issues/34))
- Tricky cyclical dependencies are handled ([#36](https://github.com/rollup/rollup/issues/36))
- `sourcemap` option is used by CLI (was omitted previously)

## 0.8.3

- Correctly rename functions that have arguments with the same name ([#32](https://github.com/rollup/rollup/issues/32))
- Ensure unused default exports are given a legal name ([#33](https://github.com/rollup/rollup/issues/33))

## 0.8.2

- Support `moduleId` and `moduleName` via CLI ([#24](https://github.com/rollup/rollup/issues/24))

## 0.8.1

- Anonymous functions that are exported as default are converted to named function declarations for correct hoisting, rather than being bound to functions ([#29](https://github.com/rollup/rollup/issues/29))
- Automatically-generated default export names are deconflicted with local definitions ([#29](https://github.com/rollup/rollup/issues/29))

## 0.8.0

- Top-level variable declarations with multiple declarators are split up, to avoid unnecessary code importing and incorrectly-ordered statements ([#26](https://github.com/rollup/rollup/issues/26))
- `this` at the top level is `undefined` ([#28](https://github.com/rollup/rollup/issues/28))

## 0.7.8

- Avoid using `path.parse` - unsupported in node 0.10

## 0.7.7

- Promise `source-map-support` from `devDependencies` to `dependencies` ([#23](https://github.com/rollup/rollup/issues/23))

## 0.7.6

- Better placement of `export default` statements ([#21](https://github.com/rollup/rollup/issues/21))
- Prevent function calls and property assignments from being treated as rebinding for sake of unbound default exports
- Add `--external foo,bar,baz` option to CLI (equivalent to `external: ['foo', 'bar', 'baz']`)
- Add CLI tests

## 0.7.5

- Prevent accidental conflicts with the global namespace ([#20](https://github.com/rollup/rollup/issues/20))

## 0.7.4

- More precise statement re-ordering to satisfy `export default` constraint (fixes bug introduced in 0.7.3)

## 0.7.3

- Default exports are not bound. To enable this, statements within a module are sorted to retain their original order ([#15](https://github.com/rollup/rollup/issues/15))
- Better positioning of comments ([#14](https://github.com/rollup/rollup/issues/14))
- Various fixes to get Travis-CI rigged up

## 0.7.2

- Fix sourcemap paths on Windows ([#6](https://github.com/rollup/rollup/pull/6))

## 0.7.1

- Named functions can be used as default exports from a bundle
- Method calls are assumed to mutate the owner (i.e. `foo.bar()` mutates `foo`) ([#13](https://github.com/rollup/rollup/issues/13))
- `options.indent` can be used to control indentation of resulting bundle. `options.true` (default) means ' auto', `options.false` means empty string. Alternatively specify whitespace e.g. `' '` or `'\t'` ([#5](https://github.com/rollup/rollup/issues/5))

## 0.7.0

- Ensure statements are always separated by a newline ([#9](https://github.com/rollup/rollup/pull/9))
- Use CommonJS `exports` correctly (UMD exports)
- Throw error if `moduleName` is required but missing (UMD exports)
- Attach IIFE global to `this` rather than `window`
- Allow names inside bundle to the the names of `Object.prototype` properties ([#12](https://github.com/rollup/rollup/pull/12))
- Keep exports live ([#11](https://github.com/rollup/rollup/pull/11))

## 0.6.5

- Add sourceMappingURL comment to code, as appropriate
- Higher resolution sourcemaps

## 0.6.4

- Fix CJS bundling with default export

## 0.6.3

- Fix exports and external module imports with some output formats
- Fix endless cycle bug on Windows ([#3](https://github.com/rollup/rollup/pull/3)) - thanks @Bobris

## 0.6.2

- Permit assignments to properties of imported bindings

## 0.6.1

- Support for basic transformers

## 0.6.0

- BREAKING - `rollup.rollup` and `bundle.write` both take a single options argument
- BREAKING - external modules must be declared upfront with `options.external: [...]`
- Non-relative module paths will be resolved by looking for `jsnext:main` fields in the appropriate `package.json` files. This behaviour can be overridden by passing an alternative `resolveExternal` function
- Fix sourcemap options
- Include CLI files in npm package (duh)

## 0.5.0

- Command line interface
- Sourcemap generation
- Correct behaviour with `export { x as y } from 'z'`

## 0.4.1

- More import name deconflicting

## 0.4.0

- Self-hosting! `rollup.rollup` now rolls up rollup
- Fix bug with comments inside a statement later being appended to it
- Prevent shadowing of external modules
- Rewrite computed property identifiers where necessary
- Preserve original statement order where possible
- Internal refactoring

## 0.3.1

- Saner deconflicting
- Rename namespace imports from external modules correctly

## 0.3.0

- Basic functionality present, mostly spec-compliant

## 0.2.1

- Include dist files in npm package (duh)

## 0.2.0

- First release capable of doing anything useful
- Still lots of basic functionality missing

## 0.1.0

- Initial experiment
