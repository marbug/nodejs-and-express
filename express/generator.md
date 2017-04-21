# Express - Generator #

## Install generator ##

Use the application generator tool, express-generator, to quickly create an application skeleton.

The express-generator package installs the express command-line tool. Use the following command to do so:

    npm install express-generator -g

## Help ##

Display the command options with the -h option:

    express -h

You'll see something like:

    Usage: express-cli [options] [dir]

    Options:

      -h, --help           output usage information
          --version        output the version number
      -e, --ejs            add ejs engine support
          --pug            add pug engine support
          --hbs            add handlebars engine support
      -H, --hogan          add hogan.js engine support
      -v, --view <engine>  add view <engine> support (dust|ejs|hbs|hjs|jade|pug|twig|vash) (defaults to jade)
      -c, --css <engine>   add stylesheet <engine> support (less|stylus|compass|sass) (defaults to plain css)
          --git            add .gitignore
      -f, --force          force on non-empty directory

## Generate app ##

For example, the following creates an Express app named **myapp**. The app will be created in a folder named **myapp** in the current working directory and the view engine will be set to [Pug](https://pugjs.org/):

    express --view=pug myapp

or try something like:

    express --view=dust my-dust-app
    express --view=ejs my-ejs-app
    express --view=hbs my-hbs-app
    express --view=hjs my-hjs-app
    express --view=jade my-jade-app
    express --view=pug my-pug-app
    express --view=twig my-twig-app
    express --view=vash my-vash-app

## Install dependencies ##

    cd myapp
    npm install

## Run the app ##

On MacOS or Linux, run the app with this command:

    DEBUG=myapp:* npm start

On Windows, use:

    set DEBUG=myapp:*
    npm start

Then load [http://localhost:3000/](http://localhost:3000/) in your browser to access the app.

## Useful links ##

[Express Getting Started](http://expressjs.com/en/starter/generator.html)
