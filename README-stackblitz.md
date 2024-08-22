# shadcn-docs starter

**"Beautifully designed Nuxt Content template built with shadcn-vue.
Customizable. Compatible. Open Source."**

- https://shadcn-docs-nuxt.vercel.app/
- https://github.com/ZTL-UwU/shadcn-docs-nuxt

```shell
# using stackblitz webide
 npx nuxi@latest init shadcn-docs-starter -t github:ZTL-UwU/shadcn-docs-nuxt-starter
 ERROR unable to fetch...
```

try opening the template repo above with stackblitz: ZTL-UwU/shadcn-docs-nuxt-starter...

- dependencies crash ide during npm install
- pnpm does not seem to work

try using yarn:

add `"startCommand": "yarn dev",` to package.json
run `yarn` in terminal to install packages
run `yarn run dev` in terminal to launch dev server

add the following to `package.json`:
```
  "stackblitz": {
    "startCommand": "yarn; yarn run dev" 
  },
```

**important**: IF USING legacy stackblitz IDE (NOT Codeflow), set vscode workspace settings to disable "format on save" (at least for markdown files) - it fucks up the important spacing for nuxt-docs special mdc format apparently"

```
# in .vscode/settings.json:
"editor.formatOnSave": false,
```
