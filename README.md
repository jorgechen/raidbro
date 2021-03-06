# [RaidBro](http://jorgechen.github.io/raidbro) - WoW Raiding Tool

This is a simple tool for guilds to analyze its raiders.  RaidBro provides up-to-date info on your guild, such as a raider's attendance and the gear received since the past weekly reset.


## Installation

RaidBro is made for the community. Feel free to fork the project and use it to help you.  With whatever new ideas you think of, giving credit to me is appreciated!

After cloning the repository, install dependencies:
```
git clone https://github.com/sylvanknave/raidbro.git
cd raidbro
npm install
```

Run the local server:
```
npm start
```

Currently the front-end is a GitHub Page, which means we need to commit the items to the gh-pages branch of the repository.
```
cd raidbro
npm start
(CTRL + C)
cp build/* ./
git add ...
git commit ...
```


#[Gulp](https://github.com/gulpjs/gulp) Plugins


##[browserify](https://github.com/substack/node-browserify)
Browsers do not allow us to use the require method from Node.js. With browserify, we can implement dependency management on the browser. It also will bundle the code into one file in an efficient way to not repeat dependiencies that are used more than once.

##[browserSync](http://www.browsersync.io/)
When developing and testing the website, browserSync is a powerful tool that will rebuild and refresh the webpage so you can see the changes you make as you are working.

##markup
Copies all of the files from /src/www to the build folder.

##[gulp_starter](https://github.com/greypants/gulp-starter)
A useful repository that explains how many of gulp's features work and contains an example project to get familiar with it. We use this example to construct our own project.


## Notes

Sometimes when we add new links, we gotta refreshLinks()
- http://www.wowhead.com/forums&topic=227864/dynamic-wowhead-tooltips

Installing NodeJS on Ubuntu
- https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager#debian-and-ubuntu-based-linux-distributions
- http://www.hostingadvice.com/how-to/install-nodejs-ubuntu-14-04/
