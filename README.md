# Motor-Imagery-Analysis-LSTM-CNN:
Here is a code to analyse eeg signals of right/left hand MI tasks using LSTM and 1D CNN. 

## MI task:
MI task is an experiment where a subject is asked to imagine doing something in its head and in this case, the subject is imagining moving right or left hand.

## Dataset used:
[An online dataset](http://gigadb.org/dataset/100295) containing 52 subjects' eeg signals while they are perfoming MI tasks is used in this project. In this dataset, each subject has around 200 right and 200 left trails of eeg recording. A more detailed discussion of its experiment can be found [here](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5493744/#bib17) 

## LSTM and 1D CNN:
In this code, performance of LSTM and 1D CNN on analysis of MI tasks is studied. From our observation, 1D CNN works better on this specifc task, which surprieses us because LSTM normally gives our the best results on time-series analysis. A more detailed discussion of 1D CNN's performance can be found on the project report.

## Results:
The average accuracy over all valid subjects is 66.25% (+/- 17.87%). And we have achieved high accuracy (above 80%) on eight subjects with the highest being 87.5%.
