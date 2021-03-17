# aaai2021-scene-graph-image-retrieval

This repository contains the resources released by [Image-to-Image Retrieval by Learning Similarity between Scene Graphs](https://arxiv.org/abs/2012.14700).

* `compute_human_correlation_v1.ipynb`: A notebook that reads the human experiment data and computes inter-human agreement score.
* `triplets.csv`: The list of image triplets used in human experiments. 
    * `query_id`: Visual genome id of the query image.
    * `target_id1`: Visual genome id of the first target image.
    * `target_id2`: Visual genome id of the second target image.
* `anon_results.csv`: The human experiment data. 
    * `user_id`: anonymized id of human annotators.
    * `answer`
        * 0 (`target_id1` images is more relevant to the query image)
        * 1 (`target_id2` images is more relevant to the query image)
        * 2 (target 1, target 2, and the query are all identical)
        * 3 (neither of the images are relevant to the query image)
    * `triplet_id` : THe id of triplet.


We will upload the prediction results from our models and baselines as well as a code for computing agreement between algorithms and human annotations.
