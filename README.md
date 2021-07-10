# capacitor-ios-playground
Capacitor iOS platform web project playground using `Vite` + `Vue3` + `WindiCSS`(Tailwind).

[Capacitor Playground](https://dennischungtw.github.io/capacitor-ios-playground/)

## Setup
- `npm install`, this should install all need module from npm.
## Develop
### Web UI dev
- `npm run dev` open Vite.js develop server

![image](https://user-images.githubusercontent.com/79894563/124779755-9d1c2580-df74-11eb-83e6-ede60def6f37.png)

Follow [Tailwind CSS](https://tailwindcss.com/) + [Pug](https://pugjs.org/) and vue3 logic to implement new stuff.

Use [Volar](https://marketplace.visualstudio.com/items?itemName=johnsoncodehk.volar) VS Code plugin to deal with vue3 code.

### [Capacitor](https://capacitorjs.com/)

> `npx cap add ios` to create ios app folder **for the first time**

1. `npm run build` - to create static html build in `dist` folder
2. `npx cap sync` - to let capacitor sync the build folder with ios folder
3. `npx cap open ios` - to open xcode and start build iOS app

>
> #### document for cap
> - [Installing Capacitor](https://capacitorjs.com/docs/getting-started)
> - [Environment Setup](https://capacitorjs.com/docs/getting-started/environment-setup)
> - [Development Workflow](https://capacitorjs.com/docs/basics/workflow)
