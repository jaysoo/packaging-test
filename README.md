# Packaging test repo

This is a test repo for JS packages. There are two packages, `@test/one` and `@test/two`, where the latter has a dependency on the former.

You can run the release command, and Nx will update all the versions correctly in `dist`.

```shell
npx nx release 1.0.1 
```

Inspect both `dist/packages/one/package.json` and `dist/packages/two/package.json` and see that the versions are bumped and two's dependency on one is also bumped.


