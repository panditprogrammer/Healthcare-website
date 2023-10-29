# SETUP Tailwind CSS via CLI
This installation is required NodeJS. Make sure you have already installed nodeJS. Nodejs will be used for only installation of tailwind css.
1. Create two directories "dist" and "src".
2. In "dist" directory create an "index.html" file.  
3. In "src" directory create an input.css file for tailwind css 
4. Run this command in Root of Project
```
npx tailwindcss init
```
It will create a configuration file for tailwind css.

5. Edit "tailwind.config.js" and add content directory path. (*.* for all types of files)
```
module.exports = {
  content: ["./dist/index.html"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

6. Add some tailwind CSS classes in your "index.html" file.
7. Run this command in root of project
The flag '-i' for input file path and '-o' for output file path
```
npx tailwindcss -i ./src/input.css -o ./dist/style.css
```
After running this command "style.css" file will be created.
8. Link "style.css" file with "index.html".
9. You are ready to go!.
But wait a minute, Your tailwind css class changes may not reflect on browser. you have to rerun the command as mentioned in step (7).

IMPORTANT: You can use this flag with that command for continue watching changes on your files.
```
npx tailwindcss -i ./src/input.css -o ./dist/style.css --watch
```
10. Now you can Design and develop your web application smoothly without worrying about run command.

For more information about installation of tailwind css you can visit the official web documentation here [Tailwind CSS Docs](https://tailwindcss.com/docs/installation).