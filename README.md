Demo - https://lokeshloki3.github.io/reactjobsvite/

Steps - 

1. Install Node.

2. Install Vite Run command:
	npm create vite@latest projectname 
		Select -
			React
			JavaScript
	cd react-jobs
	npm install

3. Run command:
	npm run dev
  

Setps to Install Tailwind Vite using PostCSS method

4. Run commands for Tailwind:
	A. npm install -D tailwindcss postcss autoprefixer
	B. npx tailwindcss init -p  
	
5. Install tailwind css intellisense extension. [IGNORE IF ALREADY INSTALLED]

6. Add "./index.html', './src/**/*.{js,ts,jsx,tsx}" in content in [ tailwind.config.js ] file.
7. And also extend theme
  theme: {
    extend: {
      fontFamily: {
        sans: ['Roboto', 'sans-serif'],
      },
      gridTemplateColumns: {
        '70/30': '70% 28%',
      },
    },
  },

8. Open src/index.css or src/App.css and insert: 
	@tailwind base;
	@tailwind components;
	@tailwind utilities;

9. Run command to go live:
	npm run dev
	
(Close and again open VS Code for className suggestions)

npm i react-router-dom 
npm i react-icons
npm i react-spinners
npm i react-toastify 

Host Vite Project on github pages -

	npm install gh-pages --save-dev
	
	Add in package.json above name
	"homepage" : "https://username.github.io/reponame"
	
	Add both in Scripts in package.json above dev -
	"predeploy":"npm run build",
	"deploy":"gh-pages -d dist",
	
	Add in vite.config.js above plugin -
	base:"/reponame/",
	
	Add /reponame to Route to render Home in App.json for Github Page
	If wants to change commit in repo first remove homepage url 
	and after committing again write homepage for navbar logo only
	
	git init
	git status
	git add .
	git commit -m "initial commit"
	git branch -M 'main'
	git remote add origin "url of repository"
	git push -u origin 'main'
	
	npm run deploy
	
Just install these if copying my project -

npm i react-icons
npm i react-toastify
npm run dev
