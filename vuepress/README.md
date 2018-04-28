# Static website using VuePress

- https://vuepress.vuejs.org/

## Dev

````bash
make new empty
````

To test

````bash
npm run docs:dev
````

## Layers

### 0-Original

Just a README.md with default theme

- https://vuepress.vuejs.org/guide/getting-started.html
- `npm install --save-dev vuepress`
- add scripts to package.json
  - NOTE: when using `docs` folder instead of project root, change command to `vuepress dev docs`

````json
{
  "scripts": {
    "docs:dev": "vuepress dev",
    "docs:build": "vuepress build"
  }
}
````

- for in place update, run `npm update --dev`
- for clean update
  - `make rm-0-original`
  - `make new-0-original`
  - `make patch-0-original`

### 1-awesome

A table component for awesome list, allow filtering by multiple conditions

- https://vuepress.vuejs.org/guide/using-vue.html#using-components
- https://github.com/vuejs/vuepress/tree/master/docs/.vuepress/components
- `.vuepress/components` contains vue component, it can import js file in other folder using webpack

## Notes

- you can pass directory to `vuepress` command, i.e. `vuepress dev docs` would use `./docs` instead of current folder