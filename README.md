This is the defualt docusaurus template buit with:

```bash
npx @docusaurus/init@latest init sandpack-docusaurus-test classic
```

with [this changes](https://github.com/pomber/sandpack-docusaurus-test/commit/11d277abacffca96ea671b2fab84839aaa8ac3b8).

---

Repro:

1. Clone repo
1. Run:

```bash
yarn
yarn start
```

---

Error:

```error
client.js?e6b8:10 Uncaught (in promise) ReferenceError: process is not defined
    at eval (webpack-internal:///./node_modules/@codesandbox/sandpack-client/esm/client.js:21)
    at Module../node_modules/@codesandbox/sandpack-client/esm/client.js (:3000/vendors-node_modules_codesandbox_sandpack-react_dist_esm_presets_SandpackRunner_js.js:23)
    at __webpack_require__ (:3000/runtime~main.js:36)
    at fn (:3000/runtime~main.js:339)
    at eval (webpack-internal:///./node_modules/@codesandbox/sandpack-react/dist/esm/contexts/sandpackContext.js:8)
    at Module../node_modules/@codesandbox/sandpack-react/dist/esm/contexts/sandpackContext.js (:3000/vendors-node_modules_codesandbox_sandpack-react_dist_esm_presets_SandpackRunner_js.js:143)
    at __webpack_require__ (:3000/runtime~main.js:36)
    at fn (:3000/runtime~main.js:339)
    at eval (webpack-internal:///./node_modules/@codesandbox/sandpack-react/dist/esm/hooks/useSandpack.js:6)
    at Module../node_modules/@codesandbox/sandpack-react/dist/esm/hooks/useSandpack.js (:3000/vendors-node_modules_codesandbox_sandpack-react_dist_esm_presets_SandpackRunner_js.js:183)
    at __webpack_require__ (:3000/runtime~main.js:36)
    at fn (:3000/runtime~main.js:339)
    at eval (webpack-internal:///./node_modules/@codesandbox/sandpack-react/dist/esm/common/Layout.js:8)
    at Module../node_modules/@codesandbox/sandpack-react/dist/esm/common/Layout.js (:3000/vendors-node_modules_codesandbox_sandpack-react_dist_esm_presets_SandpackRunner_js.js:79)
    at __webpack_require__ (:3000/runtime~main.js:36)
    at fn (:3000/runtime~main.js:339)
    at eval (webpack-internal:///./node_modules/@codesandbox/sandpack-react/dist/esm/presets/SandpackRunner.js:7)
    at Module../node_modules/@codesandbox/sandpack-react/dist/esm/presets/SandpackRunner.js (:3000/vendors-node_modules_codesandbox_sandpack-react_dist_esm_presets_SandpackRunner_js.js:215)
    at __webpack_require__ (:3000/runtime~main.js:36)
    at fn (:3000/runtime~main.js:339)
    at eval (webpack-internal:///./src/pages/index.js:12)
    at Module../src/pages/index.js (:3000/component---site-src-pages-index-jsc-4-f-f99.js:47)
    at __webpack_require__ (:3000/runtime~main.js:36)
    at Function.fn (:3000/runtime~main.js:339)
```
