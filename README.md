# Multi-Threading

Matrix Multiplication Function: The `matrix_multiply()` function is responsible for performing matrix multiplication using `np.dot()`. The resulting matrix is stored at a specific index within the result array.

Multithreading Function: Within `run_with_threads()`, matrix multiplication is conducted employing a specified number of threads. It orchestrates the creation of threads for each matrix multiplication operation, initiates their execution, and then awaits their completion. The function subsequently returns the total time taken for the operation.

Matrix Definitions: We initialize a constant matrix A alongside a list containing 100 randomly generated matrices.

Execution: For each number of threads ranging from 1 to 10, `run_with_threads()` is invoked, capturing the time taken for each operation within `results_table`.

Results: Utilizing `tabulate()`, the obtained results are presented in a tabulated format.

Plotting: The number of threads is plotted against the corresponding time taken utilizing `matplotlib.pyplot.plot()`. This graph is subsequently displayed.

Observation: Notably, the minimum time taken is observed when the number of threads is 8, aligning with the expectation due to the presence of 8 cores on the laptop. Additionally, an interactive dashboard is constructed using ipywidgets, offering various refresh rates while concurrently generating random matrices.
