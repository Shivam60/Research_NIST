# Convolutional Neural Network Committees For Handwritten Character Classification

```sh
- It is better to explain using **flowchart, or diagram**
```

```sh
- For taking less time, we have to reduce no of epochs(training a single net for the 62 class problem takes almost six hours).
We can't be sure if 5 epochs or 500 is enough for convergence since it will vary from data to data. We can stop training when the error converges or gets lower than a certain threshold. This also goes into the territory of preventing overfitting.
```


```sh
- Averaging individual committee member outputs, instead of optimizing their combinations(which would cost additional valuable training data) ,is best option.
```


```sh
- Deformations are essential to prevent overfitting, and greatly improve generalization.
```


```sh
- Uppercase letters are much easier to classify than lower- case letters—error rates are four times smaller. Shapes of uppercase letters are better defined, and in-class variability due to different writing styles is generally smaller.
```


```sh
- We will face difficulties like : {0,o,O}, {1,l,i,I}, {6,G}, {9,g}
**Solution : We therefore also train various nets on digits, all letters, a merged letter set, and also on lowercase and uppercase letters separately. This drastically decreases the number of confused classes and also makes it possible to compare our results to other published results**
```


```sh
- Another diffculty : We need GPU with very high processing speed, if we want minimum error. Because this will take long time to train on given huge NIST dataset(NIST SD 19 database [12], which contains 482,925 training and 82,587 test characters (i.e. upper- and lower-case letters as well as digits). Applying different and most appropriate algorithm, is second part of our project, but at first, we have to train it. 
```


```sh
- To the best of our knowledge, this research paper results are far better (30-350%) than any already published result. We must get better results than this!
```

