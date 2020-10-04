* Part 1. Finished
* Part 2.
    1. 5.05x speedup from ISPC, 9.05x speedup from task ISPC
    2. change the num of task to 40... Cuz you asked for 40 times improvement.
    3. I guess for the ISPC task, we don't need to define where the program give back
    the control, while in the Thread case we need to explicitly use join(). The ISPC task 
    works more like a detached thread to me.
