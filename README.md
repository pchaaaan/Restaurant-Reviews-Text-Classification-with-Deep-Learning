<h1>Sentiment Analysis on Arizona Restaurant Reviews Using Deep Learning</h1>

<p>This repository contains a deep learning-based approach to perform sentiment analysis on a dataset of restaurant reviews from Arizona. The project employs various deep learning models, including GRU and LSTM networks, leveraging pre-trained GloVe embeddings to enhance the feature representation.</p>

<h2>Getting Started</h2>

<h3>Prerequisites</h3>
<ul>
  <li>Python</li>
  <li>TensorFlow</li>
  <li>Keras</li>
  <li>Pandas</li>
  <li>NumPy</li>
  <li>scikit-learn</li>
</ul>

<h3>Dataset</h3>
<p>The dataset includes restaurant reviews with a 'text' column for the review content and a 'stars' column indicating the review rating. Reviews are labeled as positive (above 3 stars) or negative (below 3 stars), with 3-star reviews excluded to focus on clear sentiment distinctions.</p>

<h2>Implementation Details</h2>

<h3>Data Processing</h3>
<ul>
  <li>Reviews are labeled based on their star ratings: 1 for negative and 0 for positive sentiments.</li>
  <li>The dataset is split into training and testing sets to evaluate the model's performance.</li>
</ul>

<h3>Model Building</h3>
<ul>
  <li><strong>GRU with GloVe</strong>: A model utilizing a Gated Recurrent Unit (GRU) architecture with pre-trained GloVe embeddings set as non-trainable.</li>
  <li><strong>LSTM with GloVe</strong>: A model applying a Long Short-Term Memory (LSTM) layer, also leveraging GloVe embeddings in a similar fashion.</li>
  <li><strong>GRU with Trainable Embeddings</strong>: A GRU-based model with embeddings learned during the training process.</li>
</ul>

<p>Each model architecture involves embedding layers followed by either GRU or LSTM layers, and dense layers for classification.</p>

<h3>Training and Evaluation</h3>
<ul>
  <li>The models are trained on the preprocessed review texts and evaluated using accuracy and loss metrics.</li>
  <li>Performance is assessed on a held-out test set to ensure generalization.</li>
</ul>

<h2>Results</h2>
<p>The trained models aim to accurately classify reviews into positive or negative sentiments, offering insights into customer perceptions of various restaurants. The use of pre-trained embeddings like GloVe helps in capturing semantic relationships in the text data, potentially improving model performance.</p>
