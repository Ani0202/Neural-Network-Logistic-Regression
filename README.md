# Neural-Network-Logistic-Regression
Image recognition algorithm that recognizes cats
Problem Statement: You are given a dataset containing:

- a training set of m_train images labeled as cat (y=1) or non-cat (y=0)
- a test set of m_test images labeled as cat or non-cat
- each image is of shape (num_px, num_px, 3) where 3 is for the 3 channels (RGB). Thus, each image is square (height = num_px) and (width = num_px).
You will build a simple image-recognition algorithm that can correctly classify pictures as cat or non-cat.

## - General Architecture of the learning algorithm ##

It's time to design a simple algorithm to distinguish cat images from non-cat images.

You will build a Logistic Regression, using a Neural Network mindset. The following Figure explains why **Logistic Regression is actually a very simple Neural Network!**

<img src="https://i1.wp.com/www.maolintu.com/wp-content/uploads/2018/02/LogReg_kiank.png?fit=1036%2C804&ssl=1" style="width:650px;height:400px;">

**Mathematical expression of the algorithm**:
For one example  𝑥(𝑖) :
𝑧(𝑖)=𝑤𝑇𝑥(𝑖)+𝑏(1)
𝑦̂ (𝑖)=𝑎(𝑖)=𝑠𝑖𝑔𝑚𝑜𝑖𝑑(𝑧(𝑖))(2)
(𝑎(𝑖),𝑦(𝑖))=−𝑦(𝑖)log(𝑎(𝑖))−(1−𝑦(𝑖))log(1−𝑎(𝑖))(3)
The cost is then computed by summing over all training examples:
𝐽=1𝑚∑𝑖=1𝑚(𝑎(𝑖),𝑦(𝑖))(6)

**Key steps**:
In this exercise, you will carry out the following steps: 
    - Initialize the parameters of the model
    - Learn the parameters for the model by minimizing the cost  
    - Use the learned parameters to make predictions (on the test set)
    - Analyse the results and conclude

