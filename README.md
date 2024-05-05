# DogDisplayOverview

### **Welcome to the DogDisplayOverview Repository!**
This is a curated showcase of diverse projects, each reflecting a unique blend of technologies and methodologies. This collection not only demonstrates my technical skills but also unfolds the narrative of my evolving learning journey, offering insights into the development process and my personal growth as a developer.

Seek the 🎯 icon for my latest projects, showcasing the most refined and polished work! Projects tagged with 💯 feature the most comprehensive functionalities.

## Table of Contents
- [Introduction](#introduction)
- [Projects Overview](#projects-overview)
- [Technology Stack](#technology-stack)
- [Roadmap](#roadmap)
- [Acknowledgements](#acknowledgements)
- [Contact](#contact)

## Introduction

**Purpose of the Repository:** This repository is a both a professional demonstration of my development capabilities, as well as a personal self-documentation/self-review journey of my learning experience over (atleast) a month, as I refresh and refine my skillset after a significant period off from actively programming.

**Profesionally**, this repository serves as an simplified entry point to a portfolio consisting of a series of projects that present both a snapshot of my current active skillset, as well as demonstrating my potential capacity for learning and growth over a short period of time. This repository as well as the projects should also demonstrate my ability to incrementally leverage the technology, understanding and resources that I have access to, in order to achieve both added value and further potential for growth.

**Personally**, this repository serves as a way to review and document what I have learnt during this time as well as to review and refine my learning processes.

I hope this portfolio also demonstrates my passion for learning, growth and building stuff!

*I also really like transparency!*

## Projects Overview

**The majority of Projects** in this repository share a **common functionality** at their first and final major release, while utilizing different techonlogies for implementation.

At **1.0.0+** the major projects have:
- A **Service Layer** that is responsible for fetching data from a an external service.
- A **Presentation/Interface Layer** that initally displays a simple header, and below it a request data button. Once the request data button is pressed the application enters a **state transition**, requests data through the service layer and displays a circular loading indicator until the request is resolved. Generally there are only two outcomes as a result of this transition:
    1. **Success:** Displays a list of data in a structured format, fetched from the [The Dog API](https://www.thedogapi.com).
    2. **Error Handling:** In case of request failure, an error snackbar is displayed to inform the user.

- **Unit Tests** for each layer separately
- **Integration/E2E Tests** with both layers
- Push-Build-Test-Deploy **CI/CD process**

**List of Projects:**

 - **Client phase** (January 03 2024 - *Feb*/**Mar**/***Apr*** 2024)

    -🎯 [DogDisplayStaticClient 0.1.0](https://github.com/mittons/DogDisplayStaticClient) - Project developed between January 03 2023 and "*"


 - **C++, PHP and Python Phase** (December 29 2023 to Jan/Feb 2023)
    
    -🎯 [DogDisplayForCpp 0.2.1](https://github.com/mittons/DogDisplayForCpp) - Project developed between December 29 2023 and "*"

    -🎯 [DogDisplayForPhp 0.2.1](https://github.com/mittons/DogDisplayForPhp) - Project developed between December 29 2023 and "*"

    -🎯 [DogDisplayForPython 0.2.1](https://github.com/mittons/DogDisplayForPython) - Project developed between December 29 2023 and "*"


 - **Angular Phase** (December 22 2023 to December 25 2023)
    
    -💯 [AngularDogDisplay 1.0+](https://github.com/mittons/AngularDogDisplay01) - Practice project developed between December 22 2023 and December 25 2023

 - **Flutter Phase** (December 09 2023 to December 19 2023)
    
    -💯 [DoggoDec19 1.0+](https://github.com/mittons/doggoDec19) - Practice project developed on December 19 2023
      - 💯 [MockDogApiDec19](https://github.com/mittons/MockDogApiDec19) - Limited mock of the external data service, developed on December 19 2023

    -💯 [DoggoDec18 1.0+](https://github.com/mittons/doggoDec18) - Practice project developed on December 18 2023
      - 💯 [MockDogApiDec18](https://github.com/mittons/MockDogApiDec18) - Limited mock of the external data service, developed on December 18 2023
    
    -💯 [DoggoDec17 1.0+](https://github.com/mittons/doggoDec17) - Practice project developed on December 17 2023
      - 💯 [MockDogApiDec17](https://github.com/mittons/MockDogApiDec17) - Limited mock of the external data service, developed on December 17 2023
    
    -💯 [DoggoDec16 1.0+](https://github.com/mittons/doggoDec16) - Practice project developed on December 16 2023
      - 💯 [MockDogApiDec16](https://github.com/mittons/MockDogApiDec16) - Limited mock of the external data service, developed on December 16 2023
    
    -💯 [DoggoDisplay01 1.0+](https://github.com/mittons/doggoDisplay01) - Practice project developed between December 09 2023 to December 13 2023
      - 💯 [MockDogApi01](https://github.com/mittons/MockDogApi01) - Limited mock of the external data service, developed between December 09 2023 to December 13 2023

## Technology Stack 
The projects in this portfolio either touch directly or indirectly on the following languages, frameworks, tools and technology:
- Flutter/Dart
- Angular/TypeScript
- Python/Flask
- C++/crow
- PHP/Laravel
- Node.js
- Bash
- Powershell
- Docker
- C#
- GitHub Actions
- Git
- Markdown
- Windows
- Linux
- VS Code
- **ChatGPT**

## Roadmap

*I will add to this overview repository incrementally, and develop it, over the first few weeks after it's initial commit.*

For this repository, the following developments are planned/considered:

- [X] **Rest:** Take a break from these projects and most other things for 2-3 weeks, until around the 7th of March 2024, or a bit earlier. These projects are mostly well defined, scoped and ready. PoC for a simple output of this project can be found in the [PoC_markdown_documents](PoC_markdown_documents) folder.

- [ ] **Formally start building the end result:** Declare final phase of these projects. Define first level breakdown of it's steps and offer enough context to give the phase a limited scope.

- [ ] **Development Journey:** Document the learning and decision making process in sequence.
- [ ] **Learning Milestones:** Identify major areas of new knowledge and understanding.
- [ ] **Challenges/Solutions:** Include sections on setup requirements, usage instructions for running, and testing.
- [ ] **Skills Acquired:** Define aquired skills that were explicitly demonstrated in the projects.
- [X] **Personal Logs/Journals Archived:** I may include *(mostly)* unsanaitized copies of my personal learning journal, as well as the ad-hoc versioning changelog I used for each project before I wanted to subject it to public version control systems (i.e. before minimum viable product).
- [ ] **Further Reflections:** Reflect on my decisions, my strategy, how I can build on the experience and assets gained from these projects, and draw conclusions. Among other things.  
- [ ] **Wrap up:** Finalize the project by stating its intent and setting up my next projects.

## Acknowledgements

- **The Dog API:** The applications in this portfolio use data from [The Dog API](https://www.thedogapi.com). I route the traffic through my own private backend proxy in order to secure my user key for the API, in line with the [The Dog API TOS](https://thedogapi.com/terms).

- **ChatGPT:** Powered by OpenAI, specifically ChatGPT-4. Files in this project and files the portfolio it represents vary between being Content that is completely AI generated to being completely human-generated. The term Content, and other relevant definitions, can be observed on [The OpenAI TOS page](https://openai.com/policies/terms-of-use#using-our-services).
   - For reference: 
      - The first Flutter project from December 9th does not include any fully AI generated texts, but relied on cooperative efforts from AI. Each of the Flutter projects from between December 16th and December 19th increased the volume on human-generated content, and at December 19th every line, and all intended functionality, was processed and output by a human.
      - The Angular project is mostly human-generated.
      - The C++, PHP and Python vary heavily from file to file, from being completely AI generated to completely human-generated.

## Contact

Axel Gauti Guðmundsson - [@axelgauti](https://twitter.com/axelgauti) - axel@axelgauti.is
