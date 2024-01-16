# December 28, 2023

## Main Achievements
1. **Started working on Flask implementation of my dog listing application**

## Learning Milestones
- First experience with Flask.
- 
- Learnt a bit about rollup for js libraries and tree-shaking.

# December 30, 2023

## Main Achievements
1. **Started working on the C++ implmentation of my dog listing application**
2. **Kept working on the Flask implementation of my dog listing application**
3. **Code licencing: Learnt more about relying on code/dependenices published under Apache 2.0**

## Learning Milestones
- First experience with C++ in a long time.
   - Managed to build the project. "Hello World"~ish... but it does route json data from one endpoint on localhost to another endpoint successfully. So victory! \o/.
- Kept on keeping on with the Flask implementaion of the dog listing app
   - Impmlented the service layer testing

# January 1, 2024
## Main Achievements 
1. **Kept working on code in python, c++ and php through the day**

## Challenges and Solutions
- Python/Flask
   - Needed to figure out the boundaries between securely serving a dynamic website and injecting js into my site.
      - Challenge: Figuring out a way to present my site as a static html with js scripts to manage the dynamic parts
      - Solution: Ended up making a course for trying out a index.html landing page with container element for both the initial state elements and container elements for things that get dynamically added. The index.html contains all the scripts required (so no scripts get loaded/inject beyond the initial page).
         - This does limit my testing of server side responses to partial static elements. Which is fine because thats what i was already doing anyway.
- C++
   - Needed to start working on returning rendered templates in the C++.
      - Challenge: The library I had settled, mustache, on turned out to have not been updated in 9 years.
      - Solution: I switched to Jinja2Cpp instead. It was a learning curve to install but i think it went fine. Still have to test it (***to be updated later today***)
   - The last solution to template rendering turnd out to be not so great
      - Challenge: Jinja2Cpp was hard to install. It took long and did not seem to work even when i managed to make with it. The documentation for it was also incomplete.
      - Solution: I did learn how to use the conan package manager.. which made my install process much faster. The ultimate solution was to switch to inja for template rendering. Inja is based on Jinja2cpp and is more lightweight and it seems to work.
   - I couldn't transmit emojis from the html template file to the browser fetching and visually rendering what it got from the server.
      - Challenge: There was not much challenge, I had the input (dog emoji) and the output (signs and symbols) just needed to research the possible reasons for the transformation.
      - Solution: I found out that it was to do with the mime type relayed in the http response. Emojis are utf-8. I set the mimetype to that in my server code before sending the response.
   - 
- Php
   - Run basic server locally
      - Challenge: Run actual server that routes the json output of one local endpoint to another. 
      - Solution: I had already gotten code that worked from from chatgtp.
   - Logging in php
      - Challenge: I had no idea how to log stuff in php as i was debugging.
      - Solution: Managed to get some output, buth info and dynamic data through symphony
   - Data structures in PHP
      - Challenge: Attempted to use an array of arrays in partial lavarel (blade) html rendering. Tried to use arrays/array members as strings or object fields repeatedly.
      - Solution: Learnt a bit about arrays and objects in PHP. (like using $obj->field vs $array\['index'\])


# January 2, 2024
## Main Achievements 
1. **Kept working on code in python, c++ and php through the day**

## Learning Milestones
- Python/Flask
   - Set up the index.html for the github-pages site. It fetches most of the html.
   - Added CORS handling to the flask code
   - Did my first implementation of selenium for testing the html output of a external endpoint (in this case the flask server implementaion). It worked fine! Cool AF.

- C++
   - Added CORS handling to the code.
   - Mapped out testing and refactoring the code for testing ***Still needs to be verified***

- Php
   - Enabled CORS handling in the code. Apparently this is a very smooth ride in Laravel in PHP and I love that.
   - Changed the service layer to be globally injected (using config variable for the base url it fetches data from). Again.. this was a very smooth ride in Laravel/PHP and I love that.
   - Started working on unit tests of the server-side interface layer. Managed to get some concrete functionality executing.
   - Planned unit tests of the service layer code.

# January 3, 2024
## Main Achievements 
1. **Kept working on code in python, c++ and php through the day**

## Learning Milestones (Or just log of work done.. if you want to call it that).
- Python/Flask
   - Added to the index.html which resides on gh-pages and fetches from both of the server endpoints on heroku. Now it has a snackbar for error messages.
   - Refactored the Python project for a more modular structure. There are minor issues but i am happy with most of what I achieved. It looks much better.

- C++
   - Started setting up the refactoring of the code structure. It might not work as I havent tried running it. And its probably incomplete because I got a bunch of it from ChatGPT. But it is closer to a comprehensive and well organized structure than I had before and it will be a learning experience for me to finish it.

- Php
   - No work


# January 4, 2024
## Main Achievements 
1. **Kept working on code in python, c++ and php through the day**

## Learning Milestones (Or just log of work done.. if you want to call it that).
- Python/Flask
   - Plotted and planned more selenium code. Including an additional localhost router that can simulate network errors (for testing environments)

- C++
   - Managed to refactor the code to support injection of services and such! It requred breaking it down into a few more files but seeing it all come together was so amazing.
     - And seeing it run! Amazing!
     - And then getting a test running (even though it didnt do anything)! Woo \o/
     - And finally getting some "Run all tests" code also up (even though I only have one test project/executable right now). Now I have what seems to be an umbrella for my tests.
       - And I can dig down and create the tests. Yes!

- Php
   - Learnt more about logging in php (for debug purposes). tail -f storage/logs/laravel.log
   - Finished wrapping my head around the setup of the unit tests.
   - Added E2E testing for the routes + the service layer.
   - Started writing some DocBlocks. Not sure how that goes but apprently there is something called phpDocumentor I can possibly use to autogenerate comments from what I am doing.


# January 5, 2024
## Main Achievements 
1. **Kept working on code in c++ through the day**

- Python/Flask
   - Nothing much really

- C++
   - Added a bit to the dog breed service class.. finished error handling and such.
   - Made the first actual test that tests anything. And it injects a html client and expects a response and oh my so great. (And it finally ran! wooo \o/)
   - Went all the way with testing. Finished them. It was hard figuring out how to inject all the stuff and make it work together. 
      And I even manage to get a executable together that runs all the other test executable.

- Php
   - Nothing much really

# January 6, 2024
## Main Achievements 
1. **Kept working on code in python through the day**

- Python/Flask
   - Worked on selenium tests
     - Finished operations success path
     - Changed html (both gh-pages index and server index)
       - Moved snackbar to the server index
       - Added ids to elements in server index to facilitate testing
   - Set up delay and error middleware for testing



# January 7, 2024
## Main Achievements 
1. **Kept working on code in python through the day**

- Python/Flask
   - Set up routing for static files during testing
   - Started setting up digitial signature verification for content loaded from remote server

# January 8, 2024
## Main Achievements 
1. **Kept working on code in python through the day**

- Python/Flask
   - Finished setting up initial code for digitial signature verification for content loaded from remote server
      - This was difficult, and fun! I learnt about digital signatures and how to create and verify them in both python and js/node


# January 9, 2024
## Main Achievements 
1. **Kept working on code in python, c++ and php through the day**

- Python/Flask
   - Started code clean up and putting all the pieces together in python.
   - Managed to 
      - Set up all the selenium tests.
      - Restructure the directory structures a bit.

- C++
   - Did a ton of research on digital signatures, and implementing them in c++
      - Realized it was beyond the scope of my capabilities right now, and not within my current timeframe to learn it.
      - I ended up having a lightbulb moment, planned implementing the digital signature part by calling my python code that performs the same action. It was a fun implementation to plan. A lot of weak spots to cover.

- PHP
   - Started planning the digital signature part for php.

# January 10, 2024
## Main Achievements 
1. **Kept working on code in python, c++ and php through the day**

- C++
   - Finished implementing the digital signature implementation that calls python. Still need to test it on a linux machine but its cool to see it work on my machine.
      - This includes a signature script in python. And code that rus it (as) securely (I knew how to) from c++! Fun \o/

- PHP
   - Implemented the digital signature for the routes in php (index and renderBreeds). It was.. like an hour of work? Compared to doing it in c++. It was just all there. Wow. PHP amaze.
   - Improved testing code a bit.

- All three languages
   - Syncronized the initial page template across the languages.
   - Set up data sanitation for the input from the external dog breed service, in all three code bases
     - Plus code to test for unsafe characters, again in all three code bases

# January 11, 2024
## Main Achievements 
1. **Kept working on code in python, c++ and php through the day**

- Python
   - Review of code, listing finalization tasks according to priority

- Selenium test code
   - Review of code, listing finalization tasks according to priority

- C++
   - Learnt about MACRO variables
   - Changed the service url from hardcoded to config var
   - Removed unused code
   - Developed test code further

- PHP
   - Did a bunch of stuff, fixed some code, changed cors settings (Minimum whitelist paranoia mode). AND:
      - Commented out ALOT of skeleton code from Laravel. Whitelist whitelist whitelist, at least when I'm pushing code. I can always escalate permissions later.
   - Researched how to get PHP projects up and running on Heroku.
   - Went for a full on Heroku commit. First code in PHP I broadcast into the production env aether! Although it wasn't much of a broadcast, but it did go into the aether! Accessible by all, known by none. AND! In less than two weeks since I did my first PHP code! While doing it in two other programming langauges. And not just a skeleton template generated by a framework, but code I feel content about presenting (I will push it to GitHub tomorrow, most likely. And link to it, professionally as well.).

- All four projects (incl selenium test project)
   - Review of code, listing finalization tasks according to priority. Tasks required for MVP (min viable product) highest prio.
   - Generally cleaned all of the code. Added comments here and there, removed comments elsewhere. Even changed some variable names and order of actions.
   - Started negotiating with myself on what I wanted to acheive in my first push to public access vs what was acctually needed.
   - Specified CORS settings for all projects
   - gitignore file for all projects
   - Started planning extraction of client-side testing project (selenium project, the fourth project) from the other projects.
   - Started drafting/planning the readme.md s for the projects.
   - Started drafting/planning the overview repository for all of the dog(go) the projects.

# January 12, 2024
## Main Achievements 
1. **Kept working on code in python, c++, php and the dog client project through the day**
   - All four main projects
      - Updated html headers in the index file of each project with a viewport meta tag for responsive design

   - Python
      - Moved the GhClient code (selenium stuff (including the nodejs middlware), and web/index.html) out of the python project. Into its own project
      - Set more restrictive CORS setttings for the first push (it will need to be less restrictive when I deploy to prod)
      - Decided on a name for the GH project, and made the repo! PythonDogDisplay \o/

   - C++
      - Researched making more opmitimized CMakeLists.txt files
      - Set more restrictive CORS setttings for the first push (it will need to be less restrictive when I deploy to prod)
      - Decided on a name for the GH project, and made the repo! CppDogDisplay \o/

   - Php
      - Set more restrictive CORS setttings for the first push (it will need to be less restrictive when I deploy to prod)
      - Decided on a name for the GH project, and made the repo! PhpDogDisplay \o/

   - DogDisplayGhClient
      - Moved out of python code into its own project.
      - Decided on a name for the GH project, and made the repo! DogDisplayStaticClient \o/


2. **Started working on overview project for the Dog projects on GitHub**
   - I decided on a name, and I made the repo on GitHub. DogDisplayOverview! \o/

3. **Worked on some job applications**
   - And I delivered 2 minutes before the deadline! \o/

4. **Made some contrete decisions on code licensing today, for better or worse!**
   - Created five repositories on GitHub, ones that I've planned out and actively observed how I'm relying on third party licences in each of them. 
      - The most restrictive licences I'm using as dependencies (AFAIK) are MIT, Apache-2.0, BSD-2 and BDS-3. I feel confident preemtively delcaring my projects as MIT licenced.
         - I hope it is ok. Code, knowledge and understanding should be free, but I still want a slight restriction on how people act on what I publish. I don't want to publish stuff and then have someone restrict me on what I have already published only because I did not licence it. And at the same time, I want to respect the liecences and restrictions others present, in the context of the third party code I am using and relying upon. I hope I'm safe in my decision to use MIT for my projects. But whatever... ¯\\_(ツ)_/¯.... if I made a mistake.. then I am willing to learn, improve, and update my behaviour and presentation. If someone finds an error I will listen, learn and improve. I'm dedicated to respecting others, and the boundaries others set! (Within certain limits, for example I would not easily accept it when a person or people act towards any other person or persons and then stonewalls. Boundaries are not a cheap way for a person/people to avoid responsibility and accountability for actions, words and decisions they make by their own initiatve! 💪!)
		
5. **Finally exited the orbit of CHAOS for this project. I've researched everything, done the 'experimental kitchen' part, defined the recipe and materials, gathered the materials, cleaned up the experimental kitchen and started cooking the actual production recipe. I have reached escape velocity from the gravitational pull of the initial CHAOS of research, experimentation and brainstorming.. and I have entered the sphere of ORDER for this project. I've started sepratating the good from the bad and the ugly, and I've started publishing the good parts.**

- This is such a philosophical statement. Probably too much for something I am already thinking about publishing 😅. But whatever ¯\\_(ツ)_/¯. Transparency is fine too!
- Also I made repositories, with thought out names and licences and such. First steps.. Everything is ready, the recipe, ingredients.. I can start cooking! And take determined steps towards the finish line, and then continue and start work on other projects. \o/


# January 13, 2024
## Main Achievements 
1. **Kept working on code in python, c++ and php, as well as the overview for these projects, through the day.**

   - All three languages
      - Got scripts for generating files on the third party licences up and running.
      - Cleaned code as much as I had to and could.
      - Generated version files and changelogs
      - Generated readmes for projects
      - Learnt about and researched versioning and changelogs a bit (Semantic Versioning)
	  - Versioned and added a changelog to the project (I think all of them?)
     - Verified the contents of ai generated content in READMEs is in line with my own understanding.
     - Moved to local repository folder.
     - Git added .
     - Git commited
     - Git remote added origin
     - Git pushed! \o/

   - Overview project
      - Generated readme for the overview of these projects, my process and my aims and my strategy.
      - Scaled back the readme, moved things to a Roadmap, preferring to develop my readme further at a later point, rather than directly use text generated by using my context. Getting generated stuff (an almost kind of real placeholder) was great for strategizing the project, but I feel a strong need to mentally converge with every line I place into env at a level this high in my portfolio paper trail. I dont express important stuff in my own name (at least I hope I have learnt to) without it being based on my understanding.
      - Git added .
      - Git commited
      - Git remote added orgin
      - Git pushed! \o/

# January 14, 2024
## Main Achievements 
1. **Kept working on code in python, c++ and php, as well as the overview for these projects, through the day.**
   - CppDogDisplay
      - Fixed versioning in code.
      - Added a comment on signing service design decision.
   - PhpDogDisplay 
      - Added changelogs file
   - PythonDogDisplay
      - Added some liecense stuff.
      - Fixed versioning in code/or added changelogs for them (i forgot to add the changelog file ).

   - DogDisplay Overview project
      - Added a version
      - Planned slight changes to README.md
      - Planned versioning
      - Planned adding raw data
      - Created raw data folders, files and folder readmes locally.
         - Also gave those a first pass review.

2. **Worked on project demonstrating transferable skills from factorio experience to development projects.**
   - Factorio translate-able skills to dev skills
      - Started repo on github
      - Gathered a bunch of past data. Including:
         - Bunch of screenshots Ive posted online along with my comments on those pictures (valuable text, in the moment documentation).
         - Min max scripts that I found.
      - Made additional plans for possible content (third party material)

3. **Worked on some job applications**
   - Just planning my work and syncing my strategy with requirements in the postings.


# January 15, 2024
1. **Project management and meta-cognitive, meta-meta cognitive stuff.**
   - Project mgmt
      - Created a script for syncing version refrerences across a project with the latest entry to CHANGELOG.md as the base comparison.
      - Set up comprehensive backlog for my ongoing projects
         - Even made that into a project

2. **Worked on project demonstrating transferable skills from factorio experience to development projects.**   
   - Factorio translate-able skills to dev skills
      - Wrote an initial readme for the repository.
      - Set up some tasks for prepping the initial alpha of the repo

3. **Kept working on current DogDisplay projects.**
   - DogList server projects (c++, php, python)
      - Set up listed tasks for projects
      - Added a Python script that looks for files known to reference current project version and commits to testing them if they do contain that reference. The script then it validates whether all of the files in the project that reference curr_ver reference the same version, returns information on succesful matches and errors. Returns with exit code 1 if errors are found.

   - DogDisplay projects (server + overview)
      - Switched to staging branch
      - Added lightweight CI/CD script for staging env that checks for conistency between files in version references, if it passes, pushes to main.
      - Added OpenAI powered, ChatGPT-4, statements to all README.md files

   - Overview Repository
      - Added changelog
      - Added this file along with the ad hoc local version control logs for the projects from the initial experimental phase.