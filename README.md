# sveltekit-frontend-backend

A starter monorepo separating SvelteKit front-end and backend code, in TypeScript

NOTICE: This package is experimental prior to NPM release 1.0.0 and will continually evolve before then.

## Notes

Implemented with yarn workspaces. List each package in the `workspaces` entry of `packages.json`.

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
