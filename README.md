# eleventy-vite-test-01

- Check that it serves and builds just as starter blog
  - Works on Mac and Windows
- Add vite plugin and test serve and build
  - Serve works, build breaks on windows
- If breaks, test on Mac
  - Breaks on Mac
- If that works, try custom input / output folders

Mac error:  
 ✝  testing/2022/pg-11ty-vite-test-01   master±  npm run build

> muac-digital-cv@1.0.0 build

> npx @11ty/eleventy

[11ty] Writing \_site/index.html from ./index.njk

vite v2.8.6 building for production...

✓ 1 modules transformed.

[vite]: Rollup failed to resolve import "css/index.css" from ".11ty-vite/index.html".

This is most likely unintended because it can break your application at runtime.

If you do want to externalize this module explicitly add it to

`build.rollupOptions.external`

[11ty] Encountered a Vite build error, restoring original Eleventy output to \_site Error: [vite]: Rollup failed to resolve import "css/index.css" from ".11ty-vite/index.html".

This is most likely unintended because it can break your application at runtime.

If you do want to externalize this module explicitly add it to

`build.rollupOptions.external`

    at onRollupWarning (/Users/patrickgrey/Documents/rising-sky/testing/2022/pg-11ty-vite-test-01/node_modules/vite/dist/node/chunks/dep-9c153816.js:39242:19)

    at onwarn (/Users/patrickgrey/Documents/rising-sky/testing/2022/pg-11ty-vite-test-01/node_modules/vite/dist/node/chunks/dep-9c153816.js:39020:13)

    at Object.onwarn (/Users/patrickgrey/Documents/rising-sky/testing/2022/pg-11ty-vite-test-01/node_modules/rollup/dist/shared/rollup.js:23129:13)

    at ModuleLoader.handleResolveId (/Users/patrickgrey/Documents/rising-sky/testing/2022/pg-11ty-vite-test-01/node_modules/rollup/dist/shared/rollup.js:22419:26)

    at /Users/patrickgrey/Documents/rising-sky/testing/2022/pg-11ty-vite-test-01/node_modules/rollup/dist/shared/rollup.js:22380:26 {

watchFiles: [

    '/Users/patrickgrey/Documents/rising-sky/testing/2022/pg-11ty-vite-test-01/.11ty-vite/index.html'

]

}

[11ty] Problem writing Eleventy templates: (more in DEBUG output)

[11ty] ENOENT: no such file or directory, stat '/Users/patrickgrey/Documents/rising-sky/testing/2022/pg-11ty-vite-test-01/.11ty-vite' (via Error)

[11ty]

[11ty] Original error stack trace: Error: ENOENT: no such file or directory, stat '/Users/patrickgrey/Documents/rising-sky/testing/2022/pg-11ty-vite-test-01/.11ty-vite'

[11ty] Copied 2 files / Wrote 1 file in 0.14 seconds (v2.0.0-canary.4)
