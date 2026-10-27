# Iris Classification: Perceptron vs ANN

Classifies iris flowers into 3 species (setosa, versicolor, virginica) from
4 measurements, and compares a single-neuron Perceptron with a small
Keras neural network.

## Dataset
Iris dataset: 150 samples (50 per class), 4 features (sepal length/width,
petal length/width). 120 samples for training, 30 for testing (stratified).

## Models
| Model | Details |
|---|---|
| Perceptron | scikit-learn, max_iter=1000, linear boundary |
| ANN | Input(4) -> Dense(8, ReLU) -> Dense(3, Softmax), Adam, sparse categorical crossentropy, 100 epochs, batch size 8 |

## Results
| Model | Test accuracy |
|---|---|
| Perceptron | XX |
| ANN | XX |

The test set has only 30 samples, so one sample is about 3.3%.
The difference between the models is small and should be read with care.

## Observations
- Setosa is easy to separate. Versicolor and virginica overlap slightly,
  which is where the Perceptron (a straight-line model) makes more mistakes.
- The ANN can learn a non-linear boundary through its hidden ReLU layer.

## Limitations
Iris is a small, clean dataset. Results do not reflect performance on
harder real-world data.

## Run
Place `iris.csv` next to the notebook and run all cells.
