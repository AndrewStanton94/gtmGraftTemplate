# GTM graft template

Using babel to create scripts in Google Tag manager.
Also comes with my styling and linting preferences.

## How to use

1. Go to [github.com/andrewstanton94/gtmGraftTemplate](https://github.com/AndrewStanton94/gtmGraftTemplate)
1. Create repo from template
1. Clone it
1. Run `npm init` to generate the package.json file
	- Use [this page](https://spdx.org/licenses/) to get the SPDX licence code. E.g. `GPL-3.0-or-later`
1. Add these sections to the `package.json` file

	```javascript
		"scripts": {
			"build": "babel .js --out-file dist.js"
		},
		"devDependencies": {
			"@babel/cli": "^7.6.4",
			"@babel/core": "^7.6.4",
			"@babel/preset-env": "^7.6.3"
		}
	```
1. Run `npm install` to get dependencies
1. Run `npm run build` to build the file to paste into GTM **Remember to wrap it in a `script` tag**
1. Replace this file with a relevant README
