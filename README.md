# appcom README Styleguide

This document aims at giving an introduction to README files and thus documentation in general. We argue why README files are important and give a basic idea on how to start writing and them and what to include. If you want to help crafting this document please refer to the [contributing section](#contributing).

## Table of Contents

1. [Quotes](#quotes)
1. [Why does your project need a README?](#why-does-your-project-need-a-readme?)
1. [How to write great READMEs](#how-to-write-great-readmes)
1. [Tipps](#tipps)
1. [Further reading](#further-reading) 
1. [Contributing](#contributing)
1. [License](#license) 

## Quotes
This section serves only one purpose: convince you of the need of a README! 

* "Once 6 months pass, a module without documentation begins to look new and unfamiliar." - https://github.com/noffle/art-of-readme
* "No README means developers will need to delve into your code in order to understand it." - https://github.com/noffle/art-of-readme
* By the same principle a beautifully crafted library with no documentation is also damn near worthless. If your software solves the wrong problem or nobody can figure out how to use it, there’s something very bad going on - http://tom.preston-werner.com/2010/08/23/readme-driven-development.html
* Also, end-user documentation is best when it doesn't assume that the user has any prior knowledge. The point in time when I'm closest to perfect lack of knowledge about something is before I've built it[2]. So, that's the best time to document it. - http://joeyh.name/blog/entry/documentation_first/
* It is a truth universally acknowledged that a developer in possession of a good program must be in want of good documentation. - https://www.hpe.com/us/en/insights/articles/how-to-write-documentation-thats-actually-useful-1707.html

**[back to top](#table-of-contents)**

## Why does your project need a README?
For starters see the "Random quotes" section. Not convinced yet? Here are some more reasons why your projects need a README.md:

* A README is a developers first look into your creation
* When handing out a piece of software without a README another developer is (likely) not able to run or develop it 
* Starting out with a README.md forces you to focus on structure. May help you crafting an idea for the implementation
* A README file acts as a table of contents for your most important information of your software (far better than a fully crafted documentation)
* Arguing about something is way easier when it is written down somewhere. That is what your README is for!

There are several more reasons why a README is important. Please add more (see [contributing section](#contributing))

**[back to top](#table-of-contents)**

## How to write great READMEs
Before you start writing your README file we want to given an idea what your README file is for. By the same token we want to state what your README shouldn't do.

### What your README file should do
Your README always refer to a piece of software (**it**) and describes it to the outside world (i.e. other developers, users, clients - **them**). It should

1. tell them what it is (with context)
2. show them what it looks like in action
3. show them how they run and use it
4. tell them any other relevant details

### What your README file shouldn't do
It should not

* include every detailed information about your project. There are other documents that serve that purpose

### Structure
The structure of your README varies on the type of software it is describing. First we define the types of software and give a basic structure for every one of them

#### Module / Library
A piece of software, which is developed for others to use in their own projects / modules / libraries. Running it on its own is often useless. So you rely on others to use it. The structure of your README should reflect that!

| Name | Description | Required |
|:-|:-|:-|
| Introduction | Describe briefly what your software is. What problem does it solve? At what target audience is it aimed? | Yes |
| Usage | Show how to use it with a code example. Focus on the key features and do not include too much (that is for the Wiki). Also do not delve into the API to much. We'll get to that | Yes |
| API | Describe the API of your module / library such that other developers know how to interact with it. | Yes |
| Installation | Briefly describe how other developers can use your library. Make it as short as possible and rely on package managers (e.g. npm, conan, gradle, ...). Assume that they are known when refering to your target (developer) audience. | Yes |
| License | Describe the license under which your software is published. Note that an unlicensed piece of software is most likely never used. So do not skip tihs part! | Yes |

#### Solution Project (App, Website, ...)
A solution project is a piece of software, which is often aimed at a user and not a developer. It is often meant to run alone (or together with a backend server) and often does not require other dependencies. Also in general there are binaries out there (e.g. Github, Google Play, iTunes Connect, ...) to run it on a target device. On your README you should emphasize what this project does and how to run it locally on your machine, such that one can add features and fix bugs (and more).

| Name | Description | Required |
|:-|:-|:-|
| Introduction | Describe briefly what your software is. What problem does it solve? At what target audience is it aimed? | Yes |
| Overview | Give an architectural overview of your software. Is is interesting for other developers, who wants to catch on and want to developer features or fix bugs of your software. Do not go into too much detail. There are other documents for this. | Yes |
| Development | If you software is developed within a team you shhould include this section. Describe how to setup thhe project. Include dependencies, conventions and other things to know in order to start developing. In short: After reading this section everyone should be able to develop this piece of software. | Yes |
| Changelog | Describe that changes made to the software by version. Note that this should be done automatically. | No |
| License | Describe the license under which your software is published. Note that an unlicensed piece of software is most likely never used. So do not skip tihs part! | Yes |


#### Styleguide
This type of software is often not an actual software but just a set of documents describing what you should do or shouldn't do in a specific context (e.g. developing a piece of software). 

| Name | Description | Required |
|:-|:-|:-|
| Introduction | Describe what this document refers to. At what target audience is it aimed? | Yes |
| Table of contents | This shows what sections are covered in this document and gives the reader the possibility to jump to a specific section. It is highly recommended to use a TOC. | No |
| Content | This the actual content. | Yes |
| Related work | This section covers related works, further readings and tools that might be relevant or interesting for the reader. | No |
| License | Describe the license under which your software is published. Note that an unlicensed piece of software is most likely never used. So do not skip tihs part! | Yes |

**[back to top](#table-of-contents)**

## Tipps

**[back to top](#table-of-contents)**

## Further reading
* [Art of README](https://github.com/noffle/art-of-readme) - Covers basics. Slightly biased on node modules, but still relevant
* [README Driven Development](http://tom.preston-werner.com/2010/08/23/readme-driven-development.html)
* [JoeyH Blog](http://joeyh.name/blog/entry/documentation_first/)

**[back to top](#table-of-contents)**

## Contributing

You can help improve this document by making it more coherent, consistent, or readable, adding missing information, correcting factual errors, fixing typos, or bringing them up to date.

To do so, make changes to the source files (i.e. this very document). Then open a pull request to apply your changes to the master branch.

**[back to top](#table-of-contents)**

## License

Copyright 2019 appcom interactive GmbH

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

**[back to top](#table-of-contents)**