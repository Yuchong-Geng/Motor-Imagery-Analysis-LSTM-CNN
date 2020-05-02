# Motor-Imagery-Analysis-LSTM-CNN:
Here is a code to analyse eeg signals of right/left hand MI tasks using LSTM and 1D CNN. 

## MI task:
MI task is an experiment where a subject is asked to imagine doing something in its head and in this case, the subject is imagining moving right or left hand.

## Dataset used:
[An online dataset](http://gigadb.org/dataset/100295) containing 52 subjects' eeg signals while they are perfoming MI tasks is used in this project. In this dataset, each subject has around 200 right and 200 left trails of eeg recording. A more detailed discussion of its experiment can be found [here](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5493744/#bib17) 

## LSTM and 1D CNN:
In this code, performance of LSTM and 1D CNN on analysis of MI tasks is studied. From our observation, 1D CNN works better on this specifc task, which surprieses us because LSTM normally gives our the best results on time-series analysis. A more detailed discussion of 1D CNN's performance can be found on the project report.

## Results:
The average accuracy using 1D CNN over all valid subjects is 66.25% (+/- 17.87%). And we have achieved high accuracy (above 80%) on eight subjects with the highest being 87.5%. (This code uses 80/20 split of data for training and testing) 

## A Short Explanation of the Code:
### Preprocessing: 
This code contains a preprocessing section where dataset in .mat format is loaded into the notebook and useful information is extracted from the eeg data object. A detailed documentation of the data structure can be found on the paper mentioned earlier.  
### Smooth filter:
Before feeding the data into the network, you can choose to apply a smooth filter which avererges adjacent data points and thus can help reduce the potential noise from collection. The window or numnber of adjacent points can be any positive integers. (Use of this smooth filter may or may not improve the performance of the nerual network, so please see this as an availble tool that is up to you to decide whether to use it)
### Nerual Network:
As discussed earlier, two types of nerual networks are used in this project. Please feel free to play with them and here is a [documentation](https://keras.io/) for the you.
