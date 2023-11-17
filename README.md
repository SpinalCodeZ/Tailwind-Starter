# Tailwind-Starter
 Starter Tailwind-Project



    God Loves You!

    Matthew 6:26


    Here is a sample landing page using Tailwind CSS. If you dont have Tailwind ready to use just go to the Tailwind site (tailwindcss.com) and follow instructions. Make sure to have node.js installed. If you want to copy my page and stuff then you would use npm run dev to compile the projects. I used Devtamin's tutorial on youtube to learn the setup.

    lets do this step by step:

    first install the "Tailwind CSS IntelliSense" extension and the "open in browser" or "live server" extension

    make a new project in VS Code
    open a new terminal
    type node-v to ensure node.js is installed
    type npm innit (hit enter dont fill stuff until you know what your doing. this creates your package.json)
    type npm install -D tailwindcss (this will be the start to setting up everything with tailwind)
    type npx tailwindcss init (this creates the tailwind.config.js)
    create a folder named dist and inside add an index.html file
    in the tailwind.config.js add "./dist/*.{html,js}" inside the content brackets ("./src/**/*.{html,js}" to fit our project)
    add a new folder named src and inside add an input.css file
    inside the input.css file type 
        @tailwind base;
        @tailwind components;
        @tailwind utilities;
    back into the terminal type npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
    this will create an output.css file in your dist folder
    edit html with a link to your output.css file and custumize your html using tailwind css
    right click your html file and run in live server or browser (depending on extension) you should see your page
    ctrl c, then y to terminate batch job
    now in your package.json file edit to look like this
        "test": "echo \"Error: no test specified\" && exit 1",
        "dev": "tailwindcss -i ./src/input.css -o ./dist/style.css --watch"

        all you did here was add the dev under the test. by doing this you can start your program easier
    in the terminal type npm run dev
    right click your index.html and run in live server or browser (depending on extension) it should still work

    i changed my output.css file to style.css you can change it to whatever you want by going to package.json
    change the dev line you made earlier to 
        "dev": "tailwindcss -i ./src/input.css -o ./dist/style.css --watch" (notice we canged the output to have style.css)
    now in your html change the css link so it linkes to style.css
    ctrl c and y to terminate bash job
    in terminal npm run dev to resart the program and see the newly added style.css file in the dist folder
        you can delete the output.css folder since your not using it anymore
    you can keep editing your html and testing it in your live server or browser (depending on extension)

    have fun!
