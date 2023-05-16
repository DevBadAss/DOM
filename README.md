# DOM Manipulation Library

A JavaScript library for DOM manipulation, providing a convenient way to interact with HTML elements.

## Introduction

The `DOM Manipulation Library` is a lightweight and easy-to-use JavaScript library that simplifies DOM manipulation tasks. It provides a set of methods to query, modify, and interact with HTML elements using their IDs or class names.

### Import as a module

```javascript

import DOM from 'path/to/dom.js';

```

## Usage

### Instantiate the DOM module

```javascript

 const dom = new DOM();

```

### Querying Elements

The library provides methods to select and query elements in the DOM.

`select(query)`

This method queries and selects an element by its ID or class name.

```javascript

const element = dom.select('myElement');

```

`select_all(query)`

This method queries and selects all elements by their ID or class name.

```javascript

const elements = dom.select_all('myElements');

```

### Getting and Setting HTML

You can retrieve and modify the HTML content of elements using the following methods.

`get_html(selector)`

This method returns the inner HTML content of the selected element.

```javascript

const html = DOM.get_html('myElement');

```

`set_html(selector, html)`

This method sets the inner HTML content of the selected element.

```javascript

dom.set_html('myElement', '<p>New content</p>');

```

`add_html(selector, html, pos)`

This method adds HTML content to the selected element at a specified position.

```javascript

dom.add_html('myElement', '<span>Additional content</span>', 'beforeend');

```

### Modifying Classes

You can add or remove CSS classes from elements using the following methods.

`add_class(selector, className)`

This method adds a new CSS class to the selected element.

```javascript

DOM.add_class('myElement', 'newClass');

```

`remove_class(selector, className)`

This method removes a CSS class from the selected element.

```javascript

dom.remove_class('myElement', 'oldClass');

```

### Removing Elements

You can remove elements from the DOM using the following method.

`remove(selector)`

This method removes the selected element from the DOM.

```javascript

DOM.remove('myElement');

```

### Handling Events

The library provides methods to handle various events on elements.

`click(selector, callback)`

This method attaches a click event listener to the selected element.

```javascript

dom.click('myElement', (evt) => {

    // Event handler code

});

```

`dblclick(selector, callback)`

This method attaches a double click event listener to the selected element.

```javascript

dom.dblclick('myElement', (evt) => {

    // Event handler code

});

```

`mousemove(selector, callback)`

This method attaches a mouse move event listener to the selected element.

```javascript

dom.mousemove('myElement', (evt) => {

    // Event handler code

});

````

`touchstart(selector, callback)`

This method attaches a touch start event listener to the selected element.

```javascript

dom.touchstart('myElement', (evt) => {

    // Event handler code

});

```

`touchmove(selector, callback)`

This method attaches a touch move event listener to the selected element.

```javascript

dom.touchmove('myElement', (evt) => {

    // Event handler code

});

```

`touchend(selector, callback)`

This method attaches a touch end event listener to the selected element.

```javascript

dom.touchmove('myElement', (evt) => {

    // Event handler code

});

```

## Authors

- [@DevBadAss](https://www.github.com/devbadass)

## License

This project is licensed under the [MIT Licence](https://choosealicense.com/licenses/mit/)

