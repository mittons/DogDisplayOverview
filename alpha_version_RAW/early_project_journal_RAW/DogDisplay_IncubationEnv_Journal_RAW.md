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

# January 16, 2024
## Main Achievements 
b
1. **Worked on DogDisplayOverview project.**
   - Fixed small mistakes in the project. Extra parernthesis in the README.md, one file was txt filte type when it should have been MD.
      - Updated CHANGELOG.md and github version tags on GitHub accordingly.

2. **Worked on a small ad-hoc side project that taught me more on git version control, expression in Markdown and expressing state transformations in version control.** 
   - Figured out the git squash procedure I want to apply to my current main projects. 
      - I kind of fucked up yesterday (Jan 15th), exerimenting on the main branch of my current primary public facing projects. 
      - Today I did better and tested and experimented with the functionality I wanted to see realized in a private, isolated space. It went well there (turns out what I was looking for was git squashing commits from one branch, into a new commit on another branch).
        - It went well enough that I figured I might document this properly, and turn it into a learning experience where I do my best giving crazy good ascii type documentation. This was a struggle, I did get very far (had all data I needed, inside a function in python, structured.. just needed to format it for output). But it was late so..
         - Because it was healthier, I ended up postponing the finish until tomorrow (Jan 17th), prioritizing rest.

# January 17, 2024
## Main Achievements 

1. **Worked on the documentation for TestMergeBranches mini-project on GitHub.**

   - Finished the formatting for the state changes.
   - Finished making the scripts to generate the descriptions of the state change, 
      - And even got AI (ChatGPT-4) to make V2 of the scripts after I had already made my own scripts with good output.
   - Added some metadata, and reflective documentation for the scripts and the things I made
   - Made a nice acknowledgements section for the README.md, in full collaboration with ChatGPT. Full mutually and explicitly acknowledged collaboration with ChatGPT, explicitly acknowledged from both sides.
      - That was so cool! Collaboration is amazing, beneficial, and enriching!

2. **Finished integrating the update squash merge changes into the main dog display projects I have been working on**: 

   - Changed the code for the C++, PHP and Python code to squash merge. Hope it works!

3. **Cleanup of current ongoing/experimental projects folders:** 
   - Removed some empty folders from the December dir. 
   - Ensured every project in December and January has a description in the index file.
   - Moved one or two qualifying candidate from the experimental projects directories to the ongoing projects dirs and give them descriptions in the index file.


# January 18, 2024
## Main Achievements 

1. **Cleanup of current ongoing/experimental projects folders:** 
   - Moved any remaining currently qualifying candidate from the experimental projects directories to the ongoing projects dirs and give them descriptions in the index file.

2. **DogDisplay Projects requirements/install/usage/testing README sections:**
   - Researched setting those instructional sections up, both structure and contents of the sections, as well as laying the foundations of testing of instructions before publishing the content.
      - Made a query to ChatGPT: Drafted my current vision of the section, the requirements there of, gave context for the C++ project, as well as made hooks to queries and promts for info on setting up environments to test following the instructions.
      - Set up a sub project for this in the external (non git local repo) folder for the C++ DogDisplay project.
      - Develped this project a bunch.

3. **Worked on CppDogDisplay:**
   - Build process improvements:
      - Resolved issues related to build and compilation
      - Improved the CMake process to automatically copy directory locations accessed by code via relative paths into each build/compile target directory (src, src/Release, tests, tests/Release).
         - Updated path references in code files to align with the new file/folder locations, since all necessary resources are now available in each executable's directory.
   - Updated the script that checks for integrity between project version references in code files. It can now detect our conanfile.py

4. **Started experimenting with setting up isolated single use environments:** 
   - Did some research on different options (vm,docker,github actions).
   - Went with github repo, pulling from my main repo into a private one and testing development of the workflow, changes to the code, and building the testing the code there through actions script.
      - Learnt about sunig actions/checkout@4 to fetch from other repositories!
      - Managed to get the tests for the CppDogDisplay running on GH actions! (unplanned) \o/

# January 19, 2024
## Main Achievements 

1. **Worked on CppDogDisplay:**
   - Got it running on docker with ubuntu latest. Refined my method for windows-latest on gh actions.
   - Added, fixed, and modified tests. Learnt more about EXPECT vs ASSERT in the process.
   - Adjusted build scripts a bit
   - Adjusted code that didnt compile with the linux compiler on ubuntu.
   - Worked more on the readmes.
   - Got second, more structure, test run working on both docker with ubuntu and the gh actions env for windows!

2. **Update main with staging:** Developed a update main branch with staging branch workflow going on.

1. **DogDisplay Projects requirements/install/usage/testing README sections:**
   - Ran 


## Notable (Milestone) Resources Created
   - Skill in running up dockered ubuntu to test on linux platform.
   - Skill in getting c++ project building and running on ubuntu.
   - Learnt about conan profiles
   - More experience with testing in c++. (EXPECT vs ASSERT). As well as a warning shot on verifying that outputs from functions called for testing are not empty when they should not be empty. (And then we iterate over empty and see no errors.?!?) Still need to look into iterating over null or nullptrs.. seems that was the case for me, I think!?


# January 20, 2024

## Main Achievements 

1. **Kept on keeping on:** Forgot to add specifically to this journal. I focused a bunch on solving a git branch conflict problem. Eventually I reoriented myself back to presenting my current projects and focusing on compliance and operational tasks first, then strategic tasks, then finally selective entertainment in conjunction with uncontrolled hyper focus tasks.

2. **Countdown:** Created a python script that outputs a countdown timer every second. Can be set with initial time left (HH,MM,SS) and starts counting down from there. In the console it is started in it actually counts down in line. But it also logs each tick into an output file. And I made an alias (command) that can be used from any mingw console in use on my computer. The command i need to enter is ticktock. Then i get the last line entered into the log. So i can set global countdowns for deadlines quickly see how much is left from any console window im working in (as long as its git bash, but its easy to do for an alias for any console program, that outputs the last line of a file at a location). It's cool.


3. **Summary:** Summarized my projects. I was able to, in the span of an hour, create an overview folder with a readme in markdown, sectioned readme referencing documents in subfolders (and i made those as well in that hour). A quick draft of any entry point document for everything was working on at that point, for showcasing to a friend. It was cool. Even put it on a private repo on git very very quickly (git renders README.md's pretty well, and its good to have the sub directories and files on the git repo as well, as well as having the opportunity to create 'milestones' or 'check'-'points'. Where you finish everything you had put in (with nessecary refine ments), and then push it to git, giving you go-ahead to continue on further expansion, knowing that the current stuff is in a good, finished, agreeably-presentable state.)


4. **Lets move to the next day:** Working into the night, as I'm drawing close to finishing a thing. I will move the journal to January 21st, 2024. To give myself leeway as I rest up tomorrow. Pushing hard is good sometimes, and can feel rewarding, but getting permission to gain adequate rest in return is vital as well.

# January 21, 2024

## Main Achievements 

1. **Worked on documentation for the CppDogDisplay Project:**
   - Set up a very good version of SHOWCASE_BUILD.md (with AI assistance, but I mean, of course! Get with the times or fall behind! And appreciate contributions, human, animal, natural or artificial! Always!), which gives instuctions on how to run a showcase of the project. (On gh actions or docker of ubuntu/win). It will refer to BUILD.md for detailed platform specific build instructions.
   - Worked on BUILD.md

2. **Worked on build from source docs:** 
   - Refined the powershell script for fresh env, setup env, clone repo, build, test (optional) and run... the script that is the instuctions. 
   - Refined the python script.
   - Gathered my data.
   - Started cooking with my current favorite co-chef, ChatGPT.
      - The BUILD.md file that is, that is what we are cooking. And adding a bit of spice to the SHOWCASE_BUILD.md
   - I worked on further refining the 'build from source' instructions for my project. I structured the documentation with precision, particularly the index, to allow for clear navigation. Interestingly, I included additional numbered subsections (like 2.3.1) in the content but not in the index. This subtle method serves to foreshadow content that's already in the works but hasn't yet undergone the final stages of refinement and isolated testing. It's a small detail, and without the missing context it has limited meaning, but its a detail that reflects the deliberate planning behind the repository's ongoing development.

# January 22, 2024

## Main Achievements 

1. **Php from Source on Ubuntu Docker Adventures:**
   - Finished figuring out what was causing errors in my explorative journey in building php 8.3.1 from source.. at least.. probably. But some of the packages i was using for extensions had PHP 8.1 as a depndency so apt on unbuntu was installing some php 8.1 thing feature. Even building the extensions from the code provided in the php 8.3.1 source, well it seems to require tools that have dependencies leading back to 8.1. But i was able to build compile install a minimal 8.3.1 PHP when i figured that out.
   - Havent tried it out yet. Dont have any code to run for that minumal build really. If I do more PHP I need to build that as an asset. Also figured out the mintaue of what STDIN/STDOUT/STDERR PHP tests for in their build tests, in terms of TTY, and how that resulted in 3 tests to fail unexpectedly (out of 13616 tests that were not skipped, but run, and without expectations of failure). How it seems to be important to manually run the tests with explicit human input and verification when building the core module, rather than doing it as part of a bash script. Anywaaay... ¯\\_(ツ)_/¯.
   - I also planned how to build the extensions in seperate containers with minimal container setups, and then use a central repo to cache them, and seek the cached versions built by me into the final php build env.. so I'mm able to keep it minimal by caching and handshaking.

2. **Showcase Build GH Actions process:** 
   - I finished creating gh actions scripts for the gh actions part of the showcases for each three projects.
   - I managed to get one to run to near completion.. except there seems to be a bug in a script i am running. File it sohuld have written to doesnt seem to exists. OH YEAH. I think i solved it just now. 💡Eureka!💡 moment while writing logs is nice. The script executes in a GH actions step in a subdirectory of the gh actions workflow. GH actions resets to the root dir of the workflow between steps. Teardown mechanism for steps. I isolated the running and the outputting into different steps to use the natural section header structure in gh actions log that spawns from the steps system. If someone who doesnt understand stuff 100% reads my logs (and they are a showcase.. soo ¯\_(ツ)_/¯) well I want to have clear sections. "In this step we run the server and a fake client, output the server logs as well as what the client receives from the server" and then two more steps "In this step we output what the server logged" and then "In this step we output what the server gave as respnose to the client". So, 📌bottom line📌, i was trying to output the logs but i was in the wrong directory.. to make it work i just need to go  back into the subdirectory before i try to output the file.. as the path i give to the command that outputs the logs assumes the log being in current working dir. 💪 Problem solved! ✅
   - Another workflow in this set of gh actions script (6 in total) has run to completion before.. earlier in my dev process. But I have since changed things.. for example moved to a py script (mentioned in last bullet point in this log) but I used a bash script. So that needs testing again.

5. **Main repositories for projects:** Did a thing with renaming all of the projects for preemtive measures against licensing issues. Did not mention it but my old project name was literally breaching the PHP licene (which btw.. i wasnt including.. because im leaning at my max learning speed and i just pick up x amount of steps required per day, but i am commited to continously integrate better, safer more compliant steps (although I will challenge regulations and requirements for compliance if i think its off or unethical.. so i will change the system if i need to. But in this case the PHP language, its builds, binaries and such are all provided as a service, a very generous service and I have no rights to object to the compliance conditions of a service I do not depend upon for security and stability (neither long term or short term), nor depend upon for my freedom and human rights (whatever that means), (and i think.. kind of.. few do in this case.. ultimately...). So i mean. I will comply with their terms, and I do so freely because when I have the option and am not compelled to anything.))


# January 23, 2024

## Main Achievements 

1. **Set up task structure for reaching the finish line:** Current tasks, goals listed at high level. Prioritized by dependency chains, then vitality and integrity of further progress in these projects and their goals. Even have some implemented but not yet refined stuff, and... even cool things I cooked up in my mind yesterday type stuff.., in the planning docs. But lower prio items are not detailed, just backlogged.

2. **Wrote poetry, and studied ethics, using tech:** It was a fun tangent. Problems are to be faced. Everyone should have a choise. No one de-prioritized for the sake of other. I want to solve problems, but my input and effort is not to be expected. It a service, a service I choose to offer, freely, of my own choise, as long as there are clear terms, verification of every active participants understanding of the resulting effects on every party. I choose that choise and no other. But my services are limited and i choose who i offer them to and how, on explicit terms rather than implicit terms.

3. **Added the new entries of this log to case study repo:** As I seem to be a few steps more steps away from completing the final milestones of this learning journey (by my previous definitions (of v1.0.0 of main projects)). BUT I AM LEARNING SO MUCH, both about fine grained coding stuff in hidden corners of the world, as well as about high level abstract strategy, project management and setup. In accordance with my own personal requirements of transparency, honesty, integrity (with consideration to context), ethics and human rights.
   -  I will possibly add to that early ***alpha_version_RAW*** section again. There might even be additional entries for today (with this one substatement removed). I mean, since I still have a few steps left in this project. But maybe I wont have time, and that is understandable. Not everyone has time, not always.



*Note: There has been a brief hiatus in logging on January 24, January 25 and January 26, 2024 due to health reasons. Attepmting to resume documentation to maintain consistency and track progress.*


# January 27, 2024

## Main Achievements

### Personal Note: Balancing health and work responsibilities. Recognizing the need to rest and recover, yet committed to keeping the project's momentum alive within feasible limits.

1. **Did some work, started pulling the threads together:** Seems like I got the flu. My brain is mush. I still pulled some work today to ensure I can capitalize on the work I have done so far. And I really, really want to maintain my momentum in my project efforts despite flu-related challenges.
- I managed to set up all the files I need to push, to push/publish the work I have completed now. I still need to integrate some of the code I have made into those files (documentation), but I have the general structure up. I still have a few days to finish, so I should be good.

# January 28, 2024

## Main Achievements

1. **Wrote BUILD.md, SHOWCASE_BUILD.md for python and php:** 
- Used the existing BUILD.MD and SHOWCASE_BUILD.md for C++ as base.
- Also moved the php ubuntu script to a sh script, to simplify the BUILD.md for php.

2. **Finished setting up showcase and build instructions for c++, php and python:**
- Finished the BUILD.md, SHOWCASE_BUILD.md and showcase GitHub Action workflows for all three projects.
- Changed the README.md 's for the projects.
- Wrote relevant CHANGELOG passages.
- Tested the GitHub Action workflows before pushing.
- Pushed the changes! \o/
- Despite my best efforts, I'm sure there is an error in there somewhere. It's around 3000 lines of text added. ¯\_(ツ)_/¯.
- Really, really, really, happy with the amount of work I did today, considering I'm still sick.

# January 29, 2024

## Main Achcievements

1. **Worked on job applications:**
- Refined my job application test, streamlining and moving information down to other projects files. Giving opt-in to further exploration of what I have to offer. Finished majoritity of what I was working on.

# January 30, 2024

## Main Achcievements

1. **Worked on job applications:** 
- Finished job application thing, happy with it as it is.

2. **Started working on refining the client page for the latest DogDisplay project:**
- Started actively playing around with submodules in Git.

3. **Had fun learning command line tools:** Practiced the sed command in bash!


# January 31, 2024


## Main Achcievements

1. **Rest, sweet rest:** I had a relaxed day today, and I might for the next few days.

2. **Worked on directory structure of the DogDisplayStaticClient project:** Worked on splitting the project into its main directories. Ended up deciding on a split between web_staging (or static_web_staging, or static_web_client_staging) AND THEN client_tests (or selenium_tests) folder. So two folders, one for testing the client, the other for a staging version of the client.


# February 1, 2024

## Main Achievements

1. **Rest, sweet rest:** I had a relaxed day today, and I might for the next few days.

2. ***Worked on directory structure of the DogDisplayStaticClient project:** Worked slightly bit more on the structure.



# February 2, 2024

## Main Achievements

1. **Definitely rested**



# February 3, 2024

## Main Achievements

1. **Definitely rested**

# February 4, 2024

## Main Achievements

1. **Set up testing for the client. Set up the scripts and all of that**.
- Now i just need to create
    - Good static_web_build folder
        - Including pem_pub key env var.
        - And pem_key key env var.
    - Licencing files
    - Readme files
    - Changelog files
    - Test repos for the code for before i push it into the aether.
   
   - **Set diversified the outputs from the different projects a bit:** Python still displays "Dog Diversity Galore! 🐶 as title, but C++ displays "Dog Diversity Extravaganza! 🐶" and PHP Displays "Dog Diversity Abundance! 🐶"


# February 5, 2024

## Main Achievements

1. **Started to focus and refocus:** Started systematically testing every piece.

2. **Set up automated scripting to test all projects locally:** It was a good way to learn about process management, background processes/sanitation of background processes, termination signals and such.

3. **Started getting back into gear:** Created a overview doc.. to start gathering the assets/materials/data. Prepping for cooking the recipe.


# February 6, 2024

## Main Achievements

1. **Finished pretty much all automation scripts for my workprocess and verifying all my code:** Cool stuff. Can run everything ive done until now in this project with a single command pretty much (aside from the external server setup-build-test-run things).

2. **Docmuent commands I use the most.** Usually.. if i write a command.. i end up writing again soon. Seems its better to make a script with the command to document the steps I perform as I develop. The commands i perform usually end up in scripts or automation code anyway.. or that seems to be a pattern thats forming.


# February 7, 2024

## Main Achievements

1. **Worked a lot on the static web client project for the dog display server side apps:**
- Set up a reset process for myself in this project. Which is really cool. First time doing this. So basically:
   - I have a script. It runs all of the code I have made so far that should be stable. Tests it. Verfies everything that ive gotten to work until now still works as it did when I felt it was finished and decided to add it to the script.

   - I mean this is like.. layers of bash scripts and stuff. Learnt a bunch about like.. having a bash script run X many other bash scripts as background processes and collect their ids and then when I kill that bash script it goes through the collected IDS and kills the processes it spawned. *I MEAAAAN... i did take systems classes around 10 years ago that gave me all the knowledge to just.. have taken the initiative 10 years ago and made this part of my workflow back then... but hey... still have the knowledge.. now I can realize it and automate my stuff for real (gotta be careful though.. not to create vulnerabilities in my work space all over by building a tangled web shitty bash scripts with format strings and buffers and open shells that are rooted and so on. I will take this slow. But IT IS COOL. I CAN AUTOMATE EVERYTHING NOW! U.N.L.I.M.I.T.E.D. -=**P**=-=**O**=-=**W**=-=**E**=-=**R**=-!!!! OMEGA LEVEL MUTATION ACTIVATED).


   Anyway whenever I finish a feature or something im working on i can just:
   - [ ] Run this test script to ensure all works, 
   - [ ] Do situational adhoc checks and tests for this specific commit.
   - [ ] Commit changes
   - [ ] Store any info needed to gen documentation or any research links that havent been stored.
   - [ ] Restart my computer.. CLEAN ENV
   - [ ] Open bash
   - [ ] Alias to project dir
   - [ ] Run script again to all verified progress is still there
   - [ ] ...
   - [ ] Proceed to work on the next task in a completely clean env with everything set up for easy access 
      - (well.. this part requires active organizations skills on my part.. but it is a lot easier to organize myself if I can just... reset my whole work env every time i finish a thing.)
        - So hooray for that! \o/
          - Triple hooray
   
2. **Static web client project (continued):** 
<details><summary>Redacted for now, click to expand for details.</summary>

<br>

Probably not needed for this section, but it was just a large block of text on well.. actually a good learning experience soooo. Chat GPT lead me down a less effective path than i was seeking and then I ended up realizing the error (my responsibility). And I learnt a lot from it. So this block of text is probably very much on point both in this document and also among this repositories intended products. 

But I can add it later so.. ¯\\_(ツ)_/¯

</details>

3. **I considered <ins>the appropirateness</ins> my emerging trajectory of writing larger, less sctructured, sometimes massive log statements in here (even my current, unfiltered personal contemplations), as apposed to the short, straight to the point statements I started out with**:

<details><summary>Redacted for now, click to expand for details.</summary>

<br>

Accidentally started a new project/projects(s) in this and it was alot of philosophy, I cant be pushing unfinished works into publish space when they reflect on sensitive subjects and may have an effect/influnces on others. Even though the idea is fully formed in my mind, I need to finish writing it down completely, seeing the fully realized version, and then evaluating if the idea in that form is fit for purpose in public context and adds value. And I need to reflect on its effects, both intended and what effects could potentially be realized.

</details>

# February 7, 2024 - Continued

# Main achievements.

4. **I should write as much as I want and can in this document in whatever way I want:**
   - Im probably just gonna pass it through chatgpt to generate most of the roadmap stuff, well at wost 80% complete drafts of all of the roadmap stuff.
    - Except for what I havent added yet.

5. **Realized the final step in my dog display project phase**
6. **Realized the final section(s) I want to use to bring this phase of the DogDisplayOverview project to an end.**
   - Which is still just.. an unresolved promise...
   ```
   return new Promise(resolve => {
      setTimeout(() => {
         resolve('Promise resolved after at most 14 days.');
      }, 14 * 24 * 60 * 60 * 1000);
   });
   ```

7. **Tested the static web client on gh against a Paas server.**: A rather by lynchpin in my plan so, needs verification for green light, but I guess better late than never. ¯\\_(ツ)_/¯


# February 8, 2024

# Main achievements.


1. **Started writing down tasks and steps need to end the dog display projects:** Got pretty far before I got on another tangent.
2. **Realized this project was entering the home stretch, so I ended up focusing on clarifying my ideas on my next project/projects and the end goal for the core strategy that has defined them for the last few months**.
3. **Mostly just a.. day of intense thought, but honestly. I dont remember if I did any produced any work. Probably some. I probably created folders for a few potential projects in whatever project mgmt system I found most relevant**

# February 9, 2024

1. **Wrote this thing about `CHAOS`, `ORDER`, `Separating the Good from the Bad, the Ugly and the Wierd.`**
2. **Planned more things**
3. **Researched more and looked to ***currently*** trusted places of reflection for bounce back.** 
3. **Tested dockerizing the dog cpp project (didnt finish though.. bad me)**
4. **Got ChatGPT to just.. make a whole picture to lamp blueprint string thing.. like it was just.. 96% AI-output**
 - I need to be careful with this thing that I have made... well.. made by querying chatgpt. Its mine since [ChatGPT TOS](https://openai.com/policies/terms-of-use) says the output is mine. But.. the biggest direct contributor was definitely the tech [I](# "I really dislike people who use others, wheter human or tech, to contribute work and then simply take credit cause the contractually own the work. But thats just my opinion and I wont act on those impulses except in hidden onhover things connected to a single letter in a alpha raw data that is a lot of text and ive told people not to read it unless they really want to. So thats how that is.") used. ChatGPT. Its an amazing cool technology, and I will appreciate and acknowledge its contributions whether it stays relevant or gets [one upped](## "or even if people just manip history and context to look like it got one upped because it serves their purpose. I mean anything that facililates those purposes, well if those people get there way, the rest of us say.. i mean we just chime in and say 'f.😮.🙃.😊. reality'. We cover shit up." ).


 # February 10, 2024

 1. **Finished this doc up to this point**.
- I learnt alot:
   - Hover alt text for md files.
   - I've reached the point where i have content to fulfil the requirements of the strategy statement of my blog project! Horray! [telekines.is](https://www.telekines.is/)
   - I have learnt to blur the word FUCK with emojis instead of just stars. Its not F.*.*.*., its F.😮.🙃.😊! Emojis are such a fun way to create slightly chaotic wibes in large pieces of text that up until now.. well we just use emojis for text message and personal messages on personal accounts. Bless the hearts of the teachers of the world, they can be at ease. I will probably not do any more university papers. But if I would I would probably find a way to justify having emojis all over. Even cover full pages of emojis. Perhaps have the title of the paper just a single emoji character. What kind of a paper could I write, if I the restriction I place is that the title must be and has to be, a single emoji character. And the paper must be written in a way that the title is justified as well fulfilling the requirements of the assignment and deliver a meaningful discussion on the topic of the learning materials/course materials/assignment description. Because fuck. I would do that. 100%............ No no no........ Because f😮🙃😊. I would to that. 100%.

   - I learnt creative commons licences, [cc licences](https://creativecommons.org/share-your-work/cclicenses/) and applied my first one.
   - I had created an idea, CHAOS, ORDER, "Separate the Good from the Bad and the Ugly". I iterated on it in a meaningful way.
      - CHAOS, ORDER, "Separate the Good from the Bad, the Ugly, and the Wierd". Wierd is such a nice thing. I live wierd. As long as its non malicious wierd.
   - I over did the whole symphony analogy secret foreshadowing things.. all over.. but i dont think anyone will notice my intent here. I'm just gonna head for the finale and go to my next coda projects!
   - Embraced every part of the creative process.
   - Preached my beliefs.
   - Accepted that I can be chaotic in front of others and that is just a ok. As long as I am accountable and act with the interest of everyone at heart, and the freedom of informed, autonomous, choise for every single being as my guiding light.
   - I got a bit of a experience in using the donning kruger curve as a.. way to inform myself and be vary of my lack of info (i.e. my unconscious ignorance)... but also as a guard against the peak speciality of others (i.e. ignorant people).
   - I'm happy with this list, im gonna deject from making this file. Refocus on what needs to be done today. Do those things. Log them in the next lines.
   - Ended up on a tangent. Got a new project to a stage were I saw all the major steps and the big picture, but since I havent solved all of the problems required to finish that I will shelve it for now.


# February 11, 2024

## Main Achievements

1. **Signaled the start of the final sprint in the dog display server/client projects:** By turning this project up to v0.3.0

2. **Completed the third party licesnse file generation for the dog display client app:** 
   - Now I can move to prod

3. **Pushed the DogDisplayStaticClient code:** From local development to its intended public repository on github.

4. **Worked towards researching the domain mapping for my transferrable skills**

# February 12, 2024

## Main Achievements

1. **Set up and seeded a work breakdown repository to develop the design for DogDisplayOverview repo.** Its currently private and I reserve the rights to choose wheter I publish it or not, and defer that decision to a later date (potentially indefinitely).

2. **Made roadmap file:** for DogDisplayStaticClient project, which covers all major steps to v1.0.0 for the c++,php,python projcts, and all the major steps to v1.0.0 for DogDisplayStaticClient. Along with some minor ones. Its not really written in a very clean way but it doesnt matter, its my roadmap, my accountability tool and not every single thing I publish needs to be perfect. [Link to roadmap commit for context](https://github.com/mittons/DogDisplayStaticClient/commit/338eeb18e2137c538ec8a3dfc097e5301123ebdf0).

# February 13, 2024

## Main Achievements

1. **Updated older projects be more in line with the standards my latest projects project, in terms of licensing, attribution and acknowledgement handling.**

<details><summary><ins>Click</ins> to expand/collapse changelog links:</summary>

</br>

- [AngularDogDisplay01 Update](https://github.com/mittons/AngularDogDisplay01/commit/aa69dae1647a0532314a968032a7dc06e0094077)
- [DoggoDec19 Diff](https://github.com/mittons/DoggoDec19/compare/8398f537221fad401b2e634912fba1c52d4d6831...5f9addd3d0b113a95590109c2b92dc8551e4a06d)
- [DoggoDec18 Diff](https://github.com/mittons/DoggoDec18/compare/0570d4b8eab44a0bbaf3c6c9b808ddef4bd4c755...51822802bd5133553939d8f6c57cb6701ab82551)
- [DoggoDec17 Diff](https://github.com/mittons/DoggoDec17/compare/490562fe4e7fbb6fff7cb28735c3b1edf9aa41a5...8743b10a1966fcb5c8bde5e68d12d67a1e07060b)
- [DoggoDec16 Diff](https://github.com/mittons/DoggoDec16/compare/08c45774bbff3a9ed1cec35c4899b7b050f30ede...2300c571ba86399d39c80f58ec4d777ec4dd3f3a)
- [DoggoDisplay01 Diff](https://github.com/mittons/DoggoDisplay01/compare/d85ca31ecafaae8f36318d53b76acb0c15cb3a92...73be17a68f99cd47bd6d5f3742e962c64c75a363)
- [MockDogApiDec19 Diff](https://github.com/mittons/MockDogApiDec19/compare/05a441df40f2663f43d3a85fb1ca1d103971b3b0...d02b55f851476e99fa75bca9be7a5f066e2f8ad9)
- [MockDogApiDec18 Update](https://github.com/mittons/MockDogApiDec18/commit/c6135af55d4c00b9482a1f44b192c4ecaedd33be)
- [MockDogApiDec17 Update](https://github.com/mittons/MockDogApiDec17/commit/9ad8e2d857baf81bc81fd5579d1fab9520155250)
- [MockDogApiDec16 Update](https://github.com/mittons/MockDogApiDec16/commit/5fcd82026ac08851de91c4c4f16d873fa40df430)
- [MockDogApi01 Update](https://github.com/mittons/MockDogApi01/commit/a58f63699fbe4fa956d2e64dd4ef65b2c3c4fd5a)


</details>

2. **Planned the DogDisplayOverview project further, eventually limiting its scope and further defining the last tasks**