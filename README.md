# Basic Web Notifications
-----
> Create a beautiful Notifications, Messages and Alerts with simple lines of code.

## Installation
 * Download all files then import them in your `index.html`
---
## Usage 
### Import css and js files
-- CSS file
```html
    <link rel="stylesheet" href="path/to/dist/css/notifications.min.css">
```

-- JS file
```html
	<script src="path/todist/js/notifications.min.js"></script>
```

### then add this element before the body closing tag
> Don't forget the `notifiable="enable"` attribute. 
```html
    <div class="whateverClassName" notifiable="enable"></div>
```
---
## In your JS file
```js
    /*
      create a new Notification Instance.
      it takes three parameters className, id or whatever selector 
      Notification Tyoe
      JOSN object called Options
    */
	var notify = new Notification('.whateverClassName', 'type', {
		title: '',
		body: '',
		position: ''
	});
```
---
## Notification Types
* `primary`
* `secondary`
* `success`
* `info`
* `warning`
* `danger`
---
## Notification Postions
* `top`
* `top-left`
* `top-right`
* `bottom`
* `bottom-left`
* `bottom-right`
---

## Show the notification
```js 
    notify.show();
```
## Hide the notification
```js 
    notify.hide();
```
## Notification Methods
```js 
    notify.show();
    notify.showAfter(3000);
    notify.hide();
    notify.hideAfter(3000);
```