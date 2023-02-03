# Multiple Entries

You can split your slides.md into multiple files and organize them as you want using the `src` attribute.

#### `slides.md`

```markdown
# Page 1

Page 2 from main entry.

---

## src: ./subpage.md
```

<br>

#### `subpage.md`

```markdown
# Page 2

Page 2 from another file.
```

### `Keem'sExperience.md`

###

My Experience of Tailwind:

## Good

1. At first I was opposed to bloating HMTL with css classes, as it felt reminiscent of in-line styling, however, it actually became EASIER and FASTER to keep track of scss
   instead of handling with scss modules for every component.
2. Tailwind comes with useful extensions for your IDE, such as the Tailwind Intellisense plugin that gives you autocompletion, linting for errors, and a hover preview to show
   what that class is applying.
3. Speed, Tailwind's utility classes are very versatile and prevent the need for creating unecessary names to apply a padding 1rem
4. Tailwind's utility classes handle pseudo elements, classes and hover/focus states which proved very useful when creating custom components - React-select

## Bad

1. Markup can get cluttered with classes, so we'd need an agreement on how many is too much. However, I did have a potential solution when using clsx to place each classname
   in its own index as CSVs that can be neatly ordered instead of one giant string - we could create an npm that would join these indexes as one giant string behind the scenes

Grid areas are still are not available, instead use
For Layouts we would still use SCSS modules to setup, since we can defined Grid Areas by name

[Learn more](https://sli.dev/guide/syntax.html#multiple-entries)
