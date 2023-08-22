# Pop-it iOS App

## About
This project is one of the assessments from the 42889 41889 Application Development in the iOS Environment iOS Application Development.

## Objectives
1. The purpose of this project is to demonstrate competence in the following skills:
2. The full software development cycle
3. iOS App UI and program design
4. iOS UI programming
5. Effective use of platform APIs
6. Program testing

## Functionality Specification
The game is called BubblePop (you can call your app a different name if you wish to). In this
game, a number of bubbles are randomly displayed on an iOS device screen. A player pops a
bubble by touching the bubble, and every time they pop a bubble they earn a certain number of
points. Bubbles come in five colours: red, pink, green, blue and black. Each colour corresponds
to a specific number of points and has a specific probability of appearance (see table 1). All
bubbles appear on the screen briefly (see core functionality 9). A player needs to pop as many
bubbles as possible within a certain timeframe (default to 60 seconds) to get high scores. Note
that, if a player pops two or more bubbles of the same colour consecutively, they earn 1.5 times
the points for the additional bubbles they pop. Finally, game scores are saved and a high score
board is displayed after a game run is finished. Figure 1 provides a rough mock up of what the
main interface may look like. NOTE: Figure 1 gives you a guide for your GUI, you may design a
Colour Game Points Probability of Appearance more sophisticated and more polished GUI for your own work. You will get 1 functionality mark
for each functionality item specified below
Red      1   40%
Pink     2   30%
Green    5   15%
Blue     8   10%
Black   10    5%
 
## Core Functionalities
1. A player must be able to enter their name before the start of a game run. (You may load
the player's name from the GameKit API if you wish. This extra work is not required.)
2. A game timer shall be displayed and it must count down continuously in one-second
intervals. When the timer reaches zero, the game stops.
3. A score shall be displayed. It shall be zero initially and shall be updated every time the
player successfully “pops” a bubble.
4. The default timeframe for a game is 60 seconds, i.e. the game timer starts from 60
seconds and counts down to 0. This number shall be adjustable in the app settings.
5. The maximum number of bubbles displayed on the screen is defaulted to 15, i.e. there
shall be between 0 and 15 bubbles shown on the screen at the same time. This number
shall be adjustable in the app settings.
6. The app randomly decides how many bubbles (up to the maximum allowed bubble
number) shall be displayed on the screen at a time. The bubble colour is decided according
to the Probability of Appearance in Table 1.
7. Bubbles shall be displayed at random positions on the screen with the following
restrictions:
1. The entire bubble shall be displayed within the screen. There shall not be any bubble
with some parts off the screen once it has fully appeared.
2. No two (or more) bubbles shall overlap each other.
8. When a player touches a bubble, the bubble shall be removed from the screen and the
corresponding game points shall be added to the overall score. For example, if the green
bubble in Figure 1 was touched, it shall disappear and the score shall increase by 5 game
points. If two or more bubbles of the same colour are popped in a consecutive sequence,
the bubbles after the first one will get 1.5 times their original game points. For example, if
two black bubbles were popped one after the other, 25 (10 + 1.5 * 10) shall be added to
the total score. Round to the nearest integer if necessary.
9. The app shall refresh bubbles displayed every game second. That is, after every game
second, the app shall randomly remove a number of bubbles (do not include the bubbles
that have been popped by the player) and replace them with another set of randomly
positioned bubbles. There may be more or less bubbles on the screen compared with the
previous game second subjected to the restrictions in 5 and 6. In this case, "random"
means chosen by the program, not the user. So you have a lot of discretion in
placement of new bubbles and selection of old bubbles.
10. When the game stops, the player’s score shall be saved in a persistent file (or database)
that contains all players’ names and their highest scores.
11. At the end of the game, a high score board shall be displayed with the names and scores
of the highest ranking players. (See Figure 2)
