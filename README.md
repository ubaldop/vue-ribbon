<p align="center">
  <img src="https://github.com/P3trur0/vue-ribbon/blob/master/assets/logo.png?raw=true" alt="vue-ribbon"/>
  <br/>
  <a href="https://www.npmjs.com/package/vue-ribbon"><img src="https://img.shields.io/badge/npm-1.0.1-blue.svg" alt="Version"></a>
  <a href="https://www.npmjs.com/package/vue-ribbon"><img src="https://img.shields.io/badge/license-MIT-green.svg" alt="License"></a>
</p>

_Did you develop a Vue application hosted on GitHub? Add this Vue component for embedding a GitHub fork ribbon on it!_

---

vue-ribbon is a Vue Single File Component implementing [GitHub ribbons](https://github.blog/2008-12-19-github-ribbons/). It comes with a set of properties making the component customizable for your needs.

### Properties

If you need to customize the ribbon look and feel, you can use the following optional properties.


| Name     | Description                                                                                     | Type      | Default                         |
| -------- | ----------------------------------------------------------------------------------------------- | --------- | ------------------------------- |
| text     | The text to display on the ribbon                                                               | `String`  | _vue-ribbon: check it out!_     |
| url      | The URL linked                                                                                  | `String`  | _https://flatmap.it/vue-ribbon_ |
| position | The position of the ribbon. It can be `right-top`,  `right-bottom`,  `left-top`,  `left-bottom` | `String`  | _right-top_                     |
| fixed    | If defined, it makes the ribbon fixed                                                           | `Boolean` | _false_                         |
| color    | Defines the background color of the ribbon                                                      | `String`  | _#364a5e_                       |

The color of the text is automatically detected by the component: for background color with a luma greater than 128 the text is white, otherwise black.
See how it looks on this [demo](https://flatmap.it/vue-ribbon)!

### Installation
You can install vue-ribbon using npm:

```bash
npm install --save vue-ribbon
```

Alternatively, you can import `vue-ribbon` via `<script>` tag in the browser directly, avoiding the NPM installation:

```html
<script src="https://unpkg.com/vue"></script>
<script src="https://unpkg.com/vue-ribbon"></script>
```

### Usage
Once installed, it is easy to use it.  

#### Importing the component
First, you need to import `vue-ribbon` in your files. You can do that in different ways. For example, it can be imported into a build process for use in full-fledged Vue applications:

```js
import Ribbon from 'vue-ribbon';

export default {
  components: {
    Ribbon,
  },
  // rest of the component
}
```

#### Using the component
Once imported, you can use your component as follows:

```js
<Ribbon/>
```

### Credits
The inspiration for this component comes from [github-fork-ribbon-css](https://github.com/simonwhitaker/github-fork-ribbon-css).

### Contributing
This component can be improved both in features and performances. Please, help in doing it better!