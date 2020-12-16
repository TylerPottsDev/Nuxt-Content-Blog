---
title: My second blog post
description: Welcome to my second blog post using the content module.
slug: second-post
img: blog-2.jpg
---

# Mastering VueJS
### My learning notes on Vue (version 3)

## Installation Types

- CDN
- NPM
- CLI (_Preferred_)
- Vite

### CLI Installation
The `cli` installation is easy but requires prior knowledge of `NodeJS`.

Installing the CLI is as easy as running the following command in your terminal (requires node/npm to be installed).

``` sh
yarn global add @vue/cli
# OR
npm install -g @vue/cli
```

---

## Introduction

Vue is a progressive framework for building user interfaces. Unlike other monolithic frameworks, Vue is designed from the ground up to be incrementally adoptable.

Personally, Vue is the _easiest_ frontend framework / library to learn.

Vue uses __declarative rendering__, this means that it can render data to the DOM using _standard_ HTML template syntax such as;

```html
<div id="block">
  <h1>Hello, World!</h1>
</div>
```

Using Vue you can create links between the data and the DOM for example if we have a `prop` or a variable in our `<script></script>` tag and this is updated the DOM will react and update to match the new data.

---

## Directives

Vue uses html `attributes` known as __directives__ `e.g. 'v-on'`. Directives can attach event listeners that invoke methods in our instances. See example below;

```html
<div id="event-handler">
  <h2>Welcome</h2>
  <button v-on:click="doSomething">Click me</div>
</div>
```

The above snippet tells Vue to run the method `doSomething` when the button is clicked. The method is declared in the `<script></script>` tags under `methods` or more recently using the Vue composition API's `setup` method.

There is more directives than `v-on`, for example you can also use `v-model` to bind data to an DOM element or use `v-if` to conditionally render an element. There is a lot more too what you can find scattered around the [Vue Website](https://v3.vuejs.org/guide/).

On top of the existing directives you can also create your own custom directives. [Find out more here](https://v3.vuejs.org/guide/custom-directive.html#intro).


