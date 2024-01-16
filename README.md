# DogDisplayOverview

### **Welcome to the DogDisplayOverview Repository!**

## Table of Contents
- [Introduction](#introduction)
- [Projects Overview](#projects-overview)
- [Roadmap](#roadmap)
- [Data Source](#data-source)
- [Contact](#contact)

## Introduction

**Purpose of the Repository:** This repository is a both a professional demonstration of my development capabilities, as well as a personal self-documentation/self-review journey of my learning experience over (atleast) a month, as I refresh and refine my skillset after a significant period off from actively programming.

**Profesionally**, this repository serves as an simplified entry point to a portfolio consisting of a series of projects that present both a snapshot of my current active skillset, as well as demonstrating my potential capacity for learning and growth over a short period of time. This repository as well as the projects should also demonstrate my ability to incrementally leverage the technology, understanding and resources that I have access to, in order to achieve both added value and further potential for growth.

**Personally**, this repository serves as a way to review and document what I have learnt during this time as well as to review and refine my learning processes.

I hope this portfolio also demonstrates my passion for learning, growth and building stuff!

*I also really like transparency!*

*I will add to this overview repository incrementally over a few days, or a week or two. (or three).*


**The majority of Projects** in this repository share a **common functionality** at their first and final major release, while utilizing different techonlogies for implementation.

At **1.0.0+** the major projects have:
- A **Service Layer** that is responsible for fetching data from a an external service.
- A **Presentation/Interface Layer** that initally displays a simple header, and below it a request data button. Once the request data button is pressed the application enters a **state transition**, requests data through the service layer and displays a circular loading indicator until the request is resolved. Generally there are only two outcomes as a result of this transition:
    1. **Success:** Displays a list of data in a structured format, fetched from the [The Dog API](https://www.thedogapi.com).
    2. **Error Handling:** In case of request failure, an error snackbar is displayed to inform the user.

- **Unit Tests** for each layer separately
- **Integration/E2E Tests** with both layers
- Push-Build-Test-Deploy **CI/CD process**

## Projects Overview

**List of Projects:** 

 - **C++, PHP and Python Phase** (December 29 2023 to Jan/Feb 2023)
    - [CppDogDisplay 0.1.0](https://github.com/mittons/CppDogDisplay) - Project developed between December 29 2023 and "*"

    - [PhpDogDisplay 0.1.0](https://github.com/mittons/PhpDogDisplay) - Project developed between December 29 2023 and "*"

    - [PythonDogDisplay 0.1.0](https://github.com/mittons/PythonDogDisplay) - Project developed between December 29 2023 and "*"


 - **Angular Phase** (December 22 2023 to December 25 2023)
    - [AngularDogDisplay 1.0+](https://github.com/mittons/AngularDogDisplay01) - Practice project developed between December 22 2023 and December 25 2023

 - **Flutter Phase** (December 09 2023 to December 19 2023)
    - [DoggoDec19 1.0+](https://github.com/mittons/doggoDec19) - Practice project developed on December 19 2023
    - [DoggoDec18 1.0+](https://github.com/mittons/doggoDec18) - Practice project developed on December 18 2023
    - [DoggoDec17 1.0+](https://github.com/mittons/doggoDec17) - Practice project developed on December 17 2023
    - [DoggoDec16 1.0+](https://github.com/mittons/doggoDec16) - Practice project developed on December 16 2023
    - [DoggoDisplay01 1.0+](https://github.com/mittons/doggoDisplay01) - Practice project developed between December 09 2023 to December 13 2023

**Technology Stack:** These projects touch on the following languages/frameworks: 
- Flutter/Dart
- Angular/TypeScript
- Python/Flask
- C++/crow
- PHP/Laravel
- Node.js
- Bash
- Docker
- C#
- GitHub Actions

## Roadmap

For this repository, the following developments are planned/considered:

- [ ] **Development Journey:** Document the learning and decision making process in sequence.
- [ ] **Learning Milestones:** Identify major areas of new knowledge and understanding.
- [ ] **Challenges/Solutions:** Include sections on setup requirements, usage instructions for running, and testing.
- [ ] **Skills Acquired:** Define aquired skills that were explicitly demonstrated in the projects.
- [X] **Personal Logs/Journals Archived:** I may include *(mostly)* unsanaitized copies of my personal learning journal, as well as the ad-hoc versioning changelog I used for each project before I wanted to subject it to public version control systems (i.e. before minimum viable product).
- [ ] **Further Reflections:** Reflect on my decisions, my strategy, how I can build on the experience and assets gained from these projects, and draw conclusions. Among other things.  

## Data Source

- **The Dog API:** The applications in this portfolio use data from [The Dog API](https://www.thedogapi.com). I route the traffic through my own private backend proxy in order to secure my user key for the API, in line with the [The Dog API TOS](https://thedogapi.com/terms).

## Contact

Axel Gauti Guðmundsson - [@axelgauti](https://twitter.com/axelgauti) - axel@axelgauti.is