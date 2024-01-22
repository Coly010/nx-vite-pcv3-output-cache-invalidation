## Repo Highlighting Cacheable Target Invalidated by Build Output

This repo demonstrates the issue where a cacheable target's output will invalidate the task's cache, effectively meaning the task will never be restored from cache.

### Reproduction

1. Clone the repo
2. Run `npm install`
3. Run `npx nx build`
4. Re-Run `npx nx build` <- Note that it does not read from cache

