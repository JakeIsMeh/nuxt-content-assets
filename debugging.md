npm is doing something wrong as usual (rollup natives missing)

- used pnpm

---

generated nuxt entry file is asking for `ipx` directly instead of using proper 
pnpm import (file://path/to/proj/node_modules/.pnpm/ipx@3.0.1/index.js)

- set `ipx` as a devDependency for playground (hacky workaround, but so is using --shamefully-hoist)

---

in @nuxt/image 1.7.1, the runtime components are now distributed as `.vue` files 
instead of `.js` files.

- updated import in playground/components/content/NuxtImg.ts
