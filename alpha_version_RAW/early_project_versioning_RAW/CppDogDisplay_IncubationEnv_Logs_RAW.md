# doggoCPP - Project Folder Index

## PROJECT DIR: _archive
### About Project:
_

### Started On:
:calendar: January 05, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_


## PROJECT DIR: _clutter
### About Project:
_

### Started On:
:calendar: January 09, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_


## PROJECT DIR: docs
### About Project:
Docs for these projects

### Started On:
:calendar: January 01, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_


## PROJECT DIR: doggoCPP_01
### About Project:
First iteration of my dog breed list display parctice project in C++.

This project just has the nessecary setup to route json data from one endpoint to another.

It has a seperate service layer and a interface/presentation layer.
- Service layer fetches data from external REST api
- Presentation/interface layer exposes the data on another endpoint.

### Started On:
:calendar: December 30, 2023 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_

## PROJECT DIR: doggoCPP_03
### About Project:
A project that extends [doggoCPP_01] and develops upon it. 

It adds/develops two things:
- Html templates and template rendering, using inja.
- Package mgmt: Now uses conan and conanfiles for package management.

### Started On:
:calendar: January 01, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
- Learning about conan and conanfiles. It seems to be much faster/more compact than vcpkg.
- Finding inja. Inja saved the day. It was the template renderer that finally worked.


## PROJECT DIR: doggoCPP_04
### About Project:
A project that extends [doggoCPP_03] and develops upon it.

It now provides two different endpoints for requesting rendered html.
- One that serves the initial site with the header and the request dog breeds button. (This endpoint is also set to return utf-8 formatted data. For the emoji in the header).
- Another endpoint that serves the dog breeds data rendered in html format.

It also provides an endpoint for the static js file.

### Started On:
:calendar: January 02, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_


## PROJECT DIR: doggoCPP_05
### About Project:
A project that extends [doggoCPP_04] and develops upon it.

Added CORS functionality to the static/js/bundle.js route.

### Started On:
:calendar: January 02, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_


## PROJECT DIR: doggoCPP_06
### About Project:
A project that extends [doggoCPP_05] and develops upon it.

Refactors the whole project into more modular units.
-Allows for dependency injection
-Adds test files
	- Enables the service layer unit test file (without real test code)
	- Enables a "all test" executable as well (should run all tests)

### Started On:
:calendar: January 05, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
This was a doozie to perform.

### Notable (Milestone) Resources Created:
_


## PROJECT DIR: doggoCPP_07
### About Project:
A project that extends [doggoCPP_06] and develops upon it.

Fully implements error handling in the DogBreedService class.
Implements the first actual test in the DogBreedServiceTests class.

### Started On:
:calendar: January 05, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_

## PROJECT DIR: doggoCPP_08
### About Project:
A project that extends [doggoCPP_07] and develops upon it.

Fully impliments the tests in the classes:
- DogBreedServiceTests
- RouteTests
- EndToEndTests
Also adds a AllTests executable to the project that runs all of the tests from each of the three test suites at once.

### Started On:
:calendar: January 05, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_

## PROJECT DIR: doggoCPP_09
### About Project:
A project that extends [doggoCPP_08] and develops upon it.

- Split the CMakeLists.txt file into subdirectories.

### Started On:
:calendar: January 09, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_


## PROJECT DIR: doggoCPP_10
### About Project:
A project that extends [doggoCPP_09] and develops upon it.

Adds a SigningService class that has a sign_data function.
- The sign data digitally signs the data that is passed to it using a python script.

Also aligned the initial template to the python and php projects

### Started On:
:calendar: January 10, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_


## PROJECT DIR: doggoCPP_11
### About Project:
A project that extends [doggoCPP_10] and develops upon it.

Connected the data signature class, SigningService, to the main code.
- And verified that everything works.

Also added cors headers to all responses on currently implemented routes.

Set the CMakeLists file to move the signing script to the build directory from the src directory.

### Started On:
:calendar: January 10, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_

## PROJECT DIR: doggoCPP_12
### About Project:
A project that extends the project [doggoCPP_11] with:
- Sanitation of input from external dog breed service.
  - Tests for sanitation code

### Started On:
:calendar: January 11, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_

## PROJECT DIR: doggoCPP_13
### About Project:
A project that extends the project [doggoCPP_12] with:
- Removed unused code
- Made the tests on the index route a bit more fine grained
- Cleaned comments in code
- Cleaned code
- Updated static js file
- Changed external service url from hardcoded value to a config value

### Started On:
:calendar: January 11, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
I feel like I have seen enough testing patterns to be just about to be ready to abstract my testing implementation and modularize them. This is great!

### Notable (Milestone) Resources Created:
I learnt more about MACROs in c++, how they impact the code that is executed (e.g. IFDEF and IFNDEF) and how to utilize them in my code and builds.


## PROJECT DIR: doggoCPP_14
### About Project:
A project that extends the project [doggoCPP_13] with:
- Specific CORS settings.

### Started On:
:calendar: January 11, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_


## PROJECT DIR: doggoCPP_15
### About Project:
A project that extends the project [doggoCPP_14] with:
- Added a gitignore file
- Added viewport meta tag to head of the template index html file, and web/index.html file, for responsive design

### Started On:
:calendar: January 12, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_



## PROJECT DIR: doggoCPP_16
### About Project:
A project that extends the project [doggoCPP_15] with:
- Set CORS to only allow only connections from localhost

### Started On:
:calendar: January 12, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_


## PROJECT DIR: doggoCPP_17
### About Project:
A project that extends the project [doggoCPP_16] with:
- Added 3rd party license file
- Cleaned comments and prepped for push
- Wrote readme.md
- FINAL LOG ITEM IN THIS FILE:
	- Moved versioning to GitHub, a public versioning system.
		- [CppDogDisplay](https://github.com/mittons/CppDogDisplay)
	- This project is part of a larger system. I also created overview for that and linked this project there
		- [DogDisplayOverview)(https://github.com/mittons/DogDisplayOverview)

### Started On:
:calendar: January 13, 2024 *(AUTO-GENERATED)* :calendar:

### Reflections:
_

### Notable (Milestone) Resources Created:
_



