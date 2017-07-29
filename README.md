# Music Generator Demo

## Overview
Use TensorFlow to generate short sequences of music with a [Restricted Boltzmann Machine](http://deeplearning4j.org/restrictedboltzmannmachine.html). 
This is the code for [Generate Music in TensorFlow](https://youtu.be/ZE7qWXX05T0) on YouTube. 

## Dependencies

  * [Tensorflow](https://www.tensorflow.org/versions/r0.10/get_started/os_setup.html)
  * pandas
  * numpy
  * msgpack-python
  * glob2
  * tqdm 
  * python-midi
  
Use [pip](https://pypi.python.org/pypi/pip) to install any missing dependencies (i.e pip install --upgrade msgpack) 

### Dependencies on Win with python3
```
    pip3 install pandas
    pip3 install msgpack-python
    pip3 install numpy
    pip3 install glob2
    pip3 install tqdm
    pip3 install git+https://github.com/vishnubob/python-midi@feature/python3
```

## Basic Usage
To train the model and create music, simply clone this directory and run
```
python rbm_chords.py
```
[Restricted Boltzmann Machine]_chords.py

The training data goes in the pop_music_midi folder. You have to use MIDI files. You can find some [here](http://www.midiworld.com/files/). Training will take 5-10 minutes on a modern laptop. The output will be a collection of midi files. You can combine them together with a script if you'd like. 

## Challenge

The challenge for this video is to create a happy/upbeat MIDI file using this script. You could play with the hyperparameters if you'd like to see what works, choose a happy/upbeat MIDI dataset, or do both. When you're done, upload your clone of this repository whether or not the code is modified with your generated MIDI files included in the repo. Post a link to your code in the comments of the video. I'll mention the winner (the most upbeat sounding MIDI, any of the snippets is fine or if you want you can combine them) in my next video. Good luck!!

## Credits

The credit for this code goes to [dshieble](https://github.com/dshieble) i've merely created a wrapper around his code to make it easier to get started. 
