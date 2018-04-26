# fe-template

Base template for dashboard, documentation etc.

## Usage

## Dev

````bash
npm install -g vuepress
npm install -g @angular/cli
````

## Known issues

- `package-lock.json` may not work for cross platform development, i.e. `fsevent` is not installed on linux but required on mac
  - since I don't have a mac, it works for me

## License

MIT

## About

I got many side projects that has a dashboard or a website for documentation.
I often copy and paste between them for updating dependencies and shims,
thus I decided to put the shared codebase in one place and copy it to all the other projects.