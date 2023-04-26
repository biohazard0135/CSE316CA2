# CSE316CA2
CA2 CODE BASED SIMULATION 

Simulation-Program-for-Query-Handling

A simulation progarm for query handling for a online banking services is a software tool that simulates the behaviour of a Round Robin Scheduling Algorithm.

This code simulates a Banking service centre that handles queries from two types of customers: regular customers and new customers. 

The service centre has two queues: one for regular customers and another for new customers. Each customer is represented by a struct containing their ID, arrival time, and remaining time (i.e., the amount of time required to handle their query). 

The program first initializes the two queues and adds some customers to them. It then calculates the total number of requests (i.e., the sum of the sizes of the two queues). 

The program then enters a loop that continues as long as there are customers in either of the two queues. Within the loop, the program dequeues a customer from either of the two queues, processes their query, and either adds them back to the end of the same queue (if their query is not fully handled yet) or removes them from the queue (if their query is fully handled).

The program processes each query for a fixed time slice of 10 minutes (Time Quantum of Round Robin Scheduling). If a query takes longer than 10 minutes to process, the program adds the customer back to the queue, and the customer will be processed again in a future iteration of the loop. 

The program keeps track of the total time spent processing all queries, and after the loop finishes, it calculates the average query time by dividing the total time spent by the total number of requests. Finally, it prints out the total time spent and the average query time.

The entire implementation of the above code uses Round Robin Scheduling.
