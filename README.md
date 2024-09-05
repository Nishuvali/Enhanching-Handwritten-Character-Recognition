# Enhancing Handwritten Character Recognition: A Comparative Study of Normalization and Pooling Techniques
<h1>Handwritten Character Recognition</h1>

<p>
  This project compares <strong>Global Max Pooling</strong>, <strong>Batch Normalization</strong>, and <strong>Layer Normalization</strong> techniques for <i>Handwritten Character Recognition (HCR)</i>. The dataset used is the <strong>A_Z Handwritten Data.csv</strong>, which includes 26 folders (A-Z) with handwritten images of letters.
</p>

<h2>Abstract</h2>
<p>
  Handwritten character recognition faces various challenges due to different handwriting styles. Traditional methods struggle with accurately interpreting handwritten characters. This research compares <b>Global Max Pooling</b>, <b>Batch Normalization</b>, and <b>Layer Normalization</b>. By using the <i>A_Z Handwritten Data.csv</i> dataset, the model focuses on recognizing the heterogeneous writing styles of letters A-Z. The results demonstrate that <b>Layer Normalization</b> is the most effective, achieving <strong>99.98% accuracy</strong>. This study highlights the importance of selecting the right normalization technique to improve prediction accuracy and build effective character recognition systems. 
</p>

<h2>Keywords</h2>
<ul>
  <li>Handwritten Character Recognition</li>
  <li>Normalization</li>
  <li>Neural Networks</li>
  <li>Pooling Techniques</li>
  <li>Feature Extraction</li>
</ul>

<h2>Introduction</h2>
<p>
  <strong>Handwritten Character Recognition (HCR)</strong> is a key field intersecting <i>Artificial Intelligence</i>, <i>Computer Vision</i>, and <i>Pattern Recognition</i>. It involves converting handwritten input into digital data. This technology plays a critical role in fields such as postal services, digital libraries, and healthcare, automating tasks such as sorting mail, digitizing historical documents, and processing medical forms.
</p>

<h2>Dataset</h2>
<p>
  The dataset, <i>A_Z Handwritten Data.csv</i>, contains grayscale images of letters (A-Z). Each image is centered within a 28x28 pixel box. During preprocessing, the dataset is converted from CSV to PNG format, with each alphabet centered. 
</p>

<h2>Model Architecture</h2>
<h3>1. Convolutional Feature Extraction</h3>
<ul>
  <li><strong>First Two Convolutional Layers:</strong> 32 filters (3x3) with <i>ReLU activation</i> and <strong>Layer Normalization</strong>.</li>
  <li><strong>Max Pooling:</strong> Reduces image size to capture dominant features and avoid overfitting.</li>
  <li><strong>Repeating Blocks:</strong> Two convolution layers with 64 filters each, followed by <i>ReLU</i> and <b>Layer Normalization</b>.</li>
  <li><strong>Final Convolutional Block:</strong> 128 filters, with <i>MaxPooling</i>.</li>
</ul>

<h3>2. Classification with Dense Layers</h3>
<ul>
  <li><strong>Flatten Layer:</strong> Transforms image data into a single dimension.</li>
  <li><strong>Dense Layers with Dropout:</strong> Two dense layers (256 and 128 neurons) with <i>Dropout</i> to prevent overfitting.</li>
  <li><strong>Output Layer:</strong> 26 neurons for letter classification with <b>Softmax activation</b>.</li>
</ul>

<h2>Performance Comparison</h2>
<p>
  Three normalization techniques were compared:
</p>
<ul>
  <li><strong>Global MaxPooling</strong></li>
  <li><strong>Batch Normalization</strong></li>
  <li><strong>Layer Normalization</strong></li>
</ul>
<p>
  After 15 epochs, <strong>Layer Normalization</strong> achieved the highest performance with an accuracy of <strong>99.98%</strong>.
</p>

<h2>Conclusion</h2>
<p>
  In conclusion, <b>Layer Normalization</b> was found to be the most effective normalization technique, achieving a <strong>99.98% prediction accuracy</strong> on the <i>A_Z Handwritten Data.csv</i> dataset. This research underscores the importance of selecting the right normalization technique for <i>Handwritten Character Recognition</i>. Future research could explore methods like <b>RNNs</b> or <b>transformer-based architectures</b> for recognizing entire sentences.
</p>

<h2>Future Enhancements</h2>
<ul>
  <li>Extend from single-character recognition to entire sentences.</li>
  <li>Explore <i>RNN</i> or <i>Transformer-based architectures</i> for holistic text recognition.</li>
  <li>Incorporate <b>sequence-to-sequence learning</b> or <b>attention mechanisms</b> for better contextual understanding.</li>
</ul>

