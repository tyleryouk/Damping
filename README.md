INSTRUCTIONS 
Complete the exercises below and upload them as a single MATLAB script file using the naming convention “ENGR131_21F_Lab##_abc123.m”, replacing abc123 with your Case ID, and ## with the lab number. 
a. For example, if Dr. Williams were submitting Lab 2 it would be ENGR131_21F_Lab02_mrw8.m 
 
For your script, please perform the following: 
1.	Separate each question into separate, runnable sections using the “%%” comment notation. 
2.	You may use the code and notes from class and MATLAB’s documentation to solve these problems  
3.	Use comments as appropriate to indicate your thoughts and how your code works (or is supposed to work).  This is 5 points (10%) of your grade. 
 
 
QUESTION 
 
1. The spring-mass-damper system shown in fig. 1a, will behave over time as shown in fig. 1b when released from a particular height above its rest point as governed by the equation in eq. 1.   
 
 
 
	𝐻𝐻 = 𝑒𝑒−𝛾𝛾𝛾𝛾a cos(𝜔𝜔𝜔𝜔)  	 	(eq. 1) 
 
 
Where H is the height above rest, γ is the damping coefficient, a is the starting height before release, ω is the frequency of oscillation, and t is the time from release.   
 
Objective: 
Recreate the figure shown in 1b using the information below and a damping coefficient (γ) input by the user.  Check that the input from the user is positive and if not, run the function in the p-file to alert the user they entered an incorrect value. 
•	The damping coefficient will be variable input by the user 
•	t will be a vector of values from 0 to 5 
•	a = 1 
•	ω = 8. 
 
Required Files/Materials: 
•	ENGR131_21S_031_02.m 
•	ENGR131_21S_032_02.mat 
 
Recreate the plot in fig. 1b by following the steps below (45 pts): 
a)	Load the data (.mat) file into Matlab.  Do this in your script (NOT manually, 5 pts) 
b)	Create a function called CalcPosition at the bottom of your script.  This function should return the output argument Height and receive the input arguments Time and Damping.  The values of a and ω should be set as variables and can be assigned within this function.  Compute Height based on eq. 1 (5 pts). 
c)	Prompt the user to enter a damping coefficient.  To check your work and recreate the plot in Fig. 1, enter a value of 1 (2 pts) 
d)	Respond to the user input and repeat the value they entered back to them to two decimal places (2 pts) 
e)	Use a selection statement to determine if the value entered is greater than zero.  If it is, do the following (5 pts): 
i) Create a Time vector that ranges from 0 to 5 and contains 75 evenly spaced values (2 pts) ii) Compute the Height of the system by calling your CalcPosition function and passing the Time and Damping arguments to it (5 pts). 
iii) Find the minimum height of the system and it’s index (2 pts) iv) Plot the Height of the system over time using a red line with triangle markers (2 pts) v) Plot the minimum height on the graph using a blue circle (5 pts) vi) Add appropriate labels and a title (3 pts) vii) Set the Height limits of the plot to -1 to 1 (2 pts) 
f) If the value entered by the user is zero or less, call the function ENGR131_21S_031_02 (located in the .m file you downloaded), passing the input arguments Warning and Fs (loaded into Matlab when you loaded the .mat file) to it. (5 pts). 
 
 
 
Hints: 
•	Don’t get hung up on the symbol font.  You are welcome to use Damping, DC, Gamma, or similar variable name for γ.  Likewise, w serves as a good stand in for ω. 
•	When passing more than one argument to a function, be sure to keep them in the right order. 
•	You formula will contain some scalar multiplication and some vector multiplication.  These use different (though very similar looking) operators. 
•	Recall that when setting axis limits, it is expecting 4 inputs. 
•	Use the index values you find from one vector as the index for another. 
•	Consider using the hold on/hold off toggle so you can plot two different series on the same plot without over-plotting the first one. 
•	Keep in mind that user-defined functions can be written at the bottom of your script or as a separate file.  
Regardless of where they are located, they called using the same syntax. 
•	Be sure you have your sound on when you run your script. 
 
 
 
 
 
Revision 		Description 	Date 
 A 	 Original Document 		9/2/2021  
  	  		  
