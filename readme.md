# Making defaut folder for integration

## List of dependencies
- npm
- node.js
- live serve
- node-sass
- postscss-cli

## Instructions
### Install
- Create app folder 
- Create app.js
- $ npm init -y
- $ npm install live-server postcss-cli node-sass

### Folders and files
Create folders and files : 
```
- public
	- styles 
		- styles.css
	- index.html

- src
	- styles
		- scss
			- styles.scss  
	
```
### Package.json
Make sur to add the scss script in package.json
```
"scripts": {
"scss": "node-sass --watch src/styles -o public/styles"
},
```

## Run Live server
``` live-server public ```

## index.html
Don't forget the stylesheet head call
```
<link  rel="stylesheet"  href="styles/styles.css">
```

## .gitignore
If you go with git flow, don't forget to add these lines:
```
/node_modules
/.sass-cache
```

