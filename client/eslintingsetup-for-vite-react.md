# vite - react eslinting setup

**install eslint**

```console
npm install --save-dev eslint-config-react-app eslint@^8.0.0
```

**create a .eslintrc.json file**

```jsx
// .eslintrc.json contents
{"extends": ["react-app", "react-app/jest"]}
```

**Once installed, install vite eslint plugin**
```console
npm i vite-plugin-eslint -D
``` 

**Finally add the following plugins to vite.config.js as plugin like so**

```jsx
import eslint from "vite-plugin-eslint";
// https://vitejs.dev/config/
export default defineConfig({
  plugins: [react(), eslint()],
});
```

`Refer`

<!-- //stackoverflow.com/questions/69842785/how-can-i-intregate-eslint-in-a-vitereact-project -->
<!-- https://www.npmjs.com/package/eslint-config-react-app -->
<!-- https://www.npmjs.com/package/vite-plugin-eslint -->
