# Javascript

You can add arbitrary javascript when rendering the content. If you want the data to be bound to pages automatically, you can use the application.state variable:

```javascript
window.addEventListener('load', function() {
	application.state = {
		"resetPasswordUrl": "http://www.example.com"
	};
});
```

Pages upon rendering will check the application state for variables matched by name, allowing you to fill them in for rendering.