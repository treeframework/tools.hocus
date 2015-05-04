# hocus

Generate `:hover` and `:focus` styles in one go.

If you install the `hocus` module using Bower or npm, you will get these 
dependencies at the same time. If not using Bower or npm, please be sure  to 
install and `@import` these dependencies in the  relevant way.

## Installation

You can install the `hocus` module via Bower, npm, or copy and paste.

### Install using Bower:

```sh
$ bower install tree-hocus --save
```

Once installed, `@import` into your project in its Tools layer:

```scss
@import "bower_components/tree-hocus/tools.hocus";
```

### Install using npm:

```sh
$ npm install tree-hocus --save
```

### Install via file download

The least recommended option for installation is to simply download 
`_tools.hocus.scss` into your project and `@import` it into your  project in 
its Tools layer.

## Usage

Basic usage of the `hocus` module:

```scss
a {
    text-decoration: none;

    @include tree-hocus() {
        text-decoration: underline;
    }

}
```

This will yield:

```css
a {
    text-decoration: none;
}

a:hover,
a:focus {
    text-decoration: underline;
}
```

## Credits

* **[inuitcss](https://github.com/inuitcss)** Powerful, Sass-based, OOCSS
framework designed with scalability and performance in mind.
