# Queue-Implementation-Using-Array-in-CPP  

## Aim  
To study and implement **Queue implementation using array** in C++.  

## Software Required  
- Visual Studio  

---

## Theory  

A **queue** is a linear data structure that stores elements sequentially, where insertion takes place at one end (**rear**) and deletion at the other end (**front**). It follows the **FIFO (First In, First Out)** principle, meaning the element inserted first will be removed first.  

### Properties of a Queue  
- Works on **FIFO principle**.  
- Requires two pointers:  
  - **Front** → for deletion.  
  - **Rear** → for insertion.  
- Provides **sequential one-way access** to elements. Even if implemented using arrays, elements can only be accessed in order via `front` and `rear`, not directly using indices.  

### Applications of Queue  
Due to its FIFO nature, queues are widely used in real-world and computational systems:  

- **Operating Systems**  
  - Job Scheduling Algorithms.  
  - Memory Management for concurrent processing.  

- **Algorithms**  
  - Storing addresses of tree nodes.  
  - Graph traversal (e.g., **Breadth-First Search**).  

- **Real World Applications**  
  - Music or video player "Add to Queue" option (enqueue operation).  
  - Printer job scheduling.  
  - Customer service ticketing systems.  

---

## Implementation  

This concept is demonstrated using a **single C++ code** that shows queue operations:  
- **Enqueue (insertion)**  
- **Dequeue (deletion)**  
- **Display (traversal)**  

---

## Algorithm  

**Algorithm: Implement Queue using Array**  

1. **Start**  
2. Define a class `Queue` with:  
   - An integer array `arr[SIZE]`.  
   - Two integer variables `front` and `rear` initialized to `-1`.  
   - Functions: `enqueue()`, `dequeue()`, and `display()`.  

3. **Enqueue operation (`enqueue(value)`)**  
   - If `rear == SIZE - 1`, display **"Queue Overflow!"** and return.  
   - If `front == -1`, set `front = 0`.  
   - Increment `rear` and insert the value into `arr[rear]`.  
   - Display confirmation message.  

4. **Dequeue operation (`dequeue()`)**  
   - If `front == -1` OR `front > rear`, display **"Queue Underflow!"** and return.  
   - Display the element `arr[front]` being removed.  
   - Increment `front`.  

5. **Display operation (`display()`)**  
   - If `front == -1` OR `front > rear`, display **"Queue is empty"**.  
   - Otherwise, print all elements from `arr[front]` to `arr[rear]`.  

6. **In `main()`**  
   - Create an object `q` of class `Queue`.  
   - Perform enqueue, dequeue, and display operations to test queue behavior.  

7. **End**  

---

## Conclusion  

The above program demonstrates **queue implementation using arrays in C++**.  
It clearly shows how **enqueue, dequeue, and display operations** work while handling **overflow and underflow conditions**.  

This foundational implementation is essential for understanding real-world applications of queues, ranging from **system scheduling** to **graph traversal** in algorithms.  
