# Homework for the "Concurrency and Parallelism" Module

Today, as part of your homework, you will apply the concepts of multiprocessing and multithreading to develop an efficient program for parallel searching of specified keywords in text files.

Through this task, you will:

- Learn to work with files in the context of multithreading and multiprocessing programming.
- Understand how task distribution across threads or processes affects the performance and efficiency of data processing.

This task will not only deepen your understanding of multithreading and multiprocessing programming and allow you to compare the efficiency of both approaches, but it will also provide practical skills in using these concepts for optimal task distribution and resource utilization in programs.

## Technical Description of the Task

Develop a program that processes and analyzes text files in parallel to search for specified keywords. Create two versions of the program: one using the **threading** module for multithreading and the other using the **multiprocessing** module for multiprocessing.

### Step-by-Step Instructions

1. Implementation of the multithreading approach for file processing (using threading):

- Divide the list of files among different threads.
- Each thread should search for the specified keywords in its assigned set of files.
- Collect and output the search results from all threads.

2. Implementation of the multiprocessing approach for file processing (using multiprocessing):

- Divide the list of files among different processes.
- Each process should process its portion of files and search for the keywords.
- Use a data exchange mechanism (e.g., Queue) to collect and output the search results.

### Acceptance Criteria

1. The multithreading and multiprocessing approaches for file processing are implemented.
2. Files are properly distributed among threads/processes.
3. The code measures and outputs the execution time for each version.
4. Error and exception handling is ensured, particularly when working with the file system.
5. Both versions of the program return a dictionary where the key is the keyword and the value is a list of file paths where the keyword was found.
