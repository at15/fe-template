# Angular Dashboard

## Dev

````bash
# call ng new empty to use latest @angular/cli to create app called empty
make new-empty
make new-zorro
````

The app name is used in following places

- `package.json` `name`
- `.angular-cli.json` `name`, will be changed to `angular-cli.json`
- `e2e/app.e2e-spec.ts`
- `README.md`
- `src/index.html`

To test if a patch is working

````bash
# start a dev server
ng serve
````

### NG-ZORRO

https://github.com/NG-ZORRO/ng-zorro-antd

- using 0.7.0-beta.4

TODO

- [ ] login & register page (may not have logic for backend)
- [ ] dashboard page
- [ ] update [benchhub](https://github.com/benchhub/benchhub) to use it