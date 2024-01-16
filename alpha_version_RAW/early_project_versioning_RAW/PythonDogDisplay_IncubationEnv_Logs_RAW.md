# DoggoDisplayFlaskTest01 - Project Folder Index

## PROJECT DIR: _clutter
### About Project:
_

### Started On:
:calendar: January 09, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_


## PROJECT DIR: _incubation
### About Project:
_

### Started On:
:calendar: January 04, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_


## PROJECT DIR: docs
### About Project:
Documents for this cluster of projects

### Started On:
:calendar: January 03, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_


## PROJECT DIR: dogs_flask_test_01
### About Project:
Project meant to get a simple service layer + interface/presentation layer setup going in flask.

### Started On:
:calendar: December 28, 2023 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
- Service layer set up in Python using requests module.
- Interface/presentation layer set up in Python using Flask and the service layer implementation.


## PROJECT DIR: dogs_flask_test_02
### About Project:
A project that extends the Flask project [dogs_flask_test_01] with the use of Flask templates. 

In the template we should be able to render elements:
	- In sequence
	- Using conditionals
	- Using loops

### Started On:
:calendar: December 27, 2023 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
- Being able to use tempalate rendering in Flask.


## PROJECT DIR: dogs_flask_test_03
### About Project:
A project that extends the Flask project [dogs_flask_test_02]. This project is meant to enable usage of html elements from [Google's Material Design 3](https://m3.material.io/) system.

### Started On:
:calendar: December 28, 2023 *(AUTO-GENERATED)* :calendar:

### Reflections:
I managed to complete this project, but the way the currently-in-development [Material Web 1.0](https://github.com/material-components/material-web) package is set up, this requires the use of a bundling service (rollup is the one I used) that bundles up only the exact scripts used in index.js as well as the code in index.js into a single file (bundle.js), rather than referencing the whole dependency package (so if I only use one or two elements from the material package, through imports in index.js, the bundling functionality removes the need to import large packages, or map stuff, I dont need to reference @material in my index.js, the bundler just moves everything into a bundle.js that can be shipped without explicit references to dependenices. Which is kind of cool!)

### Notable (Milestone) Resources Created:
- Learnt to add Material design elements to web projects that use js, using the [Material Web 1.0](https://github.com/material-components/material-web) from Google.
- Got my first experience with bundling js depedencies for treeshaking.


## PROJECT DIR: dogs_flask_test_04
### About Project:
A project that extends the Flask project [dogs_flask_test_03]. 

This project is meant to add unit tests for the interface layer of the code, as it is its current state. ***Revisions will be needed when the interface is compeleted (at least in the context of having every functionality/attribute required for final MVP server side testing)***

### Started On:
:calendar: December 29, 2023 *(AUTO-GENERATED)* :calendar:

### Reflections:
This was fun. It was a bit worried about the unittest library in Python being too simple, expecially after seeing that pytest seems to be more *advanced* (at first sight). It was nice to discover that might not be the case.

### Notable (Milestone) Resources Created:
- Initial experience with unittest. Now I've gotten a base experience that supports me learning this testing package in at least the context of this code!
- Initial experience with using the beautiful soup scraping framework for testing html code structure and contextual data.


## PROJECT DIR: dogs_flask_test_05
### About Project:
A project that extends the Flask project [dogs_flask_test_04] with service layer unit testing. 


### Started On:
:calendar: December 29, 2023 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_


## PROJECT DIR: dogs_flask_test_06
### About Project:
A project that extends the Flask project [dogs_flask_test_05] with e2e testing. 

### Started On:
:calendar: December 30, 2023 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_


## PROJECT DIR: dogs_flask_test_07
### About Project:
A project that extends the Flask project [dogs_flask_test_06] with improved html. It now has a proper stick header, a proper button inside a sticky button container below the header and a scrollable list below the button and the header.

The interface has been finetuned towards being good-enough.

Tests have been updated to handle the changes (unit and integration).

### Started On:
:calendar: December 30, 2023 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_


## PROJECT DIR: dogs_flask_test_08
### About Project:
A project that extends the Flask project [dogs_flask_test_07] with:
	- Two endpoints:
		- One for initial state of the website ~ header and request ubtton
		- Another that returns a html snippet for the list of dog breeds.
	- Splitting testing to cover both endpoints ~ and ~ extending both endpoint tests to cover the fully developed interface


### Started On:
:calendar: December 30, 2023 *(AUTO-GENERATED)* :calendar:

### Reflections:
Changes are described in this (personal) ChatGPT chat:
- https://chat.openai.com/c/ccf1640d-504d-480e-9394-0cd7a8345b6e

### Notable (Milestone) Resources Created:
_


## PROJECT DIR: dogs_flask_test_09
### About Project:
A project that extends the Flask project [dogs_flask_test_08] with: 
- Moved test files to test folder
- Recreated the venv folder as well as the requirements file.
	- Added a packages4pip.txt file so we can reinstall from scratch again easily. ***Location:docs/pacakges4pip.txt***
- Added an index.html file that interacts with our server endpoints. ***Location: web/index.html***
	- Injects the html from route("/") and then attaches click handler onto the request button that fetches the dog list from route("/renderBreeds").
	- If route("/") fails ~ Injects "Error loading content." into the main html container
	- If route("/renderBreeds") fails ~ Displays user facing snackbar.


### Started On:
:calendar: January 03, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
Need to go over all codepaths and ensure integrity and errorhandling of the process.

### Notable (Milestone) Resources Created:

## PROJECT DIR: dogs_flask_test_10
### About Project:
A project that extends the Flask project [dogs_flask_test_09] with: 
- Refactored structure.
- Config file based on env variables.
- Injection of services.


### Started On:
:calendar: January 03, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_
## PROJECT DIR: dogs_flask_test_11
### About Project:
A project that extends the Flask project [dogs_flask_test_10] with: 
 - Selenium testing

### Started On:
:calendar: January 03, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
Probably gonna need some feed some config variables to the selenium script later in the delvelopment process.

### Notable (Milestone) Resources Created:
_

## PROJECT DIR: dogs_flask_test_12
### About Project:
A project that extends the Flask project [dogs_flask_test_11] with: 
- Completed implementing 
	- Digital signing of server responses
	- Verification of server responses in index.html
- Completed middleware for selenium tests
	- Delay middleware
	- Error middleware
	- Invalid signature middleware
- Finished writing the selenium tests module
	- Still need to decouple the index.htmls used for testing from that.
		- Just need to create a simple script that creates a index file for each test from a template and injects the correct middleware proxy url into the index template file.

- Some edits to the html as well.


### Started On:
:calendar: January 09, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_


## PROJECT DIR: dogs_flask_test_13
### About Project:
A project that extends the Flask project [dogs_flask_test_12] with: 
- PEM Private key variable is not hardcoded anymore.
- Also aligned the initial template to the php and c++ projects

### Started On:
:calendar: January 10, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_


## PROJECT DIR: dogs_flask_test_14
### About Project:
A project that extends the Flask project [dogs_flask_test_13] with: 
- Sanitation of input from external dog breed service.
  - Tests for sanitation code

### Started On:
:calendar: January 10, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_


## PROJECT DIR: dogs_flask_test_15
### About Project:
A project that extends the Flask project [dogs_flask_test_14] with: 
- Slightly increased level of code commenting

### Started On:
:calendar: January 11, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_


## PROJECT DIR: dogs_flask_test_16
### About Project:
A project that extends the Flask project [dogs_flask_test_15] with: 
- Specific CORS settings.

### Started On:
:calendar: January 11, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_


## PROJECT DIR: dogs_flask_test_17
### About Project:
A project that extends the Flask project [dogs_flask_test_16] with:
- Added a gitignore file
- Added viewport meta tag to head of the template index html file for responsive design

### Started On:
:calendar: January 12, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_



## PROJECT DIR: dogs_flask_test_18
### About Project:
A project that extends the Flask project [dogs_flask_test_17] with:
- Removed the following from the project and moved to its own project DogDisplayGhClient, (re)moved:
	- The web/index.html file
	- The selenium_tests folder
	- Dependencies and scripts from the package.json file
	- Dependencies from the python project (selenium)
	
- Set CORS to only allow only connections from localhost.


### Started On:
:calendar: January 12, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_


## PROJECT DIR: dogs_flask_test_19
### About Project:
A project that extends the Flask project [dogs_flask_test_18] with:
- Cleaned comments and prepped for push
- Wrote readme.md
- FINAL LOG ITEM IN THIS FILE:
	- Moved versioning to GitHub, a public versioning system.
		- [PythonDogDisplay](https://github.com/mittons/PythonDogDisplay)
	- This project is part of a larger system. I also created overview for that and linked this project there
		- [DogDisplayOverview)(https://github.com/mittons/DogDisplayOverview)


### Started On:
:calendar: January 13, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_


