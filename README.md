# Bug Angular devkit called `writeWorkspace`

Bug when generating angular library

Run this

```bash
pnpm install

pnpm nx generate @nrwl/angular:library test1 --dry-run --verbose

```

```
[NX] Angular devkit called `writeWorkspace`, this may have had unintended consequences in angular.json
[NX] Double check angular.json before proceeding
Skipping test1 since libs/test1/project.json already exists.
UPDATE angular.json
CREATE libs/test1/README.md
CREATE libs/test1/tsconfig.lib.json
CREATE libs/test1/tsconfig.spec.json
CREATE libs/test1/src/index.ts
CREATE libs/test1/src/lib/test1.module.ts
CREATE libs/test1/tsconfig.json
CREATE libs/test1/project.json
UPDATE tsconfig.base.json
CREATE libs/test1/jest.config.ts
CREATE libs/test1/src/test-setup.ts
CREATE libs/test1/.eslintrc.json

```

## NX report

```
Node : 14.20.1
   OS   : darwin x64
   pnpm : 7.9.0

   nx : 14.7.13
   @nrwl/angular : 14.7.13
   @nrwl/cypress : 14.7.13
   @nrwl/detox : Not Found
   @nrwl/devkit : 14.7.13
   @nrwl/eslint-plugin-nx : 14.7.13
   @nrwl/expo : Not Found
   @nrwl/express : Not Found
   @nrwl/jest : 14.7.13
   @nrwl/js : 14.7.13
   @nrwl/linter : 14.7.13
   @nrwl/nest : Not Found
   @nrwl/next : Not Found
   @nrwl/node : Not Found
   @nrwl/nx-cloud : Not Found
   @nrwl/nx-plugin : Not Found
   @nrwl/react : Not Found
   @nrwl/react-native : Not Found
   @nrwl/schematics : Not Found
   @nrwl/storybook : 14.7.13
   @nrwl/web : Not Found
   @nrwl/workspace : 14.7.13
   typescript : 4.8.3
```
