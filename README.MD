# Project WAFS :gear:

_Shields that represent my project - They change over time._

![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square) ![Activity](https://img.shields.io/github/last-commit/TristanVarewijck/TechDefined) ![Isseus](https://img.shields.io/github/issues/TristanVarewijck/TechDefined) ![Language](https://img.shields.io/github/languages/top/TristanVarewijck/TechDefined) ![Count](https://img.shields.io/github/languages/count/TristanVarewijck/TechDefined?color=#a55eea) ![NPM](https://img.shields.io/npm/v/npm) ![MIT-License](https://img.shields.io/apm/l/vim-mode)

## TechDefined Concept Design :pencil2:

![TechDefined-concept-design](https://github.com/TristanVarewijck/TechDefined/blob/main/assets/images/concept-display.png)

## Live Demo :clapper:

See the latest updated demo here:
[Link to DEMO](https://tristanvarewijck.github.io/TechDefined/)

:rotating_light: **WARNING** :rotating_light: <br>
API does not work in the live-demo to see the full experience of this app, make sure to clone it locally and run in on your localhost.

To get acces on the full API make sure to see their [pricing scheme](https://newsapi.org/pricing).

---

## Description :label:

For the project WAFS (Web Application from Scratch) I'm going to make a "single page" tech-news app.
On the app you can see the most relevant articles in the tech world, in addition, you have suggested search results and you can search for articles on a specific topic. For the project i am using the NewsAPI.

---

## Table of Contents :arrow_right_hook:

- [Features](#features)
- [Activiy] (#activitydiagram)
- [API](#api)
- [ToDoList](#todolist)
- [Usage](#Usage)
- [Meta](#meta)
- [License](#license)

---

## Features

:chains: Features for this app are mainly still under construction.

1. **Search** <br>
   Search for the Topics you are interested from over the whole World.
2. **Endless scroll** <br>
   Scroll trough endless articles related to your topic or scroll to the headlines of this current day!
3. **Sharing** <br>
   Share articles on Twitter.
4. **Text to Speech** <br>
   With the Text to Speech Feature you can have it read to you instead of reading it yourself.
5. **Suggested Topics** <br>
   With the filter-buttons your can search on topics that are suggested by the App.
6. **Read more** <br>
   Clicking on the banner of the article will bring your to the detail page where can read more about it.

---

## Activity Diagram

Here you can see 2 activity diagrams on usual behaviours of the user of this app.

1. Default Diagram <br>
   <img src="https://github.com/TristanVarewijck/TechDefined/blob/main/assets/images/Default-flow.png" alt="default-flow" width="600px"/>

2. Search Diagram + (error) <br>
   <img src="https://github.com/TristanVarewijck/TechDefined/blob/main/assets/images/Search-flow.png" alt="search-flow" width="600px"/>

## API

<img src="https://github.com/TristanVarewijck/TechDefined/blob/main/assets/images/newApi-LOGO.jpeg" alt="newsapi-logo" width="200px"/>

For this project i am using the NewsAPI from - [NewsAPI](https://newsapi.org/) <br>
To search on the app im using the endpoints below with the following params:

This one is so i can search articles for specific topics:
[https://newsapi.org/v2/everything](https://newsapi.org/v2/everything)

|  Key  |    q    |   sortBy    | language | pageSize |  apiKey  |
| :---: | :-----: | :---------: | :------: | :------: | :------: |
| value | {input} | publishedAt |    en    |   100    | {apiKey} |

this one is so i can see the latest headlines in a specific category:
[https://newsapi.org/v2/headlines](https://newsapi.org/v2/headlines)

|  Key  | country |  category  | pageSize |  apiKey  |
| :---: | :-----: | :--------: | :------: | :------: |
| value |   us    | technology |   100    | {apiKey} |

:rotating_light: : As explained earlier the API is not usable outside your localhost, for this project i used the **FREE version** of this API.

---

## ToDoList

In addition to the features that are now available, there are also additional features and tweaks that can make the app better. Do you have ideas let them know in a [PR](https://github.com/TristanVarewijck/TechDefined/pulls) :white_check_mark:

- [x] Detail pages (data)
- [ ] Locomotive scroll testing
- [ ] Working filter buttons
- [x] JS refactoring
- [ ] Keep-scroll position
- [x] No refresh on page switch
- [ ] Reponsiveness

---

## Usage

For using this app yourself you need to follow the following steps:

### 1. Clone Repo locally

```
git clone https://github.com/TristanVarewijck/TechDefined.git
```

### 2. Connect your API key

If you want to connect with the API you have to fill in your own personal {apiKey} wich you can get here: <br>
[Get NewsAPI apiKey](https://newsapi.org/).

```
https://newsapi.org/v2/everything?q=${input.value}&sortBy=publishedAt&language=en&pageSize=100&apiKey=${apiKey}
https://newsapi.org/v2/top-headlines?country=us&category=technology&pageSize=100&apiKey=${apiKey}
```

### 3. Run on Localhost

Because i am using the free version of this API your need to run it on your localhost to test it. If you want to move further with this app make sure to check out the [pricing scheme](https://newsapi.org/pricing) of NewsAPI.

For easily running this project on your localhost you can use a VSCODE extension named: <br>
[live-server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)

After installing this extension make sure to reload en hit the "Go Live" button.

### Thats it! :smile:

---

## Meta

Tristan Varewijck <br>
:email: [Tristan.varewijck@gmail.com](Tristan.varewijck@gmail.com) ||
:large_blue_diamond: [https://www.linkedin.com/in/tristanvarewijck-1999/](https://www.linkedin.com/in/tristanvarewijck-1999/)

![Ask Me Anything !](https://img.shields.io/badge/Ask%20me-anything-1abc9c.svg)

---

## License

Usage is provided under the [MIT License](https://github.com/git/git-scm.com/blob/master/MIT-LICENSE.txt) MIT. See [LICENSE](https://github.com/TristanVarewijck/TechDefined/blob/master/LICENSE) for the full details.
