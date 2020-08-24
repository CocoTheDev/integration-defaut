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
mkdir public && mkdir src && mkdir public/styles && touch public/styles/styles.css && mkdir src/styles && touch src/styles/styles.scss && touch public/index.html
```

```
- public
	- styles 
		- styles.css
	- index.html

- src
	- styles
		- styles.scss
	
```
### Package.json
Make sur to add the scss script in package.json
```
"scripts": {
"scss": "node-sass --watch src/styles -o public/styles"
},
```

## index.html
Don't forget the stylesheet head call
```
<link  rel="stylesheet"  href="styles/styles.css">
```

## Run Live server
``` live-server public ```

## Run SCSS script
``` npm run scss ```

## .gitignore
If you go with git flow, don't forget to add these lines:
```
/node_modules
/.sass-cache
```

