# Angular Unique Slug Generator Pipe

This is an Angular repository with a playground of an Angular Pipe for generating slug from an string of characters, it supports English & Spanish Characters and also comes with unique slug options which makes sure you are generating an unique slug for your app.

>If you want to see a demo with all this code checkout my [demo on Stackblitz](https://stackblitz.com/edit/angular-slugify-pipe?file=src/app/slugify.pipe.ts)

## How to use it?

Just create a pipe like slugify.pipe.ts file which is right in the src/app directory. Maybe I realease a library with that tool, I'm not sure yet. Then just use it as the following e.g.:

```html
<span class="content">
  {{ 
    content | slugify: {
      unique: true,
      uniqueOptions: { <!-- OPTIONAL -->
        randomLength: 6,
        chars: ['lowercase', 'numeric'],
        separator: '-'
      }
    }
  }}
</span>
```

The slugify itself does not generate an unique slug but if you enable the unique property then you will be shown with its default settings, if you would like to have custom settings then add uniqueOptions object (this is optional), setting up the randomLength, chars combination and the slug separator.

Before Pipe:

`¡Este artículo habla sobre Angular y sus slugs potentes!`

After Pipe:

`este-articulo-habla-sobre-angular-y-sus-slugs-potentes-dgaode`

## TODO
- [ ] Publish a npm library

## Author 
**Ruslan Gonzalez**
* Github: [Profile](https://github.com/ruslanguns)
* Website: [https://rusgunx.tk](https://rusgunx.tk)
* Twitter: [@ruslangonzalez](@ruslangonzalez)