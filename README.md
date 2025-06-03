<h1>Pneumonia Detection</h1>

<h2>About the Dataset</h2>

<p>
  The dataset is acquired from 
  <a href="https://www.kaggle.com/datasets/vinadsa/chest-x-ray-for-pneumonia-dataset" target="_blank">
    Kaggle: Pulmonary Chest X-ray Abnormalities
  </a>, which contains:
</p>

<ul>
  <li><strong>16,000 images</strong> for training</li>
  <li><strong>2,000 images</strong> for testing and validation</li>
</ul>

<p>You can download the dataset using the code snippet below:</p>

<pre>
<code>
import kagglehub

# Download latest version
path = kagglehub.dataset_download("vinadsa/chest-x-ray-for-pneumonia-dataset")
print("Path to dataset files:", path)
</code>
</pre>

<h2>Project Overview</h2>

<p>
  In this project, we differentiate chest scan images between <strong>Normal</strong> and <strong>Pneumonia</strong> patients. 
  This classification is performed using a <strong>Convolutional Neural Network (CNN)</strong>.
</p>

<ul>
  <li>Images are resized to <strong>32x32</strong> pixels for uniform processing.</li>
  <li>The CNN architecture includes <strong>2 convolutional layers</strong> with a kernel size of <strong>5x5</strong>.</li>
  <li>Max pooling is applied using a <strong>2x2 kernel</strong>.</li>
  <li>The loss function used is <strong>CrossEntropyLoss</strong>.</li>
  <li>The optimizer is <strong>Stochastic Gradient Descent (SGD)</strong> with a learning rate of <code>0.001</code> and momentum of <code>0.9</code>.</li>
</ul>

<p>
  You can experiment by changing the optimizer and learning parameters to test their impact on classification accuracy.
</p>

<h2>Final Conclusion</h2>

<ul>
  <li><strong>Testing Accuracy:</strong> 78.91%</li>
  <li><strong>Validation Accuracy:</strong> 78.36%</li>
</ul>
