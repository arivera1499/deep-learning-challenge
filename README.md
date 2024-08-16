# deep-learning-challenge
# notes. I dont believe that discussed how to download and save .h5 files from google colab and unfortunately could not get it to work on my end before the deadline. Previous lecture material, in-class assignments, and CGPT were used throughout this project for referencing and debugging. 

# purpose 
  - For this assignement we were tasked with using a deep learning model to analyze and predict if an organization funded by the alphabet soup foundation would be successfull and use the funding effectively. This model would then be used on future applicants to decide if they were a good candidate for funding.

# Results 
  - Data Processing

      -The target variable of the model was the "IS_SUCCESSFUL" column and trying to predict wether it was succesfull (1) or unsuccessful (0)
      -The features for the model can be found in the image below.
        ![image](https://github.com/user-attachments/assets/ac32e805-14f0-4784-a807-88b1d5932093)
    
      -The "EIN" and "NAME" column are the variables that should be removed as the do not help in deciding if the organization is successful or not

    
  - Compiling, Training, and Evaluating the Model
      -Two hidden layers were used with the same "relu" activation with the first layer containing 8 neurons and the second containing 5 neurons. These activations, neurons, and layers were used due to the nature of the data         and how similar the project was to the getting_real activity that we did in class. We never really went above 8 neurons during class time as the amount of time taken to render the model would increase as the amount           of neurons and layers increased. Another reason we used "relu" activation was also because of its versatility in deep learning models and its ability to for fast computation and training.
        ![image](https://github.com/user-attachments/assets/0bd3927e-0505-43e9-898e-765d40991c0d)

    -Unfortunately I was unable to reach the target performance with each instance of the model only reaching 73% accuracy. During some of the optimization trials i did notice that at some points some of the epochs were
     able to reach up to 74%.
    -Many steps were taken in order to increase the accuracy of the model such as: adding more hidden layers, adding more neurons per node, and even trying out differe activations such as "tanh".
        ![image](https://github.com/user-attachments/assets/9af86d7c-9871-42d5-9ff0-ddfd18b378b3)

# Summary 
  -Overall I was only able to achieve an accuracy score of 73% when using tf.keras deep learning models. The only other model that i can think of that may produce some luck would be the random forest example that we did in
    class. This could work better as the are better at understanding non-linear data such as the data provided for this assignment.

