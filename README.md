# Objective
Use the technique known as transfer learning to develop a model that can accurately predict the diagnosis of patients (Pneumonia/Normal) 
using Keras, and then demonstrate that using BigDL, one can scale this approach and be able to fit any model like this on a much more powerful cluster.

We decided to use the EfficientNet model because it's very efficient, optimized for image classification, and very suited for transfer learning.
(https://keras.io/examples/vision/image_classification_efficientnet_fine_tuning/)

# Presentation of results
In our main notebook, we illustrate how an approach like this can work using the biggest version of EfficientNet. 
And on the secondary notebooks, one can review the results for smaller versions, just for comparison sake.

# Limitations
We use Google Colab to fit a keras pretrained model to our data and finally make good predictions.

We would also like to demonstrate how easily we could scale the training of this model to a cluster using spark. 
But sadly, we haven't been able to do this. Instead, we will explain, alongside our demonstration, how one could do this according to the available documentation.

# Conclusions
EfficientNet seems to work very well with transfer learning. 

As expected, its bigger version (B7), which is able to process images up to 600px x 600px, achieves the highest accuracy of them all. 
But at the cost of severely increasing training time just to improve on a couple percentage points of accuracy.

Finally, scaling any tensorflow, keras, or pythorch model with BigDL seems very straight forward and should help tremendously to train 
this type of models on computer clusters.

# Authors
- Juan Martín Menor de Gaspar
- Álvaro Mellado Ibáñez
