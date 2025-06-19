# Os Lab

# Syllabus

1. Process creation and termination
2. Thread
a. Create and Join
b. Pass parameters to the thread
c. Simulate Deadlock
3. CPU scheduling algorithm(Programmatically solving mock scenarios with given data)
a. FCFS
b. SJF
c. Priority Scheduling
d. Round Robin
4. Synchronization Problems
a. Producer-Consumer Problem / Race Condition Simulation
Solve with Semaphore / Mutex
b. Reader Writers Problem(Mutex)
5. File Management
a. Create, Delete, Copy, Move
6. Shell Scripting
a. Some basic problem-solving with shell scripting

## Operating System Lab Resources

### YouTube Playlist

- [Operating System Lab - YouTube Playlist](https://www.youtube.com/playlist?list=PLlr7wO747mNp5nn0hteJFnt1rpdx6GG-_)

### GitHub Repositories

1. [avin-madhu/Operating-System-Lab](https://github.com/avin-madhu/Operating-System-Lab)
    
    KTU S4 LAB 2023 - OPERATING SYSTEM LAB PROGRAMS AND ALGORITHMS
    
2. [fahimahammed/operating-system-lab](https://github.com/fahimahammed/operating-system-lab)
    - [Deadlock Detection Algorithm](https://github.com/fahimahammed/operating-system-lab/blob/main/7-deadlock-detection.cpp)
3. [ahnafshahrear/Operating-System-Lab](https://github.com/ahnafshahrear/Operating-System-Lab)
    - [Banker's Algorithm](https://github.com/ahnafshahrear/Operating-System-Lab/blob/main/bankers-algorithm.cpp)
    
    You have to setup your PC(personal or in the Lab) with your desired OS to simulate the
    lab final tasks.
    Practice the problems in the shared contents and search out more problem online to
    judge your knowledge to get well on the Lab final
    Be prepared for the viva after Lab exam
    

---

# Practice note:

- Question
    
    ‭ Problem Statement #01: (30 marks)‬
    
    ‭ Write a multithreaded program that reads‬**‭ three positive‬‭ integers‬**‭ from input. Create‬**‭ three separate‬**
    
    **‭ threads‬**‭ , each responsible for computing the‬**‭ factorial‬**‭ of one number.‬
    
    ‭ Once all threads finish their computations, the‬**‭ main‬‭ thread will join them‬**‭ , collect their results, and‬
    
    ‭ print:‬
    
    ●
    
    ‬‭ Each number and its factorial‬
    
    ●
    
    ‬‭ The‬**‭ sum‬**‭ of all three factorials‬
    
    ‭
    
    ‭
    
    ‭ Standard Inputs:‬
    
    ‭ A single line with three positive integers:‬
    
    ‭ Case 1: 3 4 5‬
    
    ‭ Output:‬
    
    ‭ Print the sum of the first half, the sum of the second half, and the total sum in the following format:‬
    
    | ‭ Factorial of 3 is:‬ | ‭ 6‬ |
    | --- | --- |
    | ‭ Factorial of 4 is:‬ | ‭ 24‬ |
    | ‭ Factorial of 5 is:‬ | ‭ 120‬ |
    | ‭ The sum of all factorials is:‬ | ‭ 150‬ |
    
    ‭ Problem Statement #02: (30 marks)‬
    
    ‭ Problem: Automate the Directory Backup Process‬
    
    ‭ Create a shell script named‬**‭ backup_manager.sh‬**‭ that performs the following steps:‬
    
    **‭ Step 1: User Input‬**
    
    ‭ Prompt the user to enter a directory path they want to back up.‬
    
    ‭ Store the input in a variable.‬
    
    **‭ Step 2: Directory Existence Check‬**
    
    ‭ - If the directory does not exist:‬
    
    ‭ - Notify the user that the directory is invalid.‬
    
    ‭ - Exit the script with an error message.‬
    
    ‭ - If the directory exists:‬
    
    ‭ - Inform the user that the directory will be backed up.‬
    
    **‭ Step 3: Backup Directory Creation‬**
    
    ‭ - Check if a‬**‭ /backups‬**‭ directory exists in the current folder.‬
    
    ‭ - If it doesn't exist, create it and notify the user.‬
    
    ‭ - If it exists, confirm that backups will be stored there.‬
    
    **‭ Step 4: Backup and Cleanup a file‬**
    
    ‭ - Prompt the user to enter a file they want to back up.‬
    
    ‭ - If the file does not exist:‬
    
    ‭ - Notify the user that the file is invalid.‬
    
    ‭ - Exit the script with an error message.‬
    
    ‭ - If the file exists:‬
    
    ‭ - Move the file to‬**‭ /backups‬**‭ and delete it from the old directory‬
    
    ‭ Example Workflow‬
    
    ‭ A user might interact with your script like this:‬
    
    ‭ $ ./backup_manager.sh‬
    
    ‭ Enter the directory path to back up: ~/mydocs‬
    
    ‭ Directory found: /home/user/mydocs‬
    
    ‭ Using existing backup directory: ./backups‬
    
    ‭ Enter the filename to back up: report.txt‬
    
    ‭ File 'report.txt' moved to ./backups and removed from original location‬**‭ Hints:‬**
    
    **‭ File Test Operators in Bash‬**
    
    | ‭ Test‬
    ‭ Expression‬ |  | ‭ Checks If...‬‭ Description‬ |
    | --- | --- | --- |
    | ‭ | -e FILE‬‭ file exists‬‭ True if file exists‬ |  |
    | ‭
    -f | FILE‬‭ regular file‬‭ True if it's a normal file (not directory/device)‬ |  |
    | ‭ | -d FILE‬‭ directory‬‭ True if it's a directory‬ |  |
    | ‭
    -r | FILE‬‭ readable‬‭ True if file has read permission‬ |  |
    | ‭
    -w | FILE‬‭ writable‬‭ True if file has write permission‬ |  |
    | ‭
    -x | FILE‬‭ executable‬‭ True if file has execute permission‬ |  |
    | ‭
    -s | FILE‬‭ non-empty file‬‭ True if file exists and is not empty‬ |  |
    | ‭
    -L | FILE‬‭ symbolic link‬‭ True if file is a symbolic link‬ |  |
    | ‭
    -b | FILE‬‭ block device‬‭ True if file is a block special device‬ |  |
    | ‭
    -c | FILE‬‭ character device‬‭ True if file is a character special device‬ |  |
    | ‭
    -N | FILE‬‭ modified since last read‬‭ True if file was modified after last read‬ |  |
    | ‭
    -O | FILE‬‭ owned by current user‬‭ True if the user owns the file‬ |  |
    | ‭
    -G | FILE‬‭ owned by user’s group‬‭ True if file belongs to the user’s group‬ |  |
- Process creation and termination
    - Creation
        
        ```c
        #include <stdio.h>
        #include <unistd.h>
        #include <sys/wait.h>
        
        int main() {
            pid_t pid = fork(); // Create a child
        
            if (pid == 0) {
                // This is the child process
                printf("Child: PID = %d, Parent PID = %d\n", getpid(), getppid());
            } else if (pid > 0) {
                // This is the parent process
                printf("Parent: PID = %d, Child PID = %d\n", getpid(), pid);
                wait(NULL); // Wait for child to finish
            } else {
                // fork failed
                printf("Fork failed\n");
            }
        
            return 0;
        }
        ```
        
        ```cpp
        output:
        Parent: PID = 13760, Child PID = 13763
        Child: PID = 13763, Parent PID = 13760
        
        visuals:
        
        [Parent]
           |
         fork()
          / \
         /   \
        [Parent] [Child]
         |         |
        wait()   prints
         |         |
         |        exits
         |
        continues
        ```
        
    
    ### Orphan: If the sleep() on child than;
    
    - Example
        
        
        ```c
        #include <stdio.h>
        #include <unistd.h>  // for fork(), sleep()
        
        int main() {
        pid_t pid = fork();  // Create child
        if (pid == 0) {
            // Child process
            printf("Child: My PID = %d\\n", getpid());
            sleep(5);  // Child sleeps (parent dies during this time)
            printf("Child: Now I'm an orphan! My new parent = %d\\n", getppid());
        } else {
            // Parent process
            printf("Parent: My PID = %d\\n", getpid());
            sleep(1);  // Parent dies after 1 second (child still sleeping)
            printf("Parent: Dying now...\\n");
        }
        return 0;
        }
        ```
        
    
    ### Zombie: If the sleep(10)/wait(NULL) on parent and _exit(0)on child than;
    
    - Example
        
        ```c
        #include <stdio.h>
        #include <unistd.h>
        #include <stdlib.h>
        
        int main() {
            printf("Parent PID: %d\n", getpid());
            
            // Fork a child process
            pid_t child_pid = fork();
        
            if (child_pid == 0) {
                // Child process
                printf("Child PID: %d (I'll become a zombie!)\n", getpid());
                exit(0);  // Child exits immediately
            } else {
                // Parent process (does NOT wait for child)
                printf("Parent is running but NOT calling wait()...\n");
                printf("Check 'ps aux | grep Z' in another terminal!\n");
                
                // Parent keeps running (zombie child remains)
                sleep(30);  // Sleep for 30 seconds (zombie exists during this time)
                
                printf("Parent exiting now... zombie will be gone.\n");
            }
        
            return 0;
        }
        ```
        
    - **Key Differences**
        
        ### **What is `init`?**
        
        - **PID 1**: The `init` process is the **first process** started by the kernel during boot.
        
        | Feature | Zombie Process | Orphan Process |
        | --- | --- | --- |
        | **State** | Terminated (dead) | Still running (alive) |
        | **Parent** | Alive but didn’t `wait()` | Dead (reparented to `init`) |
        | **Resource Use** | Wastes PID (process table slot) | No resource leak |
        | **Cleanup** | Manual `wait()` required | Automatic (by `init`) |
        
        ### **1. `sleep()`**
        
        - **Purpose:** Pauses the **current process** for a fixed amount of time.
        
        ### **2. `wait()`**
        
        - **Purpose:** Makes the **parent process pause** until a **child process terminates**.
    
- Thread
    
    ---
    
    - **Thread Creation**
        
        ### **🔧 Code Example:**
        
        ```c
        #include <stdio.h>
        #include <pthread.h>
        
        void* myThread(void* arg) {
            printf("Hello from thread!\n");
            return NULL;
        }
        
        int main() {
            pthread_t thread;
        
            // Create the thread
            pthread_create(&thread, NULL, myThread, NULL);
        
            // Join the thread (wait for it to finish)
            pthread_join(thread, NULL);
        
            printf("Thread has finished.\n");
            return 0;
        }
        ```
        
    
    ---
    
    - **Pass Parameters to the Thread**
        
        ### **🔧 Code Example:**
        
        ```c
        #include <stdio.h>
        #include <pthread.h>
        
        void* printMessage(void* arg) {
            char* message = (char*) arg;
            printf("Thread received: %s\n", message);
            return NULL;
        }
        
        int main() {
            pthread_t thread;
            char* msg = "Hello, parameter!";
        
            pthread_create(&thread, NULL, printMessage, (void*) msg);
            pthread_join(thread, NULL);
        
            return 0;
        }
        ```
        
    
    ---
    
    - **Simulate Deadlock Using Threads and Mutexes**
        
        ### **🔧 Code Example:**
        
        ```c
        #include <stdio.h>
        #include <pthread.h>
        #include <unistd.h>
        
        pthread_mutex_t lock1 = PTHREAD_MUTEX_INITIALIZER;
        pthread_mutex_t lock2 = PTHREAD_MUTEX_INITIALIZER;
        
        void* thread1_func(void* arg) {
            pthread_mutex_lock(&lock1);
            sleep(1);  // Simulate delay
            pthread_mutex_lock(&lock2);
        
            printf("Thread 1 acquired both locks\n");
        
            pthread_mutex_unlock(&lock2);
            pthread_mutex_unlock(&lock1);
            return NULL;
        }
        
        void* thread2_func(void* arg) {
            pthread_mutex_lock(&lock2);
            sleep(1);  // Simulate delay
            pthread_mutex_lock(&lock1);
        
            printf("Thread 2 acquired both locks\n");
        
            pthread_mutex_unlock(&lock1);
            pthread_mutex_unlock(&lock2);
            return NULL;
        }
        
        int main() {
            pthread_t t1, t2;
        
            pthread_create(&t1, NULL, thread1_func, NULL);
            pthread_create(&t2, NULL, thread2_func, NULL);
        
            pthread_join(t1, NULL);
            pthread_join(t2, NULL);
        
            return 0;
        }
        ```
        
        - c++ code
            
            ```cpp
            #include <iostream>
            #include <thread>
            #include <mutex>
            #include <chrono>
            
            using namespace std;
            
            mutex lock1;
            mutex lock2;
            
            void thread1_func() {
                lock1.lock();
                this_thread::sleep_for(chrono::seconds(1));  // Simulate delay
                lock2.lock();
            
                cout << "Thread 1 acquired both locks" << endl;
            
                lock2.unlock();
                lock1.unlock();
            }
            
            void thread2_func() {
                lock2.lock();
                this_thread::sleep_for(chrono::seconds(1));  // Simulate delay
                lock1.lock();
            
                cout << "Thread 2 acquired both locks" << endl;
            
                lock1.unlock();
                lock2.unlock();
            }
            
            int main() {
                thread t1(thread1_func);
                thread t2(thread2_func);
            
                t1.join();
                t2.join();
            
                return 0;
            }
            ```
            
        
        A **critical section** is a code segment where **shared resources** are accessed, that must not be concurrently access**ed by more that one thread.**
        
    - practice
        - c++
            
            ---
            
            ---
            
            ## **✅ 1.**
            
            ## **Basic Thread Creation**
            
            ```cpp
            #include <iostream>
            #include <thread>
            
            using namespace std;
            
            void greet() {
                cout << "Hello from thread!" << endl;
            }
            
            int main() {
                thread t(greet);  // Start thread
                t.join();         // Wait for thread to finish
                return 0;
            }
            ```
            
            ---
            
            ## **✅ 2.**
            
            ## **Passing Parameters to Threads**
            
            ```cpp
            #include <iostream>
            #include <thread>
            
            using namespace std;
            
            void printValue(int x) {
                cout << "Value: " << x << endl;
            }
            
            int main() {
                thread t(printValue, 42);
                t.join();
                return 0;
            }
            ```
            
            ---
            
            ## **✅ 3.**
            
            ## **Sum Calculation Using Two Threads**
            
            ```cpp
            #include <iostream>
            #include <thread>
            
            using namespace std;
            
            int arr[10] = {1,2,3,4,5,6,7,8,9,10};
            int sum1 = 0, sum2 = 0;
            
            void sumFirstHalf() {
                for (int i = 0; i < 5; ++i) {
                    sum1 += arr[i];
                }
            }
            
            void sumSecondHalf() {
                for (int i = 5; i < 10; ++i) {
                    sum2 += arr[i];
                }
            }
            
            int main() {
                thread t1(sumFirstHalf);
                thread t2(sumSecondHalf);
            
                t1.join();
                t2.join();
            
                cout << "Sum of first half: " << sum1 << endl;
                cout << "Sum of second half: " << sum2 << endl;
                cout << "Total sum: " << sum1 + sum2 << endl;
            
                return 0;
            }
            ```
            
            ---
            
            ## **🔐 4.**
            
            ## **Using Mutex for Safe Access (Race Condition Prevention)**
            
            ```cpp
            #include <iostream>
            #include <thread>
            #include <mutex>
            
            using namespace std;
            
            int total = 0;
            mutex mtx;
            
            void add(int value) {
                lock_guard<mutex> lock(mtx); // Automatically locks and unlocks
                total += value;
            }
            
            int main() {
                thread t1(add, 10);
                thread t2(add, 20);
            
                t1.join();
                t2.join();
            
                cout << "Total: " << total << endl;
                return 0;
            }
            ```
            
            ---
            
            ## **⚠️ 5.**
            
            ## **Deadlock Example (Don’t Do This)**
            
            ```cpp
            #include <iostream>
            #include <thread>
            #include <mutex>
            
            using namespace std;
            
            mutex m1, m2;
            
            void threadA() {
                lock_guard<mutex> lockA(m1);
                this_thread::sleep_for(chrono::milliseconds(100));
                lock_guard<mutex> lockB(m2);
                cout << "Thread A done" << endl;
            }
            
            void threadB() {
                lock_guard<mutex> lockB(m2);
                this_thread::sleep_for(chrono::milliseconds(100));
                lock_guard<mutex> lockA(m1);
                cout << "Thread B done" << endl;
            }
            
            int main() {
                thread t1(threadA);
                thread t2(threadB);
            
                t1.join();
                t2.join();
            
                return 0;
            }
            ```
            
            ---
            
            ## **✔️ 6.**
            
            ## **Avoid Deadlock Using std::lock()**
            
            ```cpp
            #include <iostream>
            #include <thread>
            #include <mutex>
            
            using namespace std;
            
            mutex m1, m2;
            
            void safeThreadA() {
                lock(m1, m2); // Lock both at once
                lock_guard<mutex> lockA(m1, adopt_lock);
                lock_guard<mutex> lockB(m2, adopt_lock);
                cout << "Safe Thread A done" << endl;
            }
            
            void safeThreadB() {
                lock(m1, m2); // Lock both at once
                lock_guard<mutex> lockA(m1, adopt_lock);
                lock_guard<mutex> lockB(m2, adopt_lock);
                cout << "Safe Thread B done" << endl;
            }
            
            int main() {
                thread t1(safeThreadA);
                thread t2(safeThreadB);
            
                t1.join();
                t2.join();
            
                return 0;
            }
            ```
            
            ---
            
            ## **🧠 Best Practices**
            
            | **Practice** | **Why it’s important** |
            | --- | --- |
            | Use thread.join() | Prevents early program exit or zombie threads |
            | Use mutex or lock_guard | Prevent race conditions |
            | Avoid locking in opposite order | Prevent deadlocks |
            | Use std::lock() with adopt_lock | Safely lock multiple mutexes |
            
            ---
            
        
        ---
        
        - A single array of **10 elements**.
        - **Thread 1** sums **elements 0 to 4** (first 5).
        - **Thread 2** sums **elements 5 to 9** (last 5).
        - Both threads return their result to the **main thread**.
        - **Main thread adds** both and shows the final result.
        
        ---
        
        ### **✅ Clean and Simple Example**
        
        ```c
        #include <stdio.h>
        #include <pthread.h>
        
        int arr[10] = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
        
        void* sum_first_half(void* arg) {
            int* sum = (int*)malloc(sizeof(int));
            *sum = 0;
            for (int i = 0; i < 5; i++) {
                *sum += arr[i];
            }
            return (void*)sum;
        }
        
        void* sum_second_half(void* arg) {
            int* sum = (int*)malloc(sizeof(int));
            *sum = 0;
            for (int i = 5; i < 10; i++) {
                *sum += arr[i];
            }
            return (void*)sum;
        }
        
        int main() {
            pthread_t t1, t2;
            int *sum1, *sum2;
        
            pthread_create(&t1, NULL, sum_first_half, NULL);
            pthread_create(&t2, NULL, sum_second_half, NULL);
        
            pthread_join(t1, (void**)&sum1);  // Get return value of thread 1
            pthread_join(t2, (void**)&sum2);  // Get return value of thread 2
        
            int total = *sum1 + *sum2;
        
            printf("Sum by Thread 1 (1–5): %d\n", *sum1);
            printf("Sum by Thread 2 (6–10): %d\n", *sum2);
            printf("Total Sum: %d\n", total);
        
            free(sum1);
            free(sum2);
        
            return 0;
        }
        ```
        
        ---
        
        ### **🟢 Output:**
        
        ```
        Sum by Thread 1 (1–5): 15
        Sum by Thread 2 (6–10): 40
        Total Sum: 55
        ```
        
        ---
        
        - We have an **array of integers**.
        - We split the array **into two halves**.
        - We use **two threads** — each one calculates the **sum** of one half.
        - The **main thread waits** for both and **adds the two sums**.
        
        ---
        
        ## **✅ Program: Two-thread array sum**
        
        ```
        #include <stdio.h>
        #include <pthread.h>
        
        #define SIZE 8  // Array size
        
        int arr[SIZE] = {1, 2, 3, 4, 5, 6, 7, 8}; // Array to sum
        
        typedef struct {
            int start;     // Start index of sub-array
            int end;       // End index of sub-array
            int sum;       // Result of sum (to be filled by thread)
        } ThreadData;
        
        void* sumArray(void* arg) {
            ThreadData* data = (ThreadData*)arg;
            data->sum = 0;
            for (int i = data->start; i <= data->end; i++) {
                data->sum += arr[i];
            }
            return NULL;
        }
        
        int main() {
            pthread_t t1, t2;
            ThreadData data1 = {0, (SIZE / 2) - 1};     // First half
            ThreadData data2 = {SIZE / 2, SIZE - 1};    // Second half
        
            pthread_create(&t1, NULL, sumArray, &data1);
            pthread_create(&t2, NULL, sumArray, &data2);
        
            pthread_join(t1, NULL);
            pthread_join(t2, NULL);
        
            int totalSum = data1.sum + data2.sum;
        
            printf("Sum of first half: %d\n", data1.sum);
            printf("Sum of second half: %d\n", data2.sum);
            printf("Total sum: %d\n", totalSum);
        
            return 0;
        }
        ```
        
        ---
        
        ### **🧠 What’s happening:**
        
        - Array {1,2,3,4,5,6,7,8} is split into:
            - Thread 1: indexes 0 to 3 → sum = 1+2+3+4 = 10
            - Thread 2: indexes 4 to 7 → sum = 5+6+7+8 = 26
        - Final sum = 10 + 26 = 36
        
        ---
        
        ### **🟢 Output:**
        
        ```
        Sum of first half: 10
        Sum of second half: 26
        Total sum: 36
        ```
        
        ---
        
        ---
        
    
    ---
    
- CPU Scheduling  Algorithm
    - FCFS
        
        ```cpp
        #include <bits/stdc++.h>
        
        using namespace std;
        
        struct process
        {
            string id;
            int burst, waiting, turnaround;
        };
        
        int main()
        {
            int size;
            cin >> size;
            vector<process> x(size);
        
            for (int i = 0; i < size; i++)
            {
                cin >> x[i].id >> x[i].burst;
            }
            
            int time_now = 0;
            double avg_waiting = 0, avg_turnaround = 0;
            vector<pair<string, int>> timeline;
        
            for (int i = 0; i < size; i++)
            {
                time_now += x[i].burst;
                timeline.push_back({x[i].id, time_now});
                x[i].turnaround = time_now;
                x[i].waiting = x[i].turnaround - x[i].burst;
                avg_waiting += x[i].waiting;
                avg_turnaround += x[i].turnaround;
            }
        
            string gantt_chart = "|", border = "-";
            for (auto z: timeline)
            {
                gantt_chart += "  " + z.first + "  |";
                border += "-------";
            }
            cout << "Gantt Chart:\n" << border << "\n" 
                 << gantt_chart << "\n"
                 << border << "\n"
                 << "0";
        
            int index = 0;
            for (int i = 1; gantt_chart[i]; i++)
            {
                if (gantt_chart[i] == '|')
                {
                    cout << timeline[index].second;
                    if (timeline[index++].second >= 10) 
                    {
                        i++;
                    }
                }
                else cout << " ";
            }
        
            cout << "\n\n"
                 << "Average waiting time = " << avg_waiting / size << "\n"
                 << "Average turnaround time = " << avg_turnaround / size << "\n\n"
                 << "Process   |   Waiting Time   |   Turnaround Time\n"
                 << "------------------------------------------------\n";
            for (int i = 0; i < size; i++)
            {
                cout << x[i].id << "              "
                     << x[i].waiting << "                   "
                     << x[i].turnaround << "\n";
            }
        }
        
        /*//... Sample Input-Output:
        ___________________________________________________________________________________________________________________________________________________________________________________________________________________________
        Input:
        5
        P1 13
        P2 3
        P3 17
        P4 4
        P5 2
        ___________________________________________________________________________________________________________________________________________________________________________________________________________________________
        Output:
        Gantt Chart:
        ------------------------------------
        |  P1  |  P2  |  P3  |  P4  |  P5  |
        ------------------------------------
        0      13     16     33     37     39 
        
        Average waiting time = 19.8
        Average turnaround time = 27.6
        
        Process   |   Waiting Time   |   Turnaround Time
        ------------------------------------------------
        P1              0                    13
        P2              13                   16
        P3              16                   33
        P4              33                   37
        P5              37                   39
        
        *///...
        ```
        
    - SJF
        
        ```cpp
        #include <bits/stdc++.h>
        
        using namespace std;
        
        struct process
        {
            string id;
            int burst, waiting, turnaround;
        };
        
        bool compareProcess(process x, process y)
        {
            return x.burst < y.burst;
        }
        
        int main()
        {
            int size;
            cin >> size;
            vector<process> x(size);
        
            for (int i = 0; i < size; i++)
            {
                cin >> x[i].id >> x[i].burst;
            }
            sort(x.begin(), x.end(), compareProcess);
        
            int time_now = 0;
            double avg_waiting = 0, avg_turnaround = 0;
            vector<pair<string, int>> timeline;
        
            for (int i = 0; i < size; i++)
            {
                time_now += x[i].burst;
                timeline.push_back({x[i].id, time_now});
                x[i].turnaround = time_now;
                x[i].waiting = x[i].turnaround - x[i].burst;
                avg_waiting += x[i].waiting;
                avg_turnaround += x[i].turnaround;
            }
        
            string gantt_chart = "|", border = "-";
            for (auto z: timeline)
            {
                gantt_chart += "  " + z.first + "  |";
                border += "-------";
            }
            cout << "Gantt Chart:\n" << border << "\n" 
                 << gantt_chart << "\n"
                 << border << "\n"
                 << "0";
        
            int index = 0;
            for (int i = 1; gantt_chart[i]; i++)
            {
                if (gantt_chart[i] == '|')
                {
                    cout << timeline[index].second;
                    if (timeline[index++].second >= 10) 
                    {
                        i++;
                    }
                }
                else cout << " ";
            }
        
            cout << "\n\n"
                 << "Average waiting time = " << avg_waiting / size << "\n"
                 << "Average turnaround time = " << avg_turnaround / size << "\n\n"
                 << "Process   |   Waiting Time   |   Turnaround Time\n"
                 << "------------------------------------------------\n";
            for (int i = 0; i < size; i++)
            {
                cout << x[i].id << "              "
                     << x[i].waiting << "                   "
                     << x[i].turnaround << "\n";
            }
        }
        
        /*//... Sample Input-Output:
        ___________________________________________________________________________________________________________________________________________________________________________________________________________________________
        Input:
        4
        P1 6
        P2 8
        P3 7
        P4 3
        
        ___________________________________________________________________________________________________________________________________________________________________________________________________________________________
        Output:
        Gantt Chart:
        ------------------------------------
        |  P5  |  P4  |  P1  |  P3  |  P2  |
        ------------------------------------
        0      2      5      11     18     26 
        
        Average waiting time = 7.2
        Average turnaround time = 12.4
        
        Process   |   Waiting Time   |   Turnaround Time
        ------------------------------------------------
        P5              0                   2
        P4              2                   5
        P1              5                   11
        P3              11                  18
        P2              18                  26
        
        *///...
        ```
        
    - Priority Scheduling
        
        ```cpp
        #include <bits/stdc++.h>
        
        using namespace std;
        
        struct process
        {
            string id;
            int burst, priority, waiting, turnaround;
        };
        
        bool compareProcess(process x, process y)
        {
            return x.priority < y.priority;
        }
        
        int main()
        {
            int size;
            cin >> size;
            vector<process> x(size);
        
            for (int i = 0; i < size; i++)
            {
                cin >> x[i].id >> x[i].burst >> x[i].priority;
            }
            sort(x.begin(), x.end(), compareProcess);
        
            int time_now = 0;
            double avg_waiting = 0, avg_turnaround = 0;
            vector<pair<string, int>> timeline;
        
            for (int i = 0; i < size; i++)
            {
                time_now += x[i].burst;
                timeline.push_back({x[i].id, time_now});
                x[i].turnaround = time_now;
                x[i].waiting = x[i].turnaround - x[i].burst;
                avg_waiting += x[i].waiting;
                avg_turnaround += x[i].turnaround;
            }
        
            string gantt_chart = "|", border = "-";
            for (auto z: timeline)
            {
                gantt_chart += "  " + z.first + "  |";
                border += "-------";
            }
            cout << "Gantt Chart:\n" << border << "\n" 
                 << gantt_chart << "\n"
                 << border << "\n"
                 << "0";
        
            int index = 0;
            for (int i = 1; gantt_chart[i]; i++)
            {
                if (gantt_chart[i] == '|')
                {
                    cout << timeline[index].second;
                    if (timeline[index++].second >= 10) 
                    {
                        i++;
                    }
                }
                else cout << " ";
            }
        
            cout << "\n\n"
                 << "Average waiting time = " << avg_waiting / size << "\n"
                 << "Average turnaround time = " << avg_turnaround / size << "\n\n"
                 << "Process   |   Waiting Time   |   Turnaround Time\n"
                 << "------------------------------------------------\n";
            for (int i = 0; i < size; i++)
            {
                cout << x[i].id << "              "
                     << x[i].waiting << "                   "
                     << x[i].turnaround << "\n";
            }
        }
        
        /*//... Sample Input-Output:
        ___________________________________________________________________________________________________________________________________________________________________________________________________________________________
        Input:
        5
        P1 10 3
        P2 1 1
        P3 2 4
        P4 1 5
        P5 5 2
        
        ___________________________________________________________________________________________________________________________________________________________________________________________________________________________
        Output:
        Gantt Chart:
        ------------------------------------
        |  P2  |  P5  |  P1  |  P3  |  P4  |
        ------------------------------------
        0      1      6      16     18     19 
        
        Average waiting time = 8.2
        Average turnaround time = 12
        
        Process   |   Waiting Time   |   Turnaround Time
        ------------------------------------------------
        P2              0                   1
        P5              1                   6
        P1              6                   16
        P3              16                  18
        P4              18                  19
        
        *///...
        ```
        
    - Round Robin
        
        ```cpp
        #include <bits/stdc++.h>
        
        using namespace std;
        
        struct process
        {
            string id;
            int burst, waiting, turnaround;
        };
        
        int main()
        {
            int size;
            cin >> size;
            vector<process> x(size);
            queue<process> waiting_list;
        
            for (int i = 0; i < size; i++)
            {
                cin >> x[i].id >> x[i].burst;
                waiting_list.push(x[i]);
            }
            
            int time_now = 0, quantum = 4;
            double avg_waiting = 0, avg_turnaround = 0;
            vector<pair<string, int>> timeline;
        
            while (!waiting_list.empty())
            {
                process now = waiting_list.front();
                waiting_list.pop();
                int quantum_now = min(now.burst, quantum);
                if (waiting_list.size() == 0)
                {
                    quantum_now = now.burst;
                }
                time_now += quantum_now;
                timeline.push_back({now.id, time_now});
                now.burst -= quantum_now;
                if (!now.burst)
                {
                    for (auto &p: x)
                    {
                        if (p.id == now.id)
                        {
                            p.turnaround = time_now;
                            p.waiting = time_now - p.burst;
                            avg_waiting += p.waiting;
                            avg_turnaround += p.turnaround;
                            break;
                        }
                    }
                }
                else waiting_list.push(now);
            }
        
            string gantt_chart = "|", border = "-";
            for (auto z: timeline)
            {
                gantt_chart += "  " + z.first + "  |";
                border += "-------";
            }
            cout << "Gantt Chart:\n" << border << "\n" 
                 << gantt_chart << "\n"
                 << border << "\n"
                 << "0";
        
            int index = 0;
            for (int i = 1; gantt_chart[i]; i++)
            {
                if (gantt_chart[i] == '|')
                {
                    cout << timeline[index].second;
                    if (timeline[index++].second >= 10) 
                    {
                        i++;
                    }
                }
                else cout << " ";
            }
        
            cout << "\n\n"
                 << "Average waiting time = " << avg_waiting / size << "\n"
                 << "Average turnaround time = " << avg_turnaround / size << "\n\n"
                 << "Process   |   Waiting Time   |   Turnaround Time\n"
                 << "------------------------------------------------\n";
            for (int i = 0; i < size; i++)
            {
                cout << x[i].id << "              "
                     << x[i].waiting << "                   "
                     << x[i].turnaround << "\n";
            }
        }
        
        /*//... Sample Input-Output:
        ___________________________________________________________________________________________________________________________________________________________________________________________________________________________
        Input:
        3
        P1 24
        P2 3
        P3 3
        ___________________________________________________________________________________________________________________________________________________________________________________________________________________________
        Output:
        Gantt Chart:
        ---------------------------------------------------------
        |  P1  |  P2  |  P3  |  P1  |  P1  |  P1  |  P1  |  P1  |
        ---------------------------------------------------------
        0      4      7      10     14     18     22     26     30  
        
        Average waiting time = 5.66667
        Average turnaround time = 15.6667
        
        Process   |   Waiting Time   |   Turnaround Time
        ------------------------------------------------
        P1              6                   30
        P2              4                   7
        P3              7                   10
        
        *///...
        ```
        
- Synchronization Problems
    - Producer Consumer
        
        ### Mutex/Semaphore
        
        ```c
        // Producer Consumer Problem 
        
        #include <stdio.h>
        
        int mutex = 0; // for mutual exclusion 
        int full = 0;// false initially
        int empty = 1; // true initally
        int bufferSize;
        int items=0; // to keep count of the number of items
        
        void producer()
        {
          mutex = 1;
          empty = 0;
          items++;
          printf("\nproducer produced item-%d", items);
          if(items == bufferSize)
          {
            full = 1; // buffer is full
          }
           mutex = 0;
        }
        
        void consumer()
        {
          mutex = 1;
          full = 0;
          printf("\nconsumer consumed item-%d \n", items);
          items--;
          if(items == 0)
          {
            empty = 1; // buffer is full
          }
           mutex = 0;
        }
        
        int main()
        {
           printf("Enter the buffer size: ");
           scanf("%d", &bufferSize);
           int choice;
           do 
           {
              printf("\n\n     SELECT OPERATION\n-----------------------------\n1) produce an item\n2) consume an item\n3) Check if full\n4) Check if empty\n5) Exit");
              printf("\n-----------------------------\nEnter your choice: ");
              scanf("%d", &choice);
              if (choice == 1&& mutex == 0)
              {
                if(full == 0)
                {
                    producer();
                }
                else
                {
                    printf("\n The buffer is full!\n"); 
                }
              }
              else if (choice == 2 && mutex == 0)
              {
                if(empty == 0)
                {
                    consumer();
                }
                else
                {
                    printf("\n The buffer is empty!\n");
                }
              }
              else if (choice == 3)
              {
                 if(full == 1)
                 {
                    printf("\n The buffer is full!\n");
                 }
                 else
                 {
                    printf("\n The buffer has more space..\n");
                 }
              }
              else if (choice == 4)
              {
                 if(empty == 1)
                 {
                    printf("\n The buffer is empty!\n");
                 }
                 else
                 {
                    printf("\n The buffer has more items..\n");
                 }
              }
              else if(choice == 5)
              {
                printf("\n Exiting code...\n\n");
              }
           }while(choice != 5);
        }
        ```
        
    - Readers Writer
        
        ### Mutex
        
        ```c
        #include <stdio.h>
        
        int writing = 0; // none is writing at the start
        int reading = 0; // none is reading at the start
        int readerCount = 0; // checks number of readers
        int mutex = 1;
        
        void read()
        {
            mutex=0;
            reading = 1;
            readerCount++;
            printf("\nReader(%d) is reading...\n", readerCount);
            mutex=1;
        
        }
        
        void write()
        {
            mutex=0;
            writing = 1;
            printf("\nWriter(%d) is writing...\n", writing);
            mutex=1;
        }
        
        int main()
        {
             int choice;
        
            do 
           {
              printf("\n\n     SELECT OPERATION\n-----------------------------\n1) Read\n2) Write\n3) delete last reader\n4) delete last writer\n5) Exit");
              printf("\n-----------------------------\nEnter your choice: ");
              scanf("%d", &choice);
        
              if(choice == 1) // read 
              {
                  if(writing == 0&&mutex==1)
                  {
                    read();
                  }
                  else
                  {
                   printf("\nCannot read, A writer is currently writing...\n");
                  }  
              }
              else if (choice == 2) // write
              {
        
                 if(reading == 0 && mutex==1 && writing== 0)
                 {
                    write();
                 }
                 else if(writing == 1)
                 {
                    printf("\nCannot write, A writer is currently writing...\n");
                 }
                 else
                 {
                    printf("\nCannot write, A Reader is currently reading...\n");
                 }
              }
              else if (choice == 3)
              {
                 if(readerCount == 0)
                 {
                    printf("\n No Readers are reading !\n");
                 }
                 else
                 {
                    printf("\nA reader(%d) is removed\n",readerCount);
                    readerCount--;
                    if(readerCount == 0)
                    {
                       reading=0;
                    }
                 }
              }
              else if (choice == 4)
              {
                 if(writing==0)
                 {
                    printf("\ncurrently none is writing..\n");
                 }
                 else
                 {
                     printf("\nThe writer is removed!\n");
                     writing=0;
                 }
              }
             else if (choice == 5)
             {
                printf("\n Exiting code ...\n\n");
             }
             
           }while(choice != 5);
        }
        ```
        
    
- File Management
    - Create
        
        ### 1. Create
        
        **File:**
        
        ```bash
        touch filename.txt          # Create empty file
        echo "content" > file.txt  # Create file with content
        
        ```
        
        **Directory:**
        
        ```bash
        mkdir dirname              # Create single directory
        mkdir -p parent/child      # Create nested directories
        
        ```
        
    - Delete
        
        ### 2. Delete
        
        **File:**
        
        ```bash
        rm filename.txt            # Delete file
        rm -i file.txt            # Confirm before delete
        
        ```
        
        **Directory:**
        
        ```bash
        rmdir dirname              # Delete empty directory
        rm -r dirname             # Delete directory and contents (recursive)
        rm -rf dirname            # Force delete without confirmation (DANGEROUS)
        
        ```
        
    - Copy
        
        ### 3. Copy
        
        - Note
            
            Here are the most common ways:
            
            ---
            
            ### **✅ 1.**
            
            ### **Using cp (copy file)**
            
            This copies the **entire file**, not just its content:
            
            ```
            cp source.txt destination.txt
            ```
            
            - If destination.txt doesn’t exist, it will be created.
            - If it **does exist**, its content will be **overwritten**.
            
            ---
            
            ### **✅ 2.**
            
            ### **Using cat with > (redirect)**
            
            To copy the **contents** of one file into another:
            
            ```
            cat source.txt > destination.txt
            ```
            
            - Overwrites destination.txt with the content of source.txt.
            
            ---
            
            ### **✅ 3.**
            
            ### **Using cat with >> (append)**
            
            If you want to **append** the contents instead:
            
            ```
            cat source.txt >> destination.txt
            ```
            
            - Adds the content of source.txt **to the end** of destination.txt.
            
            ---
            
            ### **📝 Example**
            
            Let’s say you have:
            
            ```
            echo "Hello" > file1.txt
            echo "World" > file2.txt
            ```
            
            Now:
            
            ```
            cat file1.txt >> file2.txt
            cat file2.txt
            ```
            
            Output will be:
            
            ```
            World
            Hello
            ```
            
            ---
            
        
        **File:**
        
        ```bash
        cp source.txt dest.txt     # Copy file
        cp -i source.txt dest.txt # Confirm before overwrite
        
        ```
        
        **Directory:**
        
        ```bash
        cp -r sourcedir destdir    # Copy directory recursively
        cp -v file.txt dir/       # Verbose output while copying
        
        ```
        
    - Move
        
        ### 4. Move/Rename
        
        **File/Directory:**
        
        ```bash
        mv oldname.txt newname.txt # Rename file
        mv file.txt dir/          # Move file to directory
        mv -i file.txt dir/       # Confirm before overwrite
        mv dir1/ dir2/            # Move/rename directory
        
        ```
        
    - Additional Note
        
        ### Additional Useful Flags:
        
        - `v` : Verbose (show what's happening)
        - `f` : Force (override warnings)
        - `i` : Interactive (ask before overwriting)
        - `n` : No-clobber (prevent overwriting)
        - `u` : Update (only overwrite if source is newer)
- Shell Scripting
    
    ## 1. Basic Script Structure
    
    ```bash
    #!/bin/bash
    # This is a comment
    echo "Hello World"
    
    ```
    
    ## 2. Variables
    
    ```bash
    name="John"          # String variable
    age=25               # Integer variable
    PI=3.14              # Float (treated as string)
    echo "Name: $name"   # Variable expansion
    
    ```
    
    ## 3. Input/Output
    
    ```bash
    read -p "Enter your name: " username   # Prompt input
    echo "Hello, $username"               # Output
    echo -e "Line1\\nLine2"                # Enable escape chars
    printf "Formatted: %s, %d\\n" $name $age  # Formatted output
    
    ```
    
    ## 4. Arithmetic Operations
    
    ```bash
    a=5; b=3
    sum=$((a + b))       # Addition
    sub=$((a - b))       # Subtraction
    mul=$((a * b))       # Multiplication
    div=$((a / b))       # Division (integer)
    mod=$((a % b))       # Modulus
    
    ```
    
    ## 5. Conditional Statements
    
    ### If-Else
    
    ```bash
    if [ $age -ge 18 ]; then
        echo "Adult"
    elif [ $age -ge 13 ]; then
        echo "Teenager"
    else
        echo "Child"
    fi
    
    ```
    
    ### Case Statement
    
    ```bash
    case $day in
        "Mon") echo "Monday";;
        "Tue") echo "Tuesday";;
        *) echo "Other day";;
    esac
    
    ```
    
    ## 6. Loops
    
    ### For Loop
    
    ```bash
    for i in {1..5}; do
        echo "Number: $i"
    done
    
    for file in *.txt; do
        echo "Processing $file"
    done
    
    ```
    
    ### While Loop
    
    ```bash
    count=1
    while [ $count -le 5 ]; do
        echo "Count: $count"
        ((count++))
    done
    
    ```
    
    ### Until Loop
    
    ```bash
    count=1
    until [ $count -gt 5 ]; do
        echo "Count: $count"
        ((count++))
    done
    
    ```
    
    ## 7. Arrays
    
    ```bash
    fruits=("Apple" "Banana" "Cherry")
    echo ${fruits[0]}       # Apple
    echo ${fruits[@]}       # All elements
    echo ${#fruits[@]}      # Number of elements
    
    ```
    
    ## 8. Functions
    
    ```bash
    greet() {
        local name=$1       # Local variable
        echo "Hello, $name"
        return 0
    }
    greet "Alice"
    
    ```
    
    ## 9. String Operations
    
    ```bash
    str="Hello World"
    echo ${#str}            # Length: 11
    echo ${str:6:5}         # Substring: World
    echo ${str//Hello/Hi}   # Replacement: Hi World
    
    ```
    
    ## 10. File Operations
    
    ```bash
    if [ -f "file.txt" ]; then
        echo "File exists"
    fi
    
    if [ -d "directory" ]; then
        echo "Directory exists"
    fi
    
    # Read file line by line
    while IFS= read -r line; do
        echo "$line"
    done < "file.txt"
    
    ```
    
    ## 11. Advanced Features
    
    ### Command Line Arguments
    
    ```bash
    echo "Script name: $0"
    echo "First arg: $1"
    echo "All args: $@"
    echo "Arg count: $#"
    
    ```
    
    ### Exit Codes
    
    ```bash
    command_that_might_fail || echo "Command failed"
    if [ $? -ne 0 ]; then
        echo "Error occurred"
    fi
    
    ```
    
    ### Process Substitution
    
    ```bash
    diff <(ls dir1) <(ls dir2)
    
    ```
    
    ### Here Documents
    
    ```bash
    cat <<EOF
    This is a multi-line
    text block
    EOF
    
    ```
    
    ### Debugging
    
    ```bash
    set -x      # Enable debugging
    # Your code
    set +x      # Disable debugging
    
    ```
    
    ## 12. Regular Expressions
    
    ```bash
    if [[ "abc123" =~ ^[a-z]+[0-9]+$ ]]; then
        echo "Matches pattern"
    fi
    
    ```
    
    ## 13. Advanced I/O Redirection
    
    ```bash
    command > file.txt      # Overwrite output to file
    command >> file.txt     # Append output to file
    command 2> error.log   # Redirect stderr
    command &> all.log     # Redirect
    ```
    
- Interview
    
    ---
    
    ### **Deadlock**
    
    - A **deadlock** occurs when two or more processes are **waiting for each other** to release a resource, but **none ever do**.
    - They get stuck **forever**—each one is holding one resource and waiting for another.
    
    ### **🧠 Real-life Example:**
    
    Two people are trying to write with each other’s pens. Each holds one pen and waits for the other to give theirs back. Nobody writes.
    
    ---
    
    ### **🔐 2.**
    
    ### **Mutex (Mutual Exclusion Lock)**
    
    - A **mutex** is a **lock mechanism** used to ensure **only one thread** can access a **shared resource or critical section** at a time.
    - Think of it like a **key**: if one thread has the key (lock), others must wait.
    
    ### **🔁 Operations:**
    
    - lock() — acquire the mutex (wait if already locked)
    - unlock() — release the mutex
    
    ---
    
    ### **🚫 3.**
    
    ### **Mutual Exclusion**
    
    - **Mutual exclusion** is a **principle** that ensures **only one process or thread** can access a shared resource **at a time**.
    - A **mutex lock** is one way to **implement** mutual exclusion.
    
    ---
    
    ### **🧩 4.**
    
    ### **Critical Section**
    
    - A **critical section** is a **code block** that accesses **shared resources** (like variables, files, memory).
    - Only **one thread/process** should enter a critical section **at a time** to avoid **race conditions** or inconsistent data.
    
    ---
    
    ### **🎚️ 5.**
    
    ### **Semaphore**
    
    - A **semaphore** is a **signaling mechanism** to control access to resources.
    - Can allow **more than one** process/thread to access a resource, depending on the **counter value**.
    
    ### **Types:**
    
    - **Binary Semaphore**: Like a mutex (0 or 1)
    - **Counting Semaphore**: Allows access to **N** processes
    
    ### **🔁 Common operations:**
    
    - wait() or P: Decrement the semaphore. If it’s less than 0, block.
    - signal() or V: Increment the semaphore. If processes are waiting, wake one.
    
    ### **6.🧠 What is a Race Condition?**
    
    A **race condition** occurs when **two or more threads (or processes) access shared resources (like variables, files, or memory) at the same time**, and **the final outcome depends on the timing or order** of their execution.
    
    It leads to **unpredictable, incorrect, or inconsistent results**.
    
    ---
    
    ### **🔄 Summary Table**
    
    | **Term** | **What It Is** | **Key Role** |
    | --- | --- | --- |
    | **Deadlock** | Processes block each other indefinitely | Caused by circular waiting on resources |
    | **Mutex** | Lock object (binary) | Enforces mutual exclusion |
    | **Mutual Excl.** | Principle/concept | Only one process accesses resource |
    | **Critical Section** | Code accessing shared resources | Needs to be protected by locks |
    | **Semaphore** | Counter + signaling mechanism | Controls access (binary or counting) |
    | Race condition | two thread shared Resources |  |
    
    ---
