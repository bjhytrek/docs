#Setup PHP/CDN Stuff for ldsorg

##This information now lives at: [php-cdn-setup](https://github.com/teamMoFed/docs/blob/master/php-cdn-setup)

##Make folders
Clone repos
Things to know
Where to go
gulp stuff
git branching model
CDN
source/prototypes
Make folders
`cd ~/`
`mkdir Sites`
`mkdir Sites/cdn2`
`mkdir Sites/csp`
`mkdir Sites/cdn2/csp`

* Copy the **barkeraj.conf** file into **macintosh HD > private > etc > apache2 > users**
In barkeraj.conf change instances of “barkeraj” to your own username

* **macintosh HD > private > etc > apache2** folder open **httpd.conf** in sublime and uncomment out line 493 (Include **/private/etc/apache2/extra/httpd-userdir.conf**)

* in **extra/httpd-userdir.conf** comment out line 10
**UserDir Sites**
uncomment line 16
Include `/private/etc/apache2/users/*.conf`

##Clone repos

**ldsorg prototypes**
`cd ~/Sites/csp/`
`git clone --recursive https://code.ldschurch.org/stash/scm/CSPFED/repos/ldsorg/.git`
`cd ~/Sites/csp/ldsorg/`
*currently using node 0.12.7, install npm and bower stuff*
`npm i`
`bower i`
*--recursive* adds a submodule that is needed.  If you already have cloned the directory, use the following to add the submodule:
`cd ~/Sites/csp/ldsorg/
git submodule update --init --recursive`

**platform stuff**
`cd ~/Sites/csp/`
`git clone https://code.ldschurch.org/git/scm/cspfed/platform.git `

**placeholder stuff**
`cd ~/Sites/csp/`
`git clone https://code.ldschurch.org/git/scm/cspfed/placeholder.git`

**ldsorg CDN stuff**
`cd ~/Sites/cdn2/csp`
`git clone https://code.ldschurch.org/git/scm/ldscdn/ldsorg.git`

**platform CDN stuff**
`cd ~/Sites/cdn2/csp`
`git clone https://code.ldschurch.org/git/scm/ldscdn/platform.git`
**common CDN stuff (jQuery, etc)**
`cd ~/Sites/cdn2/csp`
`git clone https://code.ldschurch.org/git/scm/ldscdn/common.git`

##Things to know##
**Restart apache**
`sudo apachectl restart`

**Stop apache**
`sudo apachectl stop`

**Start apache**
`sudo apachectl start`

**Logs**
`cd /var/log/apache2/`

##Where to go

* Ldsorg prototypes: [http://localhost/csp/ldsorg/](http://localhost/csp/ldsorg/)
* Platform stuff: [http://localhost/csp/platform/ ](http://localhost/csp/platform/)

##gulp stuff

When editing folder/project specific stuff (home, temples, etc)
`gulp watch --folder [[foldername]]`

When editing a differently named file inside of a folder (strata inside of home)
`gulp watch --folder [[foldername]] --file [[filename]]`

When doing shared CSS files run the respective command depending on what you are editing
`gulp ldssass:common`
`gulp ldssass:lang`
`gulp ldssass:pages`

When doing shared JS files run the respective command depending on what you are editing
`gulp ldsscript:common`
`gulp ldsscript:pages`

##git branching model

##CDN
branch from master into feature/[[featureName]]
PR from your feature branch into dev/test/stage/master
after you merge into master, delete the feature branch

##source/prototypes
branch from master into feature/[[featureName]] (should match CDN feature branch if doing CDN-specific changes)
PR from your feature branch into master once your equivalent CDN branch has made it to master
after you merge into master, delete the feature branch

##https version of pages
This worked for me but did require a few minor tweaks as I was going through (we have a different path for file location, etc
https://gist.github.com/jonathantneal/774e4b0b3d4d739cbc53 