# 259-Final-Project-TBasil

Final project designed to establish standards for setting aside participants who did not pay adequate attention to survey answers. 

In this data set, 15 attention checks were included in the survey which consisted of pairs of a low valenced questions from established measures and a mirror question worded in the oposite direction. These mirrors were used to establish two measures of attention. First, simple percent of maximum possible differences were  calculated by taking the absolute value of the pair difference and dividing by the maximum possible difference on the scale. These 15 difference scores were then summed and z scored. Second, a flagging system was established. In this case, if both resposes on the mirrored items were above or below the middle response, a 1 was given to the score identifying poor attention to responding. If the responses were at or on the opposite side of the middle score, a 0 was given which suggested the participant had been paying attention to their resonding. This series of flags was also summed and scaled. The intention was to establish a more rigorous and a less rigorous system of identifying poor attention by partcipants.

Additionally, data were evaluated for longstringing which is an index of a partcipant giving the same response consecutively over a long stretch of items which is an indication of careless responding. Longstring values were then z scored and added to the attention sums detailed above.

With these two new variables, attention difference plus longstring and attention flags plus longstring, it was theorized that alpha values for data collected on the BFI-2 traits should increase as the most egregious attention voilaters were systematically set aside from the data set. Iterative code was written to remove the single highest attention check score (the individual who made the highest number of attention check violations) and re-calculate alpha values repeatedly until fewer than 50 participants remained in the data set. 

This code loads a data set, iterates alpha values for each of the 5 traits in the BFI-2 after sequentially removing the participant identified as having the worst attention and produces graphs of the alpha values for the traits as each participant is removed. 

Unfortunately, this approach fails to establish a clear guidline that can be universally applied to additional data sets as there is no clear plateau of alpha values after the participants who paid the least attention are removed. 
