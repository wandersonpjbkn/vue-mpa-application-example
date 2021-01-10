# Building a MPA application

Setup is pretty easy. The main part is in `vue.config.js`, which is where you will write the guidelines for Vue to compile the application as a multi-page application.

Here, I take the example of separating folders into:

- `assets`: any extra files
- `components`: `.vue` components
- `pages`: set of directories with the pair `page.vue` and `page.js`, where `page.vue` would be the view of the page you want to create and `page.js` the JS instructions for this page.

Note that if you do a standard installation of CLI VueJS, there will be the pair `App.vue` and `main.js`. The set of pages I mentioned above, is exactly this pair, repeating itself for each new page you need - including here, I still keep those names.

As I mentioned above, the entire configuration is actually found in `vue.config.js`, in the `pages` property.

This is where you will register all pages and their data:

- `entry`: main JS file (aka `main.js`)
- `template`: template that this page will use. Here, you can feel free to explore multiple templates and connect them at will to your pages.
- `title`: the title / name of this page
- `chunks`: if you want to name this page

After that, everything is exactly like the normal CLI, and can be customized at will.

## Disclaimer

I would like to take this space to explain some points:

- I am not an expert or experienced in programming or VueJS
- It turns out that I needed to develop an application using the concept of multi-page, but I found myself lost in the official explanation on the VueJS website
- I also didn't find good references on the internet or on StackOverflow, about how to really configure this application
- After some time reading and trying, I was finally able to configure - although it is nothing really abnormal
- So, when I came across the question on StackOverflow, asking the same question that I had, I understood that it would be cool to provide an answer as I would have liked to find back there
- And this is what this repository is: a very practical answer on how to configure multi-page in VueJS

## Project setup

### Install

``` bash
npm install
```

### Compiles and hot-reloads for development

``` bash
npm run serve
```

### Compiles and minifies for production

``` bash
npm run build
```

### Run your tests

``` bash
npm run test
```

### Lints and fixes files

``` bash
npm run lint
```

### Customize configuration

See '[Configuration Reference](https://cli.vuejs.org/config/)' on VueJS CLI Official Website.
