# Python Dungeon Crawler

This project was created as an introduction to Python, mainly to learn the syntax and play around with libraries within the language. It was originally a project assigned from Lambda School, however the project has evolved, and I now regularly make commits to add more functionality to the game.


## Contributors

|                                       [Jordan Christensen](https://github.com/mazjap)                                                 |
| :-------------------------------------------------------------------------------------------------------------------------:           |
| [<img src="https://avatars0.githubusercontent.com/u/24785257?s=460&v=4" width = "300" />](https://github.com/mazjap)                  |
| [<img src="https://github.com/favicon.ico" width="15"> ](https://github.com/mazjap)                                                   |
| [ <img src="https://static.licdn.com/sc/h/al2o9zrvru7aqj8e1x2rzsrca" width="15"> ](https://www.linkedin.com/in/jordan-a-christensen/) |

[![Python Version][python-image]][python-url]
[![Build Status][travis-image]][travis-url]
[![License][license-image]][license-url]

## Project Overview

Steps to get project running:

1. Install the latest version of Python using [Homebrew](https://brew.sh/):
   `brew install python`
2. Clone/Download this project to your machine
3. Open terminal, and run:
    `python3 /path/to/start.py`

### Features

- Player movement
    - Move using WASD
    - Move using arrow keys
- Attack enemies
- Pickup items
- Open doors with keys
- Gain xp and level up
- Enemy respawning

### start.py

start.py contains an infinite while loop that calls a getch method to constantly get letter input from the terminal. start.py also contains the logic to show the start menu and an instance of the game object.

### game.py

game.py holds the logic of updating and controlling the gameboard. It has a 2d list that holds characters for each position on the map. It also contains a player object and an array of enemies and items. Each time the player moves or interacts with the map, the gameboard will update.

### entity.py

entity.py holds the player and enemy classes, both subclassing an entity class. These two classes contain the logic to make the entity move, drop an item on death, etc.

### item.py

item.py contains the weapon, and potion classes, both subclassing from an item class. These two classes define the logic of the item (whether it deals damage or gives health)

### location.py

location.py is the boring one. It is the implementation of the location, direction, and termcolor classes. These classes are used to save the location of the entity/item, display player direction and show different colors in the terminal.

## Requirements

-   Python 3.0+
-   Possibly need a Mac (Haven't tested it on windows)

## Contributing

Feel free to create some pull requests and contribute to this project.

[python-image]: https://img.shields.io/badge/python-v3.7-blue
[python-url]: https://www.python.org/
[license-image]: https://img.shields.io/badge/License-MIT-blue.svg
[license-url]: LICENSE
[travis-image]: https://img.shields.io/travis/dbader/node-datadog-metrics/master.svg?style=flat-square
[travis-url]: https://travis-ci.org/dbader/node-datadog-metrics
[codebeat-image]: https://codebeat.co/badges/c19b47ea-2f9d-45df-8458-b2d952fe9dad
[codebeat-url]: https://codebeat.co/projects/github-com-vsouza-awesomeios-com
