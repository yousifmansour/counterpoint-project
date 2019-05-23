# Counterpoint Project

## TL;DR
Trained on JS Bach’s counterpuntal works, an ecoder-decoder LSTM model produces a sequence of notes that sounds nice with a given input sequence.

## What is counterpoint?
Counterpoint in music is the is the relationship between voices that are harmonically interdependent yet independent in rhythm and contour. 
There are a lot of rules that say how correct counterpoint can be contructed, but in many cases, composers and musicians end up just creating free-form counterpoint.

## What is the use of this counterpoint?
When multiple instruments or musical voices play together, the interactions of the voices is very important. All the famous classical musical pieces have apply counterpoint to some degree, and that is part of the reason of why the composers are sometimes said to be "genius".

## What does this project do?
The idea here was to think of the problem of [sequence of musical notes] => [sequence of musical notes] in the same way that translation is thought of [sequence of English words] => [sequence of French words]. There are many interesting approaches on how to tackle this sequence to sequence problem (seq2seq). Here we used the encoder-decoder LSTM model to generate the output sequence from the input sequencec.

## What dataset was used to train for this?
JS Bach was a very smart guy. He had created 2 books containing a collection of 24 musical compositions (in astyle called fugues), so 48 in total. The collections have a fugue for each key and in both major and minor (the books are called The Well Tempered Clavier I and II, which mean that the compositions (when played on the clavier, or keyboard) are not biased towards any musical key or scale). 
Since there are many people that have been recorded playing them, there are MIDI files avalible online that contain all the notes for all the voices for these fugues.
So the data set is generated from them. For more, read the [project report here](https://github.com/yousifmansour/counterpoint-project/blob/master/Project%20Report%20-%20Mirabelle%20Dib%20and%20Yousif%20Mansour.pdf).

## How to work with the files in this repo?
Run the python notebooks and follow each part of the code.

## What libraries are needed for this?
[Keras](https://keras.io/) for the LSTM.

[python-midi](https://github.com/vishnubob/python-midi) for hadling midi files.

### Project Team
Mirabelle Dib (mtd07@mail.aub.edu)

Yousif Mansour (ynm03@mail.aub.edu)