# Maintaining & Enhancing [Mythic C2](https://github.com/its-a-feature/Mythic/)


## Introduction

This repository is a collection of `knowledge` related to the `Mythic C2 Framework` documentation, planning, code snippets, and other resources related to my attemps at maintaining and enhancing `Mythic` for my own entertainment .

## Purpose

The purpose of this repository is to provide a *central location* for all of the `information` & `experience` I have gathered while working on maintaining `Mythic`.



The goal is to be able to use the writing in this, primarily markdown based repository is to enhance the output of LLMs when prompting them in relation to development, testing, and deployment of `Mythic`.


Intentions 

I intend to spend a significant amount of time building on my own fork of Mythic, the C2 framework. 

As it stands, Mythic is more of a C2 & post exploitation framework. It is typically brought into play after recon has already been preformed during an offensive operation.

I feel the design of Mythic, such as:

- being a containerized, micro-service based system that allows you to develop on top of the existing Mythic systems with ease
- The advanced & detailed documentation
- The use of react + Nginx as a transparent proxy for communication between containers and the UI allowing for data to be displayed from a variety of sources means we can build on top of the existing system without needing to refactor much
- The use of standardized formatting & data type definitions to ensure consistency and compatibility when passing data across multiple services makes sure that we are developing tooling compatible with the base framework
- The ability to install and remove services mid operation ensures maximum performance
- The use of Git & GitHub to install and manage services and modules is both impressive and useful for making the system customized to each user’s environment.

The goal is to extend the library of community tooling for the Mythic Framework, while providing extremely detailed documentation on how to use said tooling 

## Breaking it Down

### System Design

Our first focus is on understanding the Mythic Framework as it exists. For this we will create a clone of the repository and preform detailed analysis of the code as well as the documentation.

 My goal is to alternate between studying the code & then looking at the documentation for that code 

- At the time of writing the Mythic Framework is on version 3.3

I have a variety of plans for how I intend to improve Mythic, so let’s dive into that

1. focus on intelligence & information gathering in terms of global events, news, standard cyber threat intel feeds, etc. we want to focus a whole portion of our development efforts into refactoring the systems database to ensure proper representation of events and how they relate to other artifacts in the database 
2. That brings us to 2, focusing on enhancing the database schema and adding better representation of more complex objects within the realm of offensive cyber security. In the world of cybersecurity, having the most information with the most context allows you to preform the best overall analysis of a situation. The better access to accurate information & proper use of analytics based on that information leads to long term reproducible success. This all starts with saving data in the most effective way possible to build the best picture of your environment and situation 
3. Focus on enhancing the information ingestion methods. More tools for writing data to the database. 
4. See what can be done to enhance the nemesis data pipeline tooling 
    1. NOTE: make sure database is highly compatible with nemesis 
    2. Build on nemesis around the database 
5. Following up, would be developing recon related modules for Mythic. I think focusing on both human & network recon to start is a good idea. Business & industry intelligence next, then maybe scale to geopolitical stuff idk. I would like to see how large we can scale this
    1. Networking tools
        1. Project discovery 
            1. Make use  of the wide variety of network recon tools created by the project discovery organization to gather & return data that can be used within the mythic framework by writing the wide range of information gathered to the Postgres database 
6. Add additional listeners.
    1. Im interested in adding additional protocols to the list of available protocols that can be used as listeners
        1. Tox messaging protocol based listener interface 
    2. Add more listeners compatible with Mythic instances running behind a NAT
7. Add new “agents”
8. Integrate AI within reason. Any use of AI/ML will have to meet certain requirements to be considered for inclusion. This is to avoid “bullshit bloat” features that are gimmicky and easy to forget about. **The goal is to make life easier, not spend time learning something just to decide it was not worth it.**
    1. General qualifications For a feature: 
        1. Focuses on amplifying existing intelligence. RAG style models, ideally with access to search engines would be ideal when using anything related to the current generative AI hype. Avoid standard LLMs that have not been given contextual data, such as mythics internal documentation container
    2.  We want anything we integrate into the platform to be “mythic AI”, not “mythic + chatGPT”, as in it must be tailored to Mythic for it to be worthwhile. 
    3. Qualifications for a technology/model related to AI/ML
        1. Must be Open source (ideally Ollama or hugging face)
        2. Must be self host-able / able to be run locally
    4. Generally speaking I do not intend to generate the standard chatbot interface that is becoming so common. It is cool but slow on My hardware.
        1. Instead we aim to use any advanced demanding models to preform slow and detailed functions like advanced research and report generation.calculations and analysis of data, documentation and more to create a report by outlining the plan 
            1. iteratively edit, review revise and repeat to create advanced reports with citations similar to storm
                1. https://github.com/stanford-oval/storm - An LLM-powered knowledge curation system that researches a topic and generates a full-length report with citations. | this is what we are looking to create if we use LLMs 
                2. 

 

## General Goals & Principles of Development

We want to seamlessly integrate into the existing Mythic Framework. The ultimate goal is to build on top of what exists in a detailed and comprehensive way. We do not want to move too quickly in a way that leaves us with “loose ends” in the codebase, leading to improper use of features or not maximizing the potential capability of an existing feature as we enhance the framework.

 The plan is to develop in a slow, iterative process, taking detailed note of what exists and what we intend to change BEFORE changing anything. We want to be addressing real problems and creating new features not chasing down problems we created. 

### Development tooling

#### 1. Github

- Make use of issues & projects to plan out features in detail.
- Make use of multiple repositories as the mythic framework already does but keep documentation centralized to one repository using the dendron alternative Foam (the vscode extension for working with markdown)
- Copilot to reference issues & enhance the code base
- 

#### 2. LLMs 

##### 2.1. Ollama 

- use Ollama + open ui to run long term questions and analysis of the project.

#### 3. VSCode

#### 4. Markdown documentation 

---

---

---

how to improve on mythic
