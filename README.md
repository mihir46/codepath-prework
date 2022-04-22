# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: **Mihir Tyagi**

Time spent: **5** hours spent in total

Link to project: (https://glitch.com/~heartbreaking-ancient-hub)

## Required Functionality

The following **required** functionality is complete:

* [x] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [x] "Start" button toggles between "Start" and "Stop" when clicked. 
* [x] Game buttons each light up and play a sound when clicked. 
* [x] Computer plays back sequence of clues including sound and visual cue for each button
* [x] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [x] User wins the game after guessing a complete pattern
* [x] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [ ] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [ ] Buttons use a pitch (frequency) other than the ones in the tutorial
* [ ] More than 4 functional game buttons
* [ ] Playback speeds up on each turn
* [x] Computer picks a different pattern each time the game is played
* [ ] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [x] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough (GIF)

If you recorded multiple GIFs for all the implemented features, you can add them here:
![](http://g.recordit.co/C5DuSIbJ3S.gif)
![](gif2-link-here)
![](gif3-link-here)
![](gif4-link-here)

## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
https://stackoverflow.com/questions/11075927/how-can-i-use-setinterval-or-settimeout-and-display-the-results-during-the-count
https://developer.mozilla.org/en-US/docs/Web/API/setInterval

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 
I found adding a timer for how long the player could make a guess to be quite a challenge. I started by reading about the setInterval function like the tutorial suggested. First, I tried to call setInterval from playClueSequence, so that the timer would start after the clues played. I stored the intervalID in a global variable so I could clear it later, and had it call loseGame after a delay defined by the global constant, timer. Then, I called clearInterval in the guess function so that the timer would stop once the player made a guess. The problem with this approach became clear when I tried to display the timer to the player. I was unable to find how much time was left before setInterval would call loseGame. My next idea was to start by displaying the timer, and once the timer hit 0, I could call loseGame. I didn't know how to go about that, but after some googling I was able to find an example of someone using setInterval to implement a timer, which I modidfied to make my startTimer function. I used this startTimer function in the same way that I originally used the setInterval function and it wokred this time.

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 
[YOUR ANSWER HERE]

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 
[YOUR ANSWER HERE]



## Interview Recording URL Link

[My 5-minute Interview Recording](https://www.loom.com/share/2b3ca72741fe433aae463b3b92d0c019)


## License

    Copyright Mihir Tyagi

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
