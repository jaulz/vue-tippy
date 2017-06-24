# vue-tippy

> Directive wrapper for Tippy.js

## Install

#### Available through npm as `vue-tippy`.

  ``` js
  var vueTippy = require('vue-tippy')
  Vue.use(vueTippy)
  ```

## Usage

#### Using the `v-tippy` directive

#### Basic
```html
<button title="Hi!" v-tippy> My Button! </button>
```
#### Bind title
```html
<button :title="dynamicTitle" v-tippy> My Button! </button>
```

#### Popper HTML
```html
<button data-html="#contentpopup" v-tippy> My Button! </button>
```
```html
<div id="contentpopup" style="display: none">
        <div>
            <h3> Header</h3>
            <p style="color: black"> {{ message }} - data binding </p>
            <p style="color: black"> {{ clicks}} click(s) </p>
        </div>
 </div>
```

#### Vue component
```html
<button data-html="#comppopup" v-tippy> My Button! </button>
```
```html
<vue-component-test style="display: none" id="comppopup"></vue-component-test>
```
## License

[MIT](http://opensource.org/licenses/MIT)