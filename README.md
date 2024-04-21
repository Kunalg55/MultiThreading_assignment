# MultiThreading_assignment

# Methodology 
The experiment involves matrix multiplication on 100 matrices, each sized 1000 x 1000, utilizing different thread counts. Matrix multiplication is performed using the multiply() function, which employs np.dot() to compute the product of two matrices and stores the result in a designated index of the output array.

For thread utilization, the run_threads() function is devised. It supports executing matrix multiplication with a range of threads, from 1 to 10. This function initializes a list named threads to hold thread objects. It then iterates over the list of matrices, creating a new thread for each multiplication operation via the threading.Thread() constructor. Each thread starts executing using the start() method. Subsequently, after creating all threads, the function waits for all threads to finish using the join() method and records the time taken for the multiplication operations.

# Matrix Generation
Firstly, a constant matrix A of size 1000x1000 is generated using numpy.random.rand(). Then, a list containing 100 random matrices of the same size is created.

# Execution
The run_threads() function is invoked for each number of threads ranging from 1 to 10, capturing the time taken for each operation. The results are stored in the results_table list along with the corresponding number of threads.

# Results 
Finally, the results are presented in a tabular format using tabulate(), and the relationship between the number of threads and the corresponding time taken is visualized using matplotlib.pyplot.plot().

From the analysis, it's observed that the minimum time is achieved when the number of threads is set to 3.

![image](https://github.com/Kunalg55/MultiThreading_assignment/assets/142966912/6f14c810-8203-4dec-8999-2deb4780f098)

![image](https://github.com/Kunalg55/MultiThreading_assignment/assets/142966912/37ae2c58-96c9-4296-a4c6-5f6625d22b0e)

![image](https://github.com/Kunalg55/MultiThreading_assignment/assets/142966912/6c1b0129-cefe-4e73-b2ed-7059aab562f9)


