## NPM package starter

---

Very basic boilerplate for npm packages (tries to stay minimalist)

---

# how to release the package

1. Put all your code to `src` folder.
2. Commit to qest [GitHub](https://github.com/qest-cz?type=source)
3. Create new [Azure pipeline](https://dev.azure.com/qest/Qest/_apps/hub/ms.vss-build-web.ci-designer-hub)
   1. Select `GitHub`
   2. Find your repository
   3. `Run` the pipeline
   4. Every commit to master should release new version of the package

```
Every release has to increase version in packages.json
```

# file structure

- `src` - this is where all your code belongs
- `tslint/prettier` - your every day linter files
- `tsconfig` - here you specify what to build and where to put it
- `azure.pipelines` - this is yml file for azure, which should publish the package under qest organization
