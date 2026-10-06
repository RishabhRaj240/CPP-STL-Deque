C++ Deque STL – Basics
A beginner-friendly C++ program demonstrating the fundamental operations of the deque container from the C++ Standard Template Library (STL).
📌 Overview
std::deque (Double-Ended Queue) is an STL container that allows efficient insertion and deletion of elements from both the front and back.
This program demonstrates:
- Creating a deque
- Adding elements using push_back()
- Adding elements using emplace_back()
- Adding elements using push_front()
- Adding elements using emplace_front()
- Removing elements using pop_back()
- Removing elements using pop_front()
- Accessing the first and last elements
✨ Features
- Demonstrates basic std::deque operations.
- Supports insertion at both ends.
- Supports deletion from both ends.
- Demonstrates front() and back().
- Introduces commonly used STL container functions.
🛠️ Technologies Used
Technology	Purpose
C++	Programming language
STL	Standard Template Library
deque	Double-ended queue container
iostream	Console output


📝 Example Operations
The program starts with an empty deque:
{}

Add Elements at the Back
dq.push_back(1);
dq.emplace_back(2);

Result:
{1, 2}

Add Elements at the Front
dq.push_front(4);
dq.emplace_front(3);

Result:
{3, 4, 1, 2}

Remove Elements
dq.pop_back();

Result:
{3, 4, 1}

Then:
dq.pop_front();

Result:
{4, 1}

🔍 Accessing Elements
The first element can be accessed using:
dq.front();

The last element can be accessed using:
dq.back();

For the final deque {4, 1}, the output is:
1
4

💻 Source Code
#include <iostream>
#include <deque>
using namespace std;

void explainDeque() {

    deque<int> dq;

    dq.push_back(1);       // {1}
    dq.emplace_back(2);    // {1, 2}

    dq.push_front(4);      // {4, 1, 2}
    dq.emplace_front(3);   // {3, 4, 1, 2}

    dq.pop_back();         // {3, 4, 1}
    dq.pop_front();        // {4, 1}

    const int backValue = dq.back();

    cout << backValue << '\n';
    cout << dq.front() << '\n';

    // Other commonly used functions:
    // begin, end, rbegin, rend,
    // clear, insert, size, swap
}

int main() {
    explainDeque();

    return 0;
}

📤 Example Output
1
4

▶️ How to Run
1. Compile the program
g++ main.cpp -o main

2. Run the executable
./main

Windows: Run main.exe instead.

📚 Learning Outcomes
This project helps beginners understand:
- STL deque
- Double-ended queues
- push_back()
- emplace_back()
- push_front()
- emplace_front()
- pop_back()
- pop_front()
- front() and back()
- Basic STL container operations
🔄 Common Deque Operations
Operation	Purpose
push_back()	Adds an element to the back
emplace_back()	Constructs an element at the back
push_front()	Adds an element to the front
emplace_front()	Constructs an element at the front
pop_back()	Removes the last element
pop_front()	Removes the first element
front()	Returns the first element
back()	Returns the last element
size()	Returns the number of elements
clear()	Removes all elements
insert()	Inserts elements at a position
swap()	Exchanges contents of two deques


⏱️ Complexity
Operation	Typical Complexity
push_back()	O(1)
emplace_back()	O(1)
push_front()	O(1)
emplace_front()	O(1)
pop_back()	O(1)
pop_front()	O(1)
front()	O(1)
back()	O(1)
size()	O(1)


A deque is useful when efficient insertion and deletion are required at both ends of a sequence.
📸 Screenshot
Add your program output screenshot to:
screenshots/output.png

Then include it in the README:
![Program Output](screenshots/output.png)

Recommended project structure:
CPP-Deque-STL/
│
├── main.cpp
├── README.md
└── screenshots/
    └── output.png

👤 Author
Rishab Raj Chourasia
C++ | Data Structures & Algorithms | Problem Solving
