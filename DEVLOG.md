Entry #1: 
    Issue: Did not fully understand how the directions ere 
    Error message or symptoms: No error message
    Attempts made: I attempted to look at other dfs maze like codes online for how typical mazes were made. As well, I wrote down and tracked what the values of each itteration would look like if the code had run and how that would determine looking at each direction.
    Final resolution: I realized that dr -1 dc 0 represents up, dr 0 dc 1 is right, dr 1 dc 0 is donw, and dr 0 dc -1 represents left.

Entry #2: 
    Issue: I didn't understand conceptually the base cases needed that needed to be checked for a DFS when mapping through a maze
    Error message or symptoms: No error message
    Attempts made: I tried drawing out a simple maze and trying to map out some of the issues I would have had for trying to find the exit
    Final resolution: I found that the only situations where I would need to start backtracking or create base cases is when I reach out of bounds of the maze, hit a wall, or if I go to somewhere that I have previously visited.

Entry #3: 
    Issue: Trying to figure how I would use the provided code of determinning what numebrs meant what directions meant and to use it to traverse the maze
    Error message or symptoms: No error message
    Attempts made: I tried drawing a maze out, picking a spot that I would have landed on and then referencing to see how I could add the values used to determine the new row and column that it woudl go through.
    Final resolution: I determined that for each loop, I could use the given code of using a for loop to add dr and dc with my current position in the maze. With each loop, it would look check a direction and then would use recursion to call back to keep going until it either reached the exit or found a dead end.

Entry #4: 
    Issue: Trying to decide how to use recursion to perform dfs throughout the maze.
    Error message or symptoms: No error message
    Attempts made: I knew that dfs was popularily implemented through the use of recursion and that I already had a for loop that would check for each direction of what row and column I would of had. I looked at how dfs was implemented online in how recursion may have been impelemented for standard dfs. As well I noted that this may be heavily related to the base case of filling out visited parts of the maze.
    Final resolution: I determined that I would utilize the parameters used in the dfs function using the parent row and column vectors to store the current row and column that we are at in the maze so that we can then call dfs again to then again check for exit, base cases, and all four directions of where we are at now. This keeps running until a base case is fulfilled where we either backtrack or we find the exit.

Entry #5: 
    Issue: When running my dfs function, I got an out of bounds error
    Error message or symptoms: zsh: segmentation fault ./main
    Attempts made: I tried looking back in my dfs code and trying to figure out what might cause an out of bounced erorr when searching for the base case. I tried adding different if statements throughout by code to ensure that I was within the bounds of the maze when traversing.
    Final resolution: I added a conditional statement before storing the new row and column that we were going to go into where it would check if the new row and column that we were going to was actually wihin the bounds of the row and columns of the maze

Entry #6: 
    Issue: When ruunning my code, I did not see anything being outputted  after entering the dimensions I wanted for the maze. 
    Error message or symptoms: No maze being outputted
    Attempts made: I tried checking how the maze was actually generated. Since there wasn't actual code there I was supposed to edit I didn't touch it. I then checked for other conventions in C++ that could be used to output my maze since I couldn't edit printMaze()
    Final resolution:  I saw that I could use g++ with std=c++17 and compile them together in the terminal to output the maze display correctly