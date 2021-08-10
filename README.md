https://code.visualstudio.com/docs/setup/linux#_visual-studio-code-is-unable-to-watch-for-file-changes-in-this-large-workspace-error-enospc



I came up with a solution on Linux for multiple laravel sail projects.

Create a file named 'php' on /usr/local/bin

sudo touch /usr/local/bin/php
Make it executable:

sudo chmod +x /usr/local/bin/php
Edit the file (with sudo) and paste this code:

path=$(printf '%s\n' "${PWD##*/}")
command="docker exec ${path}_laravel.test_1 php "$@""
echo "Running php on docker ${path}_laravel.test_1"
$command

---
`
command="docker exec php73nginx  php "$@""
echo "Running php on docker php73nginx"
$command
`

# plugin list


* advanced-new-file: not bad
* Angular v7 Snippets: NO
* Amphirion theme(dark)
* Auto Close Tag
* Auto Complete Tag
* Auto Import - ES6, TS, JSX, TSX
* Auto Rename Tag
* Beautify
* Babel ES6/ES7
* Babel JavaScript
* Bracket Pair Colorizer
* Better PHPUnit: OK (alt + T run | alt + G run previous) (https://marketplace.visualstudio.com/items?itemName=calebporzio.better-phpunit)
* Bookmarks
* Bootstrap 4, Font awesome 4, Font Awesome 5 Free & Pro snippets
* Catalan - Code Spell Checker
* change-case
* Code Runner
* Code Spell Checker
* Color Highlight
* Darcula Theme
* Docker Explorer
* Dotenv
* ESLint
* Favorites: OK
* Firebase
* Flow Language Support
* Git Blame
* GitLens — Git supercharged
* HTML CSS Support
* HTML Snippets
* IntelliSense for CSS class names in HTML
* JavaScript (ES6) code snippets
* Laravel Blade Spacer
* Live Server
* Markdown PDF
* Markdown Preview Enhanced
* Material Icon Theme: OK
* Material Theme
* Multiline Tricks
* New Moon Dracula VSCode
* Node.js Modules Intellisense
* npm
* npm Intellisense
* Paste JSON to Code
* Path Intellisense
* PHP Debug
* PHP DocBlocker
* PHP Formatter
* PHP IntelliSense
* PHP IntelliSense Crane
* PHP Namespace Resolver
* -PHPUnit- (Better PHPUnit)
* Prettier - Code formatter
* Settings Sync
* Simple React Snippets
* Spanish - Code Spell Checker
* Spanish Language Pack for Visual Studio Code
* SVG Viewer
* Sublime Material Theme
* Sublime Text Keymap and Settings Importer: OK (https://marketplace.visualstudio.com/items?itemName=ms-vscode.sublime-keybindings)
* Terminal
* TODO Highlight
* TODO Tree
* TypeScript Import
* TypeScript Importer
* Useful React Snippets
* Vscode great icons
* Vscode Google Translate
* vscode-icons
* vscode-pdf
* vscode-spotify
* WakaTime

