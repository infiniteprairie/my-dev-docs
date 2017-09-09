2017.09.10 
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
- Nodejs and NPM
Details about this last item: While the Software Manager can find an older LTS V4 version to install, and I initially went
this route, it didn't seem satisfactory to use something this old. So I went the route of installing nvm under ~/.nvm, and 
having user-specific binaries for nodejs and its modules. Seems very well put-together in the early going, on a Linux 
machine, so far. If I encounter any of the permissions problems I met before, this time, having a project on hand 
(ci-graph) hopefully will help me to plow through them. That, and better tools and documentation, and a little bit of luck.
