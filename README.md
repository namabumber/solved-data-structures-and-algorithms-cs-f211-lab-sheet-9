Download Link: https://assignmentchef.com/product/solved-data-structures-and-algorithms-cs-f211-lab-sheet-9
<br>
<ol>

 <li>Consider an operating system where each process can only run up to a certain amount of time (say threshold = 4 secs). Then we switch to some other process. In this way, we iterate over all the active processes. In case there is only one active process, it can continuously execute (without considering the threshold). Now, given arrival times, execution times and the threshold, calculate the average waiting time.</li>

</ol>




<h2>Example-</h2>

P1 arrives at 0 and executes for 3 secs, P2 arrives at 0 and executes for 4 secs, and P3 arrives at 0 and executes for 5 secs. Threshold = 1sec.

Then the order of process execution is P1 from 0 to 1.

P2 from 1 to 2.

P3 from 2 to 3.

P1 from 3 to 4.

P2 from 4 to 5.

P3 from 5 to 6.

P1 from 6 to 7.

P2 from 7 to 8.

P3 from 8 to 9.

P2 from 9 to 10.

P3 from 10 to 11.

P3 from 11 to 12.

Waiting times-

P1 – 4 secs

P2 – 6 secs

P3 – 7 secs

Average waiting time = 5.66 secs.




<ol start="2">

 <li>Alexa has two stacks of non-negative integers, stack <strong>A</strong> and stack <strong>B</strong> where index denotes the top of the stack. Alexa challenges Nick to play the following game:</li>

</ol>

<strong> </strong>

<ol>

 <li>In each move, Nick can remove one integer from the top of either stack <strong>A</strong> or stack <strong>B</strong>.</li>

 <li>Nick keeps a running sum of the integers he removes from the two stacks. Nick is disqualified from the game if, at any point, his running sum becomes greater than some integer <strong>x</strong> given at the beginning of the game. <strong>iv.</strong> Nick’s final score is the total number of integers he has removed from the two stacks.</li>

</ol>




Given <strong>A</strong>, <strong>B</strong> and <strong>x</strong>, find the maximum possible score Nick can achieve (i.e., the maximum number of integers he can remove without being disqualified).

<strong> </strong>

<h2>Input –</h2>

The first line contains three space-separated integers describing the respective values of <strong>n</strong> (the number of integers in stack <strong>A</strong>), <strong>m</strong> (the number of integers in stack <strong>B</strong>), and <strong>x</strong> (the number that the sum of the integers removed from the two stacks cannot exceed).

The second line contains <strong>n</strong> space-separated integers describing the respective values of <strong>A</strong>. The third line contains <strong>m</strong> space-separated integers describing the respective values of <strong>B</strong>.

<strong> </strong>

<h2>Output</h2>

Print an integer on a new line denoting the maximum possible score Nick can achieve without being disqualified.

<strong> </strong>

<h1><a name="_Toc6640"></a>Example-</h1>

<strong>Input- </strong>5 4 10

4 2 4 6 1 (<strong>Note the left most element represents the top of the stack.</strong>) 2 1 8 5 (<strong>Note the left most element represents the top of the stack.</strong>)




<h2>Output- 4</h2>




<ol start="3">

 <li>You are given <strong>q</strong> queries. Each query consists of a single number <strong>N</strong>. You can perform any one of the given operations in each move:</li>

</ol>




<ol>

 <li>If we take 2 integers <strong>a</strong> and <strong>b</strong> where <strong>N</strong> = <strong>a</strong>*<strong>b</strong> then we can change <strong>N</strong> = <strong><em>max</em></strong>(<strong>a</strong>, <strong>b</strong>).</li>

 <li>Decrease the value of <strong>N</strong> by 1.</li>

</ol>




Determine the minimum number of moves required to reduce the value of <strong>N</strong> to 0.

<strong> </strong>

<h2>Input</h2>

The first line contains the integer <strong>q</strong>.

The next <strong>q</strong> lines each contain an integer <strong>N</strong>.




<strong>Output- </strong>

Output <strong>q</strong> lines, each line containing the minimum number of moves required to reduce the value of <strong>N</strong> to 0.

<strong> </strong>

<h2>Example – Input – 2</h2>

3

4




<h2>Output – 3</h2>

3




<ol start="4">

 <li>Suppose there is a circle. There are <strong>N</strong> petrol pumps on that circle. Petrol pumps are numbered <strong>0</strong> to <strong>N-1</strong>. You have two pieces of information corresponding to each of the petrol pumps: <strong>(i)</strong> the amount of petrol that a particular petrol pump will give, and <strong>(ii)</strong> the distance from that petrol pump to the next petrol pump. Initially, you have a tank of infinite capacity carrying no petrol. You can start the tour at any of the petrol pumps. Calculate the first point from where the truck will be able to complete the circle. Consider that the truck will stop at each of the petrol pumps. The truck will move one kilometre for each litre of the petrol.</li>

</ol>

<strong> </strong>

<h2>Input –</h2>

The first line will contain the value of <strong>N</strong>.

The next <strong>N</strong> lines will contain a pair of integers each, i.e. the amount of petrol that petrol pump will give and the distance between that petrol pump and the next petrol pump.

<strong> </strong>

<strong>Output- </strong>

An integer which will be the smallest index of the petrol pump from which we can start the tour.

<strong> </strong>

<a href="#_Toc6640"><strong>Example –  Input- </strong>10                                                                                                                                         3 </a>

<a href="#_Toc6641">3<strong>Output- </strong>                                                                                                                                                           4 </a>




3

1 5

<h2>1</h2>




<ol start="5">

 <li>Rahul can’t stand when two same things are placed adjacent to each other. He now has a string and wants that every adjacent pair of characters are different. Before going to begin the task he needs to know if it is at all possible with a given string by exchanging the characters of the string. Help Rahul with this task</li>

</ol>




<strong>Sample Input 1 –  </strong>bbbbb




<strong>Sample Output 1 – </strong>Not Possible




<strong>Sample Input 2 – </strong>aabababbb




<h2>Sample Output 2 – Possible</h2>




<ol start="6">

 <li>Given a matrix city, each square <strong>grid</strong>[<strong>i</strong>][<strong>j</strong>] represents the height of the building at that point (<strong>i</strong>, <strong>j</strong>). Assume that you can swim from one building terrace if they are at same level.</li>

</ol>




Now rain starts to fall. At time <strong>t</strong>, the depth of the water everywhere is <strong>t</strong>. You can swim from a square to another 4-directionally adjacent square (no diagonal moves) if and only if the elevations of both squares individually are at most <strong>t</strong>. You can swim infinite distance in zero time. Of course, you must stay within the boundaries of the grid during your swim.




You start at the top left building (0, 0). What is the least time in which you can reach the bottom right building (<strong>N</strong> – 1, <strong>N</strong> – 1)?




<h2>Sample Input</h2>

2

<ul>

 <li>2</li>

 <li>3</li>

</ul>




<h2>Sample Output</h2>

3




<strong>Explanation: </strong>

At time 0, you are in grid location (0, 0).

You cannot go anywhere else because 4-directionally adjacent neighbours have a higher elevation at <strong>t</strong> = 0. You wait for one second when water level is <strong>t</strong> = 1. Go to (1, 0). Wait for 2 more seconds and go to (1, 1).







<ol start="7">

 <li>Sam is going on a world tour. He hires you as his travel agent. He wants you to go to <strong>t</strong> cities, he will provide you the source and destination. He also states that he will willing to go via at maximum <strong>k</strong> cities between his source and destination. Find the cheapest possible flight combination.</li>

</ol>




(Hint – solve this problem using heaps)




<h2>Sample Input Format</h2>

<strong>N</strong> cities <strong>M</strong> flight routes

Next <strong>M</strong> lines would be source, destination, flight price <strong>t </strong>– No. of cities he wants to visit

Next <strong>t</strong> lines would be source, destination, <strong>k</strong>




<h2>Sample Input</h2>

3 3

0 1 100

<ul>

 <li>2 500</li>

 <li>2 100</li>

</ul>

2

0 2 0

0 2 1




<h1><a name="_Toc6641"></a>Sample Output</h1>

500

200




<ol start="8">

 <li>Suppose ShareChat will start its IPO soon. In order to sell a good price of its shares to Venture Capital, ShareChat would like to work on some projects to increase its capital before the IPO. Since it has limited resources, it can only finish at most <strong>k</strong> distinct projects before the IPO. Help ShareChat design the best way to maximize its total capital after finishing at most <strong>k</strong> distinct projects.</li>

</ol>




You are given several projects. For each project <strong>i</strong>, it has a pure profit <strong>P<sub>i</sub></strong> and a minimum capital of <strong>C<sub>i</sub></strong> is needed to start the corresponding project. Initially, you have <strong>W</strong> capital. When you finish a project, you will obtain its pure profit and the profit will be added to your total capital.




To sum up, pick a list of at most <strong>k</strong> distinct projects from given projects to maximize your final capital, and output your final maximized capital.







<h2>Sample Input format</h2>

<strong>K </strong>

<strong>W </strong>– current capital

<strong>N </strong>– number of projects

Profit array

Capital array




<h2>Sample Input</h2>

2

0

3

1 2 3

0 1 1




<h2>Sample Output</h2>

4

****************************