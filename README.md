# sveltekit-frontend-backend

A starter monorepo separating SvelteKit front-end and backend code, in TypeScript

NOTICE: This package is experimental prior to NPM release 1.0.0 and will continually evolve before then.

## Notes

Implemented with yarn workspaces. List each package folder in the `workspaces` entry of the root `packages.json`. To create a new SvelteKit package, run `npm init svelte package-folder` from the repo root.

Create a `package.json` for each package folder, and set `"name"` to `@repo-name/package-name` in each. To add a package to a sister package, use this dependency:

`"@repo-name/package-name": "*"`

Run `yarn` from the root package to update dependencies in all packages.

# Details

I've temporarily removed the following, as it might not be needed...

> I appended the following to `frontend/tsconfig.json` to pull in shared TypeScript:

```json
    "include": [
		"**/*.ts",
		"../shared/**/*.ts"
	]
```
