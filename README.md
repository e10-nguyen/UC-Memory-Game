# Pre-work - *Memory Game*

**University of California Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: **Ethan Nguyen**

Time spent: **6** hours spent in total

Link to project: (https://glitch.com/edit/#!/puzzled-luck-hallway)

## Required Functionality

The following **required** functionality is complete:

* [X] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [X] "Start" button toggles between "Start" and "Stop" when clicked. 
* [X] Game buttons each light up and play a sound when clicked. 
* [X] Computer plays back sequence of clues including sound and visual cue for each button
* [X] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [X] User wins the game after guessing a complete pattern
* [X] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [X] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [X] Buttons use a pitch (frequency) other than the ones in the tutorial
* [X] More than 4 functional game buttons
* [X] Playback speeds up on each turn
* [X] Computer picks a different pattern each time the game is played
* [X] Player only loses after 3 mistakes (instead of on the first mistake)
* [X] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [X] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [X] Random Patterns every iteration of the game

## Video Walkthrough (GIF)

If you recorded multiple GIFs for all the implemented features, you can add them here:
![](https://im4.ezgif.com/tmp/ezgif-4-5a289c148a.gif) Loses the Game
![](https://im4.ezgif.com/tmp/ezgif-4-d96f87f365.gif) Random Patterns
![](https://im4.ezgif.com/tmp/ezgif-4-998abd66ca.gif) Wins the Game

## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
Lots of time spent on stackoverflow and w3schools learning the syntax of many commands. Looked up youtube videos on the best way to adjust image size within the buttons. Also used piano key frequencies from music book. At least an hour was spent reading different discussion threads on how to best implement sounds and buttons together in one object, and to get the exact functionality I wanted I also asked some of my peers from my CS class.

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 
A huge challenge for me was getting the pictures to adjust to the button size. At first I simply inserted the images into the page, but realized that on different devices that the screen would be a different size, so while the buttons would adjust, the size of the pictures was set. Due to my own lack of knowledge of HTML syntax, most of the code that I wrote would not work. One variation I tried involved turning the images themselves into buttons, but found that was far more complicated that the solution already provided with the button objects, and would cause me to deviate very far from the pre-work example provided. I ended up finding out through a StackOverflow thread that one can add the image through a url using <img> in the button object itself. This way the button and the image would have the same parameters concerning width and height. This still required some debugging however, as I wanted this game to be able to work on different sized webpages, from a desktop computer to a smartphone. Another difficulty I encountered similar to this was how to make decreasing intervals for each clue. At first I believed that by using setInterval() I could just simply call it every time the next clue was given. For what I figured out to be a global/local function issue with classes, the setInterval() function would be called along with the countDown() function, which reset the counter at every turn of guessing. This logic bug had me stuck for a while, so I eventually went back to drawing out the function on paper to figure out why there was no change in the interval of 1000ms. Later on, I used terminal and set up breakpoints using console.log() to find that my functions clearInterval() and stopGame() were working correctly, and made new global variables so that the countdown clock worked correctly. This debugging session was a refresher for me as I have not used any web development languages in the past few months, and piqued my interest the further I got in the project.

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 
[YOUR ANSWER HERE]

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 
[YOUR ANSWER HERE]



## Interview Recording URL Link

[My 5-minute Interview Recording](your-link-here)


## License

    Copyright Ethan Nguyen

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
