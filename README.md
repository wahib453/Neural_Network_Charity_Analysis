# Neural_Network_Charity_Analysis

## Purpose

To predict whether an applicant will be successful when funded by Alphabet Soup using Deep learning model.

## Procedure

1. Import dependencies.

2. Import the input dataset.

3. Generate categorical variable list.

4. Create a OneHotEncoder instance.

5. Fit and transform the OneHotEncoder.

6. Add the encoded variable names to the DataFrame.

7. Merge one-hot encoded features and drop the originals.

8. Split the preprocessed data into features and target arrays.

9. Split the preprocessed data into training and testing dataset.

10. Create a StandardScaler instance.

11. Fit the StandardScaler.

12. Scale the data.

13. Define the model.

14. Add first and second hidden layers.

15. Add the output layer.

16. Check the structure of the model.

17. Data Preprocessing I removed the EIN and NAME columns along with ORGANIZATION_Trust, USE_CASE_Other,USE_CASE_Heathcare, AFFILIATION_Other to analyze if removing certain columns would optimize accuracy rate. I left all other columns as my variables and my dependant variable as IS_Succesful.

## Compiling, Training, and Evaluating the Model

1. First Attempt
    - 2 Hidden Layers
    - 60 neurons (Layer1), 20 neurons(Layer2)
    - Used Relu and Sigmoid Activations Functions

    ![Optimization First Attempt](https://github.com/wahib453/Neural_Network_Charity_Analysis/blob/e27d1b6643ee94f46f2980a8e9be5eccf0a7650e/Resources/Optimization-FirstAttempt.PNG)

2. Second Attempt
    - 3 Hidden Layers
    - 60 neurons (Layer1), 20 neurons(Layer2), 10 neurons
    - Used Relu and Sigmoid Activations Functions

   ![Optimization Second Attempt](https://github.com/wahib453/Neural_Network_Charity_Analysis/blob/e27d1b6643ee94f46f2980a8e9be5eccf0a7650e/Resources/Optimization-SecondAttempt.PNG)

3. Third Attempt
    - 3 Hidden Layers
    - 60 neurons (Layer1), 20 neurons(Layer2), 10 neurons
    - Reordered Relu and Sigmoid Activations

    ![Optimization third Attempt](https://github.com/wahib453/Neural_Network_Charity_Analysis/blob/e27d1b6643ee94f46f2980a8e9be5eccf0a7650e/Resources/Optimization-ThirdAttempt.PNG)

## Summary

After the third attempt, only 72 percent accuracy was achieved. May be if more attempts are carried out, over 75 % will be achieved. Additionally, inspecting the data and removing outliers can help achieve 75 percent and above.
