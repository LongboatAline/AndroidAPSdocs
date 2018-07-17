# Prediction lines
## Understanding the prediction lines

Without a popup showing details, things will get a lot easier to understand once the lines are coloured. 
(I definitely like that “rainbow” :) since the colours are used consitently throughout the AAPS interface. 
I’ll try to give a simplified summary based on what’s most interesting when you start observing these lines 
(Based on my limited understanding. Also I won’t differentiate COB/aCOB/UAM or go into their details):
* Orange is used for carbs. So the orange coloured prediction line matches what the loop thinks would 
  develop based on the known amount of Carbs on Board, assuming that the loop doesn’t adapt the current dosing. 
  When all the lines are purple, as in Version 1.xx or in the Nightscout web interface, that one’s usually 
  the one pointing skywards ;) (or, as time proceeds, the one furthest up)
* The blue-ish ones then are referring to the IOB-based predictions: a lighter blue for what the loop thinks 
  would happen if the COB information is plain wrong, and the current IOB (known pretty well) were to run 
  its course with no further carbs in the system to counter its effects. 
  Kind of a “worst case” scenario, and in the monochrome setting, that line would be the one pointing down soonest. 
  This line also gives an indication how much of a grace time there would be before running low,
  assuming there’s a worst case where 
    1. a bolus was given, 
    1. no carbs were consumed to match it, 
    1. and there were no way for the loop to cut off basal insulin
    
 * The darker blue line would be the `ZT` (Zero-temp) line, it indicates how much of a saving effect an 
   immediate Zero-Temp would have on that worst-case scenario (leaving the first two conditions, but remedying the third). 
   So that gives an indication of how much saving power a zero temp would have, 
   and how much time it’d buy you to eat your weight worth in glucose should you 
   realize that you had bolused without eating …)
   
Please note that those lines are not a prediction how your BG is supposed to run, 
they're more of an insight into the reasoning of the loop, and on what possible 
outcome the loop is basing its actions. 

## The prediction lines in action
When you start a bolus and make a carb announcement, 
upon the next run of the loop those lines should include the possible effects 
of those announcements in a brightly coloured rainbow of widely disparaging lines. 
As more and more time passes, and the bolus/carb are hopefully balancing each 
other out, those lines will start to converge as well, getting closer and closer 
to what can really be considered a possible outcome. In the meantime the loop 
will if necessary (as justified/indicated by those predictions) 
make adaptions to improve your chances of having the resulting outcome 
somewhere within your desired target range. 

## Using the prediction lines
From observing these lines (and even more from reading the output 
from the loop as available in the tab according to the algorithm used) 
you can learn what the loop is considering, and how you might need to 
adapt your parameters. 
