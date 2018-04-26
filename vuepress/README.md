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

## Notes

- you can pass directory to `vuepress` command, i.e. `vuepress dev docs` would use `./docs` instead of current folder