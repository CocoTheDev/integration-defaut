# Defaut folder app, quick landing page integration

## List of dependencies
- npm
- node.js
- live serve
- node-sass
- postscss-cli


## Using this Repo (fast way)
  - ``` git clone https://github.com/CocoThePimp/integration-defaut ```
  
- ``` npm install```  

- ``` npm run scss```  

- ``` live-server public```  

## How to create this app (long way)

### Install
- Create app folder 
- Create app.js
- $ npm init -y
- $ npm install live-server postcss-cli node-sass

### Folders and files
Create folders and files with this command line: 
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

### index.html
Don't forget the stylesheet head call
```
<link  rel="stylesheet"  href="styles/styles.css">
```

### Package.json
Make sur to add the scss script in package.json
```
"scripts": {
"scss": "node-sass --watch src/styles -o public/styles"
},
```

### .gitignore
If you go with git flow, don't forget to add these lines:
```
node_modules
```

## Run Live server
``` live-server public ```

## Run node-sass script
``` npm run scss ```


