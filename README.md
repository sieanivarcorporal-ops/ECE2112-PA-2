# ECE2112-PA-2

**Made by Siean Ivar B. Corporal | 2ECE - A**

**Objectives**
  1. create and reshape NumPy arrays using appropriate NumPy functions;
  2. perform vectorized numerical operations on an ndarray;
  3. compute array statistics and use Boolean conditions to select elements; and
  4. save computed NumPy arrays as .npy files.

# **REPRODUCIBLE NORMALIZATION PROBLEM**
  In this part of the experiment, a 5x5 matrix named X was produced and three outputs were required, the normalized array, its mean, and its standard deviation.
  The syntax used to create the randomized array was `np.random.randint` which contained the size of the array. 
  The following syntax were used:
  
  1. `X.mean()` - This syntax was used to get the mean of all the randomized elements found under the array of X and the mean of the normalized array.
  2. `X.std()` - This syntax on the other hand was used to get the standard deviation of all the randomized elements found under the array of X and the
     standard deviation of the normalized X.
  4. `(X - mean)/standarddeviation` - This syntax was used to get the normalized version of X. It gets the difference between X and the mean and is divided by its
     standard deviation.

# **CUBES DIVISIBLE BY 4 PROBLEM**
  In this part of the experiment, the first 100 integers were required to be cubed and put into a 10x10 array named C. This requirement implied that the first element
  should be 1^3 and the last should be 100^3,
  The following syntax were used:
   
  1. `np.arange(1, 101)**3` - This syntax was used to store the first 100 integers cubed into C. This meant that the integers from 1 up to 100 will be cubed and stored
     inside C.
  2. `C.reshape(10, 10)` - This syntax was used to put the elements under C in a 10 by 10 array.
  3. `C[C % 4 == 0]` - This syntax was used to get all the elements under C that is divisible by 4. The syntax `C % 4 == 0` gets the remainder of an element of C when divided by
     4 and is equated to 0. If the element satisfies the condition, it is then stored inside `div_by_4`. The whole syntax itself says that whatever element inside C that satisfies
     the condition `C % 4 == 0` will be stored inside `div_by_4`.

# **ABOVE-MEAN SQUARES PROBLEM**
  In this part of the experiment, the first 36 positive integers were required to be squared and stored under a 6x6 array named S. The mean of all the elements under S were required 
  while Boolean filtering was used to store the elements of S that are greater than its mean under above_mean.
  The following syntax were used:

  1. `np.arange(1, 37)**2` - This syntax was used to get the first 36 positive integers squared and stored under S.
  2. `S.reshape(6, 6)` - This syntax was used to store and reshape the elements under S into a 6x6 array.
  3. `S.mean()` - This syntax was used to get the mean of all the elements under S and stored under S_mean.
  4. `S[S > S_mean]` - This syntax was used to get all the elements in S that was greater than S_mean. This meant that whatever element of S that was greater than the mean of its totality
     will be stored under above_mean. 
