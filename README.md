# Numerical Python (Numpy)
## Experiment 2

### I. The Experiment
This experiment intends to demonstrate the programmer's comprehension and critical thinking through two problems: Normalization Problem and Divisible by Three Programs. 
These problems were designed to test the programmer's proficiency with Python's Library, Numpy, and their ability to solve them effectively.

The applications used are the Anoconda to access Jupyter Notebook, which was used for coding, and GitHub for sharing.

### II.  The Intended Outcomes
- To determine the functions and codes included in the Numpy Library
- To Utilize and apply the many codes and functions to create a Python program using the Numpy library

### III. The Problems

  #### I. Normalization Problem
    Create a random 5x5 array and store it to variable X. Normalize X and save the normalized array as X_normalized.npy.
    
    Normalization is a basic preprocessing technique in data analytics. It involves centering, subtracting 
    the mean, and scaling the division by the standard division. It is mathematically expressed as:

    Z = X - x̄ / σ

      i. Discussion: Program 1
         - The program was started by importing numpy and np.
         
         - In variable X, a random 5x5 array was stored. This array was made using the np.random.rand() function 
           in numpy, which creates an array with specified shapes and assigns random values to them.
           
         - The variable X is printed along with the 'Normal Array' string to keep the code organized.

         - A function was created for the convenience of not having to re-code the normalization process if it
           is used again. 

         - Using the numpy function np.mean(), the mean of the array elements can be found. The mean was saved in 
           the variable mean, which was done so that the code for the equation would be easier to understand.

         - As instructed, the normalized array will be stored in the variable Normalize_X, which is composed of the 
           normalization formula. In the formula a numpy function np.std() can be seen. This function computes the 
           array's standard deviation.
           
         - The variable Normalize_X is returned to send the function's result back.
         
         - As instructed, the array is saved using np.save(). This function is very important since it is essentially
           used to save a separate array that stores a set of data in npy format. Creating a npy format 
           stores all the dtype and data type information, which allows the array to be reconstructed on the same
           and different machines.
         
         - The normalized array is printed using np.load while the 'Normalized Array' string is printed using print(). These were done
           to keep the code organized and allow the comparison of the values of the normal array and normalized array.
            

#### II. Divisible By Three Problem
    Create the following 10x10 array consisting of the squares of the first 100 positive integers

    In this ndarray, find all the elements that are divisible by three and save the results as div_by_3.npy

      ii Discussion: Program 2
        - The function np.arrange() is used to arrange the number in order, while the **2 or the double star
          operator is used to square the array. 
          
        - The function .reshape(), reshapes the array to the desired rows and columns

        - The elements divisible by three is found using the remainder operator and equating the result to zero,
          any number with a zero remainder is divisible by zero which filters out all the numbers divisible by three.
          
        - As instructed, the array is saved using np.save(). This function is essential because it saves the array in .npy format
          which preserves the dtype and data type information, making it possible for the array to be reconstructed accurately on
          the same or different machines.
          
        - The array is printed by loading the newely saved array.
        
