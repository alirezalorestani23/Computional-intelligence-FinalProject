# Computional-intelligence-FinalProject


Introduction of ensemble learning by using LFW data set.
# Project Goal
The program will receive two pictures from people's face and should be able to determine if they belong to one person or not. 

# Dataset

- Intoduction: a database of face photographs designed for studying the problem of unconstrained face recognition. The data set contains more than 13,000 images of faces collected from the web. Each face has been labeled with the name of the person pictured. 1680 of the people pictured have two or more distinct photos in the data set.

- Limitations:
  - Face verification and other forms of face recognition are very different problems. For example, it is very difficult to extrapolate from performance on verification to performance on 1:N recognition.
  - Many groups are not well represented in LFW. For example, there are very few children, no babies, very few people over the age of 80, and a relatively small proportion of women. In addition, many ethnicities have very minor representation or none at all.
  - While theoretically LFW could be used to assess performance for certain subgroups, the database was not designed to have enough data for strong statistical conclusions about subgroups. Simply put, LFW is not large enough to provide evidence that a particular piece of software has been thoroughly tested.
  - Additional conditions, such as poor lighting, extreme pose, strong occlusions, low resolution, and other important factors do not constitute a major part of LFW. These are important areas of evaluation, especially for algorithms designed to recognize images “in the wild”.

# Ensemble Learning

- In statistics and machine learning, **ensemble methods** use multiple learning algorithms to obtain better predictive performance than could be obtained from any of the constituent learning algorithms alone. Unlike a statistical ensemble in statistical mechanics, which is usually infinite, a machine learning ensemble consists of only a concrete finite set of alternative models, but typically allows for much more flexible structure to exist among those 
- **Algorithms:**
    - Random Forest
    - Bagging
    - Voting
    - Boosting: Ada boost

# Main steps

1. Preparing data for training section: I use prepare_dataset() and prepare_dataset_subtract() functions in order to transform images into vectors. Then I make a relation between pair of pictures by:
	1. subtracting their vectors.
	2. concatenation of their vectors.
2. Then I train different models with different parameters to reach the highest accuracy.
3. Finally, I evaluate different models accuracy.

# Conclusion

- Making relation bu subtracting vectors leads to better performance.
- Generally, Random Forest Classifier performance was higher than other models.

