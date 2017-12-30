#### _2017.12.30_
Still (slowly) plowing through the JS concurrency book, Kyle Simpson's [Asynch & Performance](https://github.com/getify/You-Dont-Know-JS/blob/master/async%20%26%20performance/README.md). Good so far. Just discovered the github repo for it in writing this note -- hoping to get some more usable (i.e., actually executable) code samples out of this discovery.

Re-installed an Ubuntu chroot image on my ASUS Chromebook. The old one, for some reason was not working. Not a huge pain, as I didn't have that much installed on top of the base image (AFAIK). The initial install is *very* bare bones. This is sort of nice for Chromebooks due to the lack of disk space. I first had to install (using apt-get) a window manager, [kwin]( https://en.wikipedia.org/wiki/KWin). That shows how bare-bones the chroot image is. It's not clear whether there's any merit in doing serious dev work on the Ubuntu image, but it will be a good exercise to find out. Perl and Python are there, out of the box -- as they are with lots of other Linux desktop builds.

What follows is a minimal stack of developer tools:
1. Atom (editor)
2. git client
3. NodeJS and NPM * with a TBD base set of libraries
4. Java 8 * with a TBD base set of libraries
5. Docker
6. chromium
7. Password Safe
8. An adequate build ecosystem
9. A tool that can bootstrap a dev environment with all (or a selected subset) of the above

__What's the plan?__
For 2018, the plan is the following
1. To stand up the above dev environment in a repeatable and archivable way, so that if dev environment _X_ gets blown away, it can be resurrected quickly and painlessly. For the occasional or sporadic developer like me, this seems essential
2. Finish the JS book, and probably write up some quick notes on the major takeaways
3. Resurrect the ci-graph project, focusing on adding a database, web-enabling it, and splitting it up into microservices
4. Learn how to build and deploy Docker application container instances
5. Build and deploy ci-graph as a set of application containers


#### _2017.09.10_ 
Just re-read the diary from 2015. The Express stuff looked like a major pain... not sure it's worth revisiting in 
the form that it was in 2+ years ago. 

A number of things have happened since the 2015 time frame.

First, I developed a working version -- sans database (i.e., with a static data structure[s]) -- of a JS application called 
"ci-graph", with no UI. I would like to flesh that out with a web UI and a real database. First I want to understand whether 
a Mongo DB is appropriate still, and whether the tools built on top of Express have improved. 

Next, I ordered a book on JS concurrency and non-blocking IO [from the "You Don't Know Javascript" series].  Looking forward 
delving into that, and hopefully applying the learnings there to the above project.

Finally, I've now got a Debian Linux machine! I "found" an older Lenovo ThinkPad X1, so I wiped it, and installed Linux Mint 
"Sonya" on it. Strictly speaking this wasn't entirely necessary, but it sure makes for more comfortable and functional user 
experience using this TPX1 as a dev machine. So far, installation has been limited to the typical stuff (for me): 
- Password Safe
- Chromium
- Java 8
- NodeJS and NPM

*Details about this last item (NodeJS and NPM)*: While the Software Manager can find an older LTS V4 version to install, and I initially went this route, it didn't seem satisfactory to use something this old. So I went the route of installing nvm under ~/.nvm, and having user-specific binaries for nodejs and its modules. Seems very well put-together in the early going, on a Linux 
machine, so far. If I encounter any of the permissions problems I met before, this time, having a project on hand 
(ci-graph) hopefully will help me to plow through them. That, and better tools and documentation, and a little bit of luck.
