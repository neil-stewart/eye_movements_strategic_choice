# Data for Stewart, Gächter, Noguchi, and  Mullett (2016)

Stewart, N., Gächter, S., Noguchi, T., & Mullett, T. L. (2016). Eye movements in strategic choice. Journal of Behavioral Decision Making, 29, 137-156. [doi: 10.1002/bdm.1901](http://dx.doi.org/10.1002/bdm.1901)

# conditions.csv

This file describes how stimuli were displayed in different conditions


* id: identifier for condition

* side: row or column player

* left_colour: colour of left payoff in cell

* right_colour: colour of right payoff in cell

* own_payoff: location in cell of own payoff

* other_payoff: location in cell of other player's payoff



# fixations.csv

This file contains one row per fixation.


* expt: always "expt 1", the only experiment

* sub: subject id

* trial.no: trial number, from zero

* fix.no: fixation number, numbered from one, the fixation in which the stimulus appeared

* fix.duration: duration in ms

* fix.x: x location in pixels

* fix.y: y location in pixels

* fix.start: time of the start of the fixation from stimulus onset in ms

* fix.end: time of the end of the fixation in ms



# games.csv

This file contains one row for each of the 64 games. See Table 2.


* id: game id

* game_set: corresponds to Type in Table 2.

* game: numbers the 16 games in each type.

* game_class: based upon (x1-x5 , x3-x7), see section Games on p. 142

* a1,a2,a11,a12,a21,a22: see section Games on p. 142

* x1,x2,x3,x4,x5,x6,x7,x8: see section Games on p. 142

* y1,y2,y3,y4,y5,y6,y7,y8: £ amounts of the actual payoffs.

* cell0,cell1,cell2,cell3: The two payoffs as they appear in each of the four cells of the game




# RTs.csv

The file contains one row per trial


* expt: as above

* sub: as above

* trial.no: as above

* rt: reaction time in ms

* 



# subs.csv

The file contains one row per subject with some demographics.


* time: Time in microseconds since the big bang, or something

* date: Human readable time the experiment started

* subj: as above

* paired: the subject whom this subject was paired with

* condition: id for this subject's condition

* gender: gender

* age: age

* payment: NULL

* completed: did the subject finish

* included: NULL




# trials.csv

One row per trial.


* time: Time of the particular trial...

* date: ...in human-readable format

* subj: as above

* trial: as above

* game_id: as above

* cellorder: The ordering of the cells...

* upper_left,upper_right,lower_left,lower_right: ...with the actual text in each cell in these fields

* pressedkey: the actual key pressed on the keyboard...

* chosen_cells: and the cells they correspond to in the game

* play: NULL

