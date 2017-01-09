#The MoFed Intern Starter Doc

Welcome to the team! As an intern on the CSP Front End team (we call ourselves MoFed, for Mormon Front End Developers), we want you to grow as much as possible and contribute as well. This starter kit will outline your first set of projects and will allow us to evaluate where you're at. It will also give you the opportunity to learn and to build out tools that will help the rest of the team.

Before starting here, you should have already gone through the [Getting Started Guide](https://github.com/teamMoFed/docs/blob/master/gettingStarted.md). Your computer and environments should be set up and ready to go. If that hasn't happened yet, start there.

##Project 1: DevTest
All employees of MoFed take our DevTest as part of the interview process. This allows us to evaluate their skill level and gives us insight into their coding style and experience level. We'd like you to take this test for those same reasons, but additionally to strengthen your front end dev skills.

The DevTest is located [here](https://github.com/teamMoFed/devtest). Please read through all of the instructions and follow the instructions for the 'Lead and Above' task level. This will give you maximum exposure to the type of work we do.

###Items to keep in mind while completing the DevTest:

* Understand the requirements. You are encouraged to ask questions. Start by doing some resarch on your own. If you're at all stumped or if you have question regarding process or methodology, such as "What are you looking for here?", ask coworkers and team leads for help at any time. You have great resources around you. Please utilize them.
* Our stack consists of Node.js, React, Redux and PostCSS. If you're new to React and Redux, you're not required to use them for this test. Use what you know but plan on diving into React and Redux in the near future.
* Use CSS Variables (native, not via preprocessor). Browser compatibility is not our focus for this test.
* Develop mobile first. You aren't provided with mobile designs but you're expected to develop mobile first. Welcome to CSP.
* Make your code as reusable as possible (Always think with a component mindset)
* Write in vanilla JS - no jQuery or other such libraries
* Leverage ES6+ as often as it makes sense

This is meant to be a challenging but fun experience. Try to have fun with it and see how much you can learn.

##Project 2: Internal Project

For your next project, we'd like you to work on a tool or service that would benefit the other front end developers. You'll want to check with your manager for details on this but you'll likely be starting with one of the projects on this list:

* **[LDS Placeholder](https://design.ldschurch.org/csp/placeholder)** - This is an internal image service, similar to Lorem Pixel, where a developer can select a category and image size to use in their development. The benefit is that all of the images provided here are hand picked to be appropriate and relevant to the church. This service was written in PHP several years ago and used image_moo.php to handle the bulk of the work. The home page for the service was reskinned in mid 2016 but the whole service could benefit from being written in React and using modern CSS and Javascript. NPM modules are fine to use. The repo for this is located on [bitbucket in CSPFED](https://code.ldschurch.org/git/projects/CSPFED/repos/placeholder/browse).
* **Language Files for Lumen SCSS** - At one point, a language spreadsheet was created using Google Docs that contains charatecteristics of all of the languages that we support. This spreadsheet, unfortunately, was created in Google Docs and is used as part of a compilation process that outputs a series of .scss files. The file that processes the spreadsheet is called languages.js. This whole process ought to be overwritten to use our local/supported resources rather than Google Docs. The [author's notes](https://docs.google.com/document/d/1FsTKhJKJOhSEor_OQDVN-uCguFqBzNl8_4JxSi5Pp5w/edit#) on this process as it works today are as follows: "[Styling LDS.org Languages](https://docs.google.com/spreadsheets/d/1iln-6bG3IgWKriY6F7z9ROCcG6P-1fdLDmXNFT6PMaw/edit#gid=0) - This spreadsheet is what is used for the javascript utilties in [Lumen SASS](https://code.ldschurch.org/git/projects/LUMEN/repos/lumen-sass/browse). Update the spreadsheet, and run the languages.js utility within the lumen sass project and it will output new [lang].scss files for all languages that can be consumed by projects that need them.  You just save the changes into lumen-sass and they update that component to get the latest language updates."
* **More projects should be added to this list**

##Project 3: Production Product Work

For the remainder of your time as an intern, we'd like you to work with your team or other teams in the portfolio to do actual project work that will likely be headed for production. You'll work with the MoFed manager and team leads to determine where your time can best be spent to benefit the work as well as yourself. Remember to regularly check in with your coworkers to make sure you're on the right track and always submit pull requests so that your code can be reviewed by others - just like we all do.

##Helpful Information
You may find the following information helpful as you navigate the waters of church employment.

* You are a part of the Communication Services Portfolio (CSP), which is one of the portfolios in Information Communication Services (ICS). ICS is made up of most everyone in the Riverton Office Building (ROB) but we work with other teams, like Publishing  Services Department (PSD) and others.
* CSP is broken up into several teams. Each team has a different set of projects that they have ownership over. Each team has an assigned Team Lead, Assistant Team Lead and a Project Manager (PM) and Solutions Manager (SM). The PM and SM may have stewardship over more than one team. The portfolio also has a Portfolio Director (PD), who is Ron Stutz.
* The MoFed team consists of all front end developers in CSP. We have a front end Manager, Colt Pini, who is our employment manager. In other words, he's the one who defines the direction that the front end takes and oversees training, technology and HR matters. Nils Rasmusson is the assistant front end manager and there are several front end team leads who help provide direction for their teams of front end developers. 

That's it! Always feel free to ask any of us if you have questions and we'd especially love to hear your feedback on our processes and how we work in general. If you think there's a better way to do something, don't by shy! We want to serve in the best way we can and will adapt where possible. Not all decisions are in our hands but if we can improve, let's!
