# The Necker Cube Experiment
PsychoPy version of the Necker Cube task as used in Leclercq et al. (preprint : https://osf.io/preprints/psyarxiv/x3fc6). Tested on PsychoPy 2023.2.3

## Context
The Necker Cube (NC) Paradigm is a bistable perception task that can be used to assess perceptual inference processing under conditions of maximized ambiguity. During the task, participants are presented with a 2-dimensional projection of the NC intermittently displayed on the screen. At each trial, participants are asked to report their subjective 3-dimensional interpretation of the cube, either seen from above (SFA) or seen from below (SFB).

Different metrics can be extracted from the participants’ answers to characterize their perceptual behavior. Among those criteria we can cite the relative predominance that can be defined as the probability of experiencing each percept and constitutes a direct reflection of perceptual preferences. Alternately, mean phase duration, mean switch rate and perceptual stability are three metrics that relate to the temporal dynamics of inference processing. Mean phase duration corresponds to the time during which the perception of an interpretation persists before a perceptual switch (i.e., a change in the NC interpretation). The switch rate is a close parameter that can be defined as the mean number of switches experienced during a given period. Finally, perceptual stability, corresponds to the probability that a percept persists from one trial to the next. The interest for this later metric is driven by the idea that according to the Markov model, the current percept (i.e., one of the two cube interpretations, SFA or SFB) depends on the previous percept, but also its updating by sensory observation. This assumes a circularity in information processing, where the percept at time t becomes an a priori information at time t+1. 

![task](https://github.com/RenaudJA/Necker_cube_demo/assets/40823809/87a89055-9a09-4690-ba7c-7fba381be969)

## Procedure
The experimental procedure consists of serial NC presentations. Each trial can be  decomposed into three steps. After a fixation cross of pseudorandomized duration (ISI) (1), the Necker cube is presented (2) until participants report their interpretation of the stimulus: ‘seen from above’ (SFA) or ‘seen from below’ (SFB), using the right or left arrow of their keyboard, respectively (3).

The present code includes :
- a set-up phase to maximize standardization across participants
- a training procedure to ensure participants understood the instructions properly
- a "natural perception" part where participants are simply asked to report their percepts without further instruction
- a "forced perception" part for which participants are instructed to force their perception on one of the two possible configurations of the NC

## Output measures example
As mentionned, several metrics can be extracted from the NC paradigm. Here is an example of plot generated using the present version of the task. This curve computed on the 623 participants of Leclercq et al.'s online study represents perceptual stability as a function of ISI for the "natural perception" part. It replicates in-lab experimental findings of a stabilization phenomenon observed for longer ISI (1).

![plot](https://github.com/RenaudJA/Necker_cube_demo/assets/40823809/d5f646a9-a6ea-470d-aea8-01875e09e3d6)

1. Leopold, D. A., Wilke, M., Maier, A. & Logothetis, N. K. Stable perception of visually ambiguous patterns. Nat. Neurosci. 5, 605–609 (2002).

