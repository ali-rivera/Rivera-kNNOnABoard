# kNN on a Board

|              |                                                                                                                                                                   |
|--------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Summary      | This activity allows students to walk through the kNN machine learning algorithm in an easily interpretable, 2-dimentional space. The data represented on the board visualizes whether users made purchases (color) from social media sites and 2 features - age (x axis) and estimated salary (y axis). This data is a randomly selected sample from the [Kaggle dataset "social_network_ads"](https://www.kaggle.com/datasets/riyakapoor/social-network-ads/). Students will idtentify the  "test points" on the graph (in black and labeled A-E) and use the kNN algorithm with multiple k values to classify each of the points and choose the best k value based on their evaluation critera. They use whiteboard markers and rulers to find the nearest neighbors and create boundaries in the space. Finally, they connect their understanding of overfitting/underfitting to their choice of k value.  |
| Topics       | kNN algorithm, machine learning, overfitting/underfitting, hyperparameter tuning  |
| Audience     | Introduction to AI, could be adapted to K-12  |
| Difficulty   | Easy - given students have the assumed prior knowledge described in the Dependencies section. Otherwise, it is recommended that the questions be altered to reach students' level of prior knowledge  |
| Strengths    | This activity is unplugged and gives students an opportunity to gain an understanding of the kNN algorithm in a no-code environment. It also allows students to explore the algorithm in a familar, 2-dimensional space and gain understand that can be applied to higher dimensional spaces. The activity materials are flexible and could be used to teach multiple facets of kNN or other simple algorithms.  |
| Weaknesses   | As described in the dependencies section, this activity requires prior knowledge of some foundational machine learning concepts, as well as prior knowledge/instruction on the kNN algorithm. Creating boundaries lines at this scale requires approximation, so while creating the lines helps students understand the boundaries in space, it is not a perfect representation of how those are made in a ML program. |
| Dependencies | This activity assumes that students have some foundational prior knowledge of the following terms in the context of data science: <br /> &ensp; &ensp; - algorithmic thinking <br /> &ensp; &ensp; - classification models <br /> &ensp; &ensp; - training vs. testing data <br /> &ensp; &ensp; - evaluation criteria <br /> &ensp; &ensp; - overfitting vs. underfitting  <br /> Materials required for this activity are: <br /> &ensp; &ensp; - printed kNN boards (see comments in instructor notes about printing) <br /> &ensp; &ensp; - dry erase markers or some other erasable writing utensil <br /> &ensp; &ensp; - rulers |
| Variants     | This activity could be adapted to teach concepts like: <br /> &ensp; &ensp; - **distance metrics**: have students compare classification outcomes across various distance metrics (Euclidean distance, Manhattan distance, Minkowski Distance, etc) instead of/in addition to k values. <br /> &ensp; &ensp; - **evlauation metrics**: have students create a confusion matrix, calculate accuracy, sensitivity, specificity, etc. for each of their k values. |

## Student Activty

### kNN On a Board

**General Description:** In this activity we will explore the kNN algorithm using a visual representation of purchasing data from [Kaggle](https://www.kaggle.com/datasets/riyakapoor/social-network-ads/). The data contains social network user information including estimated salary and age, and whether the user bought a product. We will use the kNN algorithm to predict if a new user is likely to purchase a product using their salary and age. 

**Why am I doing this?**  kNN is a common algorithm used for classification problems. This lab will allow you to work through the algorithm in the same way that the computer does (just on a smaller scale) and give you a hands-on understanding of how classifications are made in the model. 

**What am I going to do?** Using the kNN board, you will first identify the 5 points in black. Then, you will classify these points as one of two classes: purchased - blue or not purchased - orange. Choose 3 k values (must be greater than 1 and odd), find the k nearest neighboring points using Euclidean distance – a straight line between 2 points and classify the point as purchased or not purchased. Record the classification for each point in a table. Then, compare these results to the actual class (obtained from your instructor) to pick the best k value and answer the questions below. 

**Questions** 

1. Using what you learned in class about kNN, explain in your own words (at a "rubber duck level") how the kNN model works. Be sure to answer the following questions in your explanation: 
<br /> &ensp; &ensp; a. What does k represent? 
<br /> &ensp; &ensp; b. How is a prediction made for a new observation (one not in the training data set)? 
<br /> &ensp; &ensp; c. In this example, is kNN being used for classification or regression? Why? 
<br /> &ensp; &ensp; d. Include references (links are fine) to any additional sources you use - you may find this [IBM article](https://www.ibm.com/topics/knn) helpful.

2. Include the table you recorded your classifications in for all 3 k values you tested for each of the 5 test points. 

3. Recommend a value for k based on your observations. Provide a rationale for why you chose that value. 

4. Using the k value you have chosen, create estimated boundaries areas (like the {ref}`example below <boundarylines-example>`). Include a picture of the board with the drawn boundaries. 

5. Which areas of the graph did kNN do best in? Worst? Why do you think this is? 

6. Overfitting and underfitting are common issues in machine learning. Explain why picking a k value too small overfits your model, and a k value too large underfits your model. 

***Insert border image***

**How will I know I have succeeded?**


| **Specs Category** | **Specs Details** |
|----------------|---------------|
| **Formatting**     | - 2 pages max <br /> - PDF format <br /> - Headings <br /> &emsp; - Lab Name <br /> &emsp; - Your name, course, date <br /> &emsp; -Questions  |
| **Questions**      | - Goal: Explore the kNN algorithm through the guided questions <br /> - Detailed responses to the questions that include examples from your experience where appropriate <br /> - Completed table for your 3 k values <br /> - Image of the graph with your drawn boundary lines <br /> - Format your responses in a numerical list corresponding to the questions list  |

**Acknowledgements:** Special thanks to Jess Taggart from UVA CTE for coaching us. This structure is pulled directly from [Streifer & Palmer (2020)](https://cte.virginia.edu/blog/2020/12/04/alternative-grading-practices-support-both-equity-and-learning). 


## Instructor Notes

### Materials 
This activity is "unplugged" and therefore requires some materials. The {ref}`kNN board <kNN-board>` below can be printed in many different formats, but for sustainability of resources it is recommended that the image be printed as large as 24" x 36" and lamintated. We find using dry erase markers on the laminated surface successful for student engagement and longevity of materials.

***Insert board image*** 

### True Values
We recommend witholding the true values below until students have made a classification for each of their k values. Often this results in a teachable moment where they do not have the true values, and will struggle to determine which k is best with missing information. This productive struggle raises questions and creates a memorable connection to the process for students. 

<br />**Point A:** Purchased (Blue)
<br /> **Point B:** Not Purchased (Orange)
<br /> **Point C:** Not Purchased (Orange)
<br /> **Point D:** Purchased (Blue)
<br /> **Point E:** Purchased (Blue)



## Resources
- [Data from Kaggle](https://www.kaggle.com/datasets/riyakapoor/social-network-ads/)
- [kNN board (.pdf)](https://myuva-my.sharepoint.com/:b:/g/personal/wat6sv_virginia_edu/Ebv9Jy5MH35MlXmgL4gT7NoBCq56Ag-Lu6HHzy5SiR4KtA?e=LIDJn3)


