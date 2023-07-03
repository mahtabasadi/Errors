
# 1: Module not found: Can't resolve 'react-router-dom' [Solved]
## راه حل 

 ### 👇️ with NPM
`npm install react-router-dom`

### 👇️ ONLY If you use TypeScript
`npm install --save-dev @types/react-router-dom`

## راه حل دوم
 Delete your node_modules and reinstall your dependencies

 `delete your node-modules`
 `delete your package-lock.json`

 ### 👇️ clean npm cache
npm cache clean --force

### 👇️ install packages
npm install

## راه حل سوم
 Verify react-router-dom is in your dependencies object:

 If you still get the error, open your package.json file and make sure it contains the react-router-dom package in the dependencies object.

`package.json

{
  // ... rest
  "dependencies": {
    "react-router-dom": "^6.3.0",
  },
  "devDependencies": {
    // 👇️ only if you use TypeScript
    "@types/react-router-dom": "^5.3.3"
  }
}
`

The `react-router-dom` module should NOT be globally installed or be in your project's `devDependencies`. It should be in the `dependencies` object in your `package.json` file.
You can try to manually add the lines and re-run `npm install`.

