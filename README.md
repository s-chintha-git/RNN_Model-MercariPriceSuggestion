Mercari Price Suggestion Algorithm
----------------

Mercari, Japan’s biggest community-powered shopping app, wants to develop an algorithm to suggest right product prices to sellers.

Approach:
- Data provided consists of 1.5 million products and each product has attributes: Name, category, description etc.
- The biggest challenge with the data was the product name and description are not of a standard format and the seller can write these fields in their own words.
- To use the seller given product name and description for price prediction, these fields are converted into vectors using word2vec model and the sequences are then run through a recurrent neural network.
- The RNN model is then combined with remaining available attributes and newly engineered attributes to develop a deep learning model for accurate price predictions.