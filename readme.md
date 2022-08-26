This an example repo for https://github.com/pnpm/pnpm/issues/5234

imaging this was a docker build that takes only part of the project (e.g. the sub package broken),

when running `pnpm install` you would expect it to succeed since the sub package does not have any package dependencies, but instead you get 
```
❯ pnpm install
Scope: all 2 workspace projects
 ERR_PNPM_PATCH_NOT_APPLIED  The following patches were not applied: is-odd@3.0.1

Either remove them from "patchedDependencies" or update them to match packages in your dependencies.
```