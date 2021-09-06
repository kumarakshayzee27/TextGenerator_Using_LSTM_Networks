# LSTM Text Generation

This project allows you to train a Long Short-Term Memory neural network to generate text using any TXT file that contains more than 100 characters

## Long-Short Term Memory Network Model
![pr1](https://user-images.githubusercontent.com/89760677/132241027-1c2168d5-7214-494e-9001-0a9f44c410b7.PNG)

## Training

To train the network you run **lstm.py**.

E.g.

```
python lstm.py name-of-file
```

Where:

* **name-of-file** is the name of the file you want to train on

The network will train for 200 epochs. 

**NOTE**: You can stop the process at any point in time and the weights from the latest completed epoch will be available for text generation purposes.

## Generating text

Once you have trained the network you can generate text using **predict.py**

E.g.

```
python predict.py name-of-file length-of-text weights-file
```

Where:

* **name-of-file** is the same file you trained the network with
* **length-of-text** is the length of the text you want to generate (min: 100)
* **weights-file** is the name of the file containing the weights you want to load into the network
