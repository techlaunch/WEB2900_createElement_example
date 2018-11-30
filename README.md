# WEB2900_createElement_example
Show an example of a simple createElement() implementation using React

# Step by step 

## 1) Create the following HTML


```html
<html>
	<header>
		<title>Create Element example</title>
	</header>
	<body>
		<div id="root"></div>
	</body>
</html>
```

## 2) Include Reach via CDN

```javascript
<script src="https://unpkg.com/react@16.0.0-rc.3/umd/react.production.min.js"></script> 
<script src="https://unpkg.com/react-dom@16.0.0-rc.3/umd/react-dom.production.min.js"></script>
```

## 3) Create an element, add it to the class "container"

```javascript
<script type="text/javascript"> 
	const rootElement = document.getElementById('root'); 
	const element = document.createElement('div'); 
	element.textContent = 'Hello World';
	element.className = 'container'; 
	rootElement.appendChild(element);
</script>
```

## 4) Add styles, see what happens

```css
<style type="text/css">
	.container{
		color: red;
		font-size: 40px;
	}
</style>
```

# The entire code 

```
<html>
	<header>
		<title>Create Element example</title>
		<style type="text/css">
			.container{
				color: red;
				font-size: 40px;
			}
		</style>
	</header>
	<body>
		<div id="root"></div>

		<script type="text/javascript"> 
			const rootElement = document.getElementById('root'); 
			const element = document.createElement('div'); 
			element.textContent = 'Hello World';
			element.className = 'container'; 
			rootElement.appendChild(element);
		</script>

		<script src="https://unpkg.com/react@16.0.0-rc.3/umd/react.production.min.js"></script> 
		<script src="https://unpkg.com/react-dom@16.0.0-rc.3/umd/react-dom.production.min.js"></script>
	</body>
</html>
```
