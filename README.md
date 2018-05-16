# fe-template

Base frontend templates for dashboard and documentation.

- [dashboard](ngdash) Angular + And Design (NG-ZORRO)
- [documentation](vuepress) VuePress

## Dev

````bash
npm install -g vuepress
npm install -g @angular/cli
````

The templates are built from layers

- layer 0 is generated from official cli
- layer n is built from layer n-1
- layer na and layer nb are both from layer n-1

## Known issues

- `package-lock.json` may not work for cross platform development, i.e. `fsevent` is not installed on linux but required on mac
  - since I don't have a mac, it works for me

## License

MIT

## About

I got many side projects that has a dashboard or a website for documentation.
I often copy and paste between them for updating dependencies and shims,
thus I decided to put the shared codebase in one place and copy it to all the other projects.