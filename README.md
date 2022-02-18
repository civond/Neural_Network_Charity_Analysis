<h2>Neural Network Charity Analysis</h2>

<h3>Overview</h3>
The purpose of this activity was to use a neural network to predict whether a given charity campaign was successful based off of the dataset provided.

<h3>Results</h3>
<i>Data Preprocessesing</i>
<ul>
  <li>The target of our model is whether the charity campaign is successful. </li>
  <li>The features for our model are items such as use case (for funding), affiliation of campaign, presence of special   considerations, asking amount, etc.</li>
    <li>The features we removed during data pre-processesing were EIN and NAME, which has no affect on the success of the campaign.</li>
</ul><br/>

<i>Compiling, Training, and Evaluating the Model</i>
<ul>
  <li>I slightly increased the number of hidden neurons from 36 to 45, and used the same number of layers (I found that increasing the number of layers didn't help much when trying to optimize the model). I used the ReLU activation sequence for all layers, sigmoid, tanh, and others all yielded worse results. </li>
  <li>Unfortunately, I was unable to reach the target model performance.</li>
    <li>Aside from trying various activation sequences, different numbers of neurons and layers, I also tried filtering the dataset more. However, I found that removing any of the columns resulted in worse model performance. </li>
</ul>

<h3>Summary</h3>
Overall, I was able to achieve a prediction accuracy of ~72.5% for the success of charity campaigns within the dataset. I recommend trying a binary classification model for the future. My reasoning for this is that I believe that a neural network for a dataset this simple is unnecessary. Its runtime is much longer than that of a binary classification model, and the goal is to predict the outcome of a binary variable (ie: a 1 or 0). I would recommend a neural network for a more complex dataset.
