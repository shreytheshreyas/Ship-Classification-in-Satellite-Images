[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/JasonManesis/Ship-Classification-in-Satellite-Images/blob/main/Ship_Classification_in_Satellite_Images_Keras.ipynb#scrollTo=SwLXYFgmBUWD)
# Ship Classification in Satellite Images
In this project a convolutional neural network model was created for ship classification in satellite images. 
For this project "Ships in Satellite Imagery" dataset was used.

## Dataset Properties

 * The specific Dataset includes 4000 images labeled with either a "ship" or "no-ship" classification.
 * These 4000 images are in .png format and have dimensions of 80 × 80 pixels. 
 * The colour depth of the above 4000 images is 24 bit (8 bits per channel).
 * Image chips were derived from PlanetScope full-frame visual scene products, which are orthorectified to a 3 meter pixel size.
 * The "ship" class includes 1000 images. Images in this class are near-centered on the body of a single ship. Ships of different sizes, orientations, and atmospheric collection conditions are included.
 * Each individual image filename follows a specific format: {label} __ {scene id} __ {longitude} _ {latitude}.png
   * label: Valued 1 or 0, representing the "ship" class and "no-ship" class, respectively.
   * scene id: The unique identifier of the PlanetScope visual scene the image chip was extracted from. 
   * longitude_latitude: The longitude and latitude coordinates of the image center point, with values separated by a single underscore.
* Dataset Link : https://www.kaggle.com/rhammell/ships-in-satellite-imagery 

## Model Architecture
![](/model_architecture.png)

## Model Performance
 
 Performance Metrics:
 
| Class        | Precision | Recall | F1-Score  | Number of Images|
|:------------:|:---------:|:------:|:---------:|:---------------:|
| 0            |0.96       | 0.90   |0.93       |   970           |
| 1            | 0.77      | 0.91   |0.84       |   350           |
|              |           |        |           |                 |
| Accuracy     |           |        |0.91       |   1320          |
| Macro Avg.   | 0.87      |0.91    |0.88       |   1320          |
| Weighted Avg.| 0.91      |0.91    |0.91       |   1320          | 
 
Some random correct classified ships are shown below:

![](/Project_Image.png)

## Requirements

<pre>
 Pandas                                    Seaborn                              Keras                      
 TensorFlow                                Matplotlib                           scikit-learn        
 OpenCV                                    NumPy                                
</pre> 
