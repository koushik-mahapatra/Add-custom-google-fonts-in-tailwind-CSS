## Adding custom fonts to a Tailwind CSS project.

- copy the import url of the font and put that on the css file

```CSS
@import url("https://fonts.googleapis.com/css2?family=Bungee+Spice&display=swap");
@tailwind base;
@tailwind components;
@tailwind utilities;
```

- add the font name inside fontFamily object to `tailwind.config.js` file like this ⬇

```js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["*.{html,js}"],
  theme: {
    extend: {},
    fontFamily: {
      bungee: ["Bungee Spice", "sans-serif"],
    },
  },
  plugins: [],
};
```

- use the font like this ⬇

```html
<p class="font-bungee">this paragram written with a bungee font.</p>
```
