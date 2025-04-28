# cs540-homework-3--hill-climbing-solved
**TO GET THIS SOLUTION VISIT:** [CS540 Homework 3- Hill Climbing Solved](https://www.ankitcodinghub.com/product/cs540-hw3-hill-climbing-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;117932&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS540  Homework 3- Hill Climbing Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
Program Goals

Deepen understanding of state space generation Practice implementation of search algorithms

Summary

We’ve introduced the 8-queens problem in class: place 8 queens on a chessboard such that no queen is attacking any other queen.

A solution for an 8×8 board with state [2, 7, 3, 6, 0, 5, 1, 4]

Recall that in the game of chess, queens attack any piece they can “see” (i.e., there is nothing between the queen and the attacking piece) in the same row, column, or diagonal.

In this assignment, you will generalize this problem to a board of arbitrary (square) size and the equivalent number of queens and add a “static point” to the board. It means that at any time, there must be a queen on the static point. You only have to place the other N-1 queens on the board.

Given the size of the board (N &gt; 0) and location of the static point (0 &lt;= static_x &lt; N and 0 &lt;= static_y &lt; N), you will implement a hill-climbing algorithm to solve the problem.

Program Specification

The code for this program must be written in Python in a file called nqueens.py. You should only submit one file with the name nqueens.py, and make sure it includes all functions needed. Do not submit a Jupyter notebook .ipynb file.

Your state representation must be a list of N integers, 0-indexed, representing the row the queen is occupying in each column (see figure above). For simplicity of representation, we will retain our assumption that there is a single queen per column. When you generate the successor states, there should not be any states with two queens in the same column.

Goal State

There are multiple possible configurations for a goal state, defined as a state in which no queen is attacking any other queen per the rules above. One of your tasks will be to define an evaluation function for the states such that the goal state has the lowest value (0) when the function is applied to it.

Functions

For this program you should write 5 Python functions:

1. succ(state, static_x, static_y) — given a state of the board, return a list of all valid successor states

2. f(state) — given a state of the board, return an integer score such that the goal state scores 0

3. choose_next(curr, static_x, static_y) — given the current state, use succ() to generate the successors and return the selected next state

4. n_queens(initial_state, static_x, static_y) — run the hill-climbing algorithm from a given initial state, return the convergence state

5. n_queens_restart(n, k, static_x, static_y) — run the hill-climbing algorithm on an n*n board with random restarts

Generate Successors

This function should return a list of lists, containing all valid successor states of the given current state. For the purposes of this program, a successor of a current state is any valid state that differs from the current state by ONE queen’s location, which means you could only move one queen by one tile.

We WILL allow multiple queens to occupy the same row or the same diagonal line, but not the same column, as it could not be described by the representation of the state.

We WILL NOT allow moving the queen on the static point.

If there is not a queen on the static point in the input state, return an empty list

The returned states should be sorted by the ascending order

For sorting the states, using sorted() method will be sufficient to get the expected ascending order.

Evaluate a State

As in class, we’ll define our f() to be the number of queens that are being attacked. Even if a queen is attacked by multiple other queens, it will only be counted once.

Given n=3, here are some example f() values:

Select Next State

Given a current state and the location of the static point, use the previous two functions to select the next state to evaluate per the following rules:

If one of the possible states (including the current state) has a uniquely low score, select that state Otherwise, sort the states in ascending order (as though they were integers) and select the “lowest” state

N-Queens

Run the hill-climbing algorithm as specified in class on a given initial state until convergence, that is, until your algorithm finds a local minimum and gets stuck (or solves the problem). Here, we define that a local minimum means that you encountered two states with the same f value in the consecutive two steps. You should use choose_next() to choose the next state from the current state, which means the next state could be the same with your current state and your function should return in this situation.

Your printed output for this function should look like the black text below, followed by the returned minimum state in green:

Each step of the hill-climbing function should print its current state along with that state’s f() value, and ultimately return the best state you find.

N-Queens with Random Restarts

Generate a random (valid!) initial state for your n*n board, and use your n_queens() function on that state. If the converged state does not solve the problem with an f() value of 0, generate a new random (valid!) initial state and try again. Try again up to k times.

If you find an optimal solution before you reach k restarts, print the solution and terminate.

If you reach k before finding an optimal solution with a score of 0, print the best solution(s) in sorted order.

Python’s random module will be helpful in generating random initial states. Each column’s coordinate should be uniformly distributed over the possible coordinates, except for the column with the static point.

To generate a single uniform integer between 0 (inclusive) and n (inclusive), the Python code is:

Be sure to account for the static point! Set the random_seed to 1 before using randint to make sure that the result of your program is reproducible, like the example below:

Remember that you just need to set the seed once at the beginning of your function, or you will always get the same number.

Test &amp; Grading

We provide a unit test module which includes all examples mentioned above to help you test your program and make sure that your program is compatible with the grading script. Remember that we will use more test cases when grading, and you are encouraged to add your own test cases to test your program.

To use the test script, first upload your nqueens.py to a CSL machine. In your working directory, run the commands below:

You could also directly click the link to download it. The test is also written in Python, so feel free to open it by a text editor and modify it. If you passed all tests you will see an OK message. The unit test module could only be executed under python3 environment, and we assume that your program should be compatible with python3.

We do not have a strict limit on the running time, but please make sure that your program could finish in a reasonable period of time. In normal cases, your program could finish running all test cases above in less than 0.1s, and finish running n_queens_restart(8, 1000, 0, 0) in less than 1s.

Some Rubric (1)

Criteria Ratings Pts

Test Cases

Full

Passed

all test

cases 0.0 pts

No

Passed

no test cases 80.0 pts

Valid Submission

Your submission should be a valid submission that is compatible with our test script, i.e. a file named nqueens.py with five functions mentioned above 20.0 pts

Full

No
