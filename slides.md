---
fonts:
  sans: Open-Dyslexic
  local: Open-Dyslexic
# try also 'default' to start simple
theme: light-icons
# apply any windi css classes to the current slide
class: "text-center"
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
# page transition
transition: fade-out
# use UnoCSS
css: unocss

layout: intro
image: https://images.unsplash.com/photo-1495401220594-550313c3046b?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2064&q=80
---

<div v-click class="mb-4 absolute bottom-4 left-12 text-left">
  <span class="text-6xl text-primary-lighter text-opacity-80 font-medium" >
    Utility first CSS
  </span>
  <div class="text-9xl text-white text-opacity-60 font-bold" >
    TailwindCss
  </div> 
</div>

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page <carbon:arrow-right class="inline"/>
  </span>
</div>

---

# What is tailwind

Tailwind is a utility first css framework which generates simple atomic classes, so you can style apps quickly without sacrificing _much_ customizability

<img v-click src="/img/LibrariesSummarised.png" class="w-128" />

---

# What is tailwind

With tailwind, insead of using semantic class names to style your markup,

you use atomic class names which represent properties.

<div class="grid grid-cols-2">
  <div>
    <p>So insead of this</p>
    <img v-click class="h-80" src="/img/Non-TailwindCard.png" />
  </div>
  <div>
    <p>You do this</p>
    <img v-click src="/img/TailwindCard.png" />
  </div>
</div>

---

# Looking at this makes me feel ill

<img src="/img/InsaneTailwind.png" class="w-256 mb-4" />

<div class="flex justify-center">
  <div v-click class="text-left flex flex-col items-end">
    <p class="w-128 me-2 italic">
      If you can suppress the urge to retch long enough to give it a chance, I really think you’ll wonder how you ever worked with CSS any other way.
    </p>
    <Quote/>
  </div>
</div>

---

# Common issues with tailwind

That is an extreme example, but lets look at some issues with tailwind

## Issues

- Classlist gets long and hard to read
- Hard to reuse code
- Delivering too much CSS when app gets large

<v-click>

## Solutions

- Use the `prettier` tailwind plugin, and use the `inline-fold` vscode extension
- Build reusable react `primitive` components
- JIT Mode (Render only the CSS you need, only when you need it)

</v-click>

---

# Keem's experience

<br/>

## Things I Loved

1. James is Tailwind God and he bestowed his blessing upon us
2. SPEED - instant gratification
3. UTILITY - Padding, hover states, custom components

<br/>

## Things To Consider

1. How much is too much?
2. Still need css modules in specific cases - Grid Area/Layouts

---

## Before

<img src="/img/accordionBefore.png" width="350" height="150">

---

## After

<img src="/img/accordionAfter.png" width="850" height="550">
