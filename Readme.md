
Robotic Manipulation
Kashish Goyal
Final Assignment
1. File Info
Root Folder
HW9.nb: The file is the Mathematica code for the assignment – 13.33(c) as well
HW9.pdf: PDF of the Mathematica code. 
Part D Folder
FeetForward – Contains files for feet forward control
Optimal Result – Contains files for final output corresponding to optimal Kp = 15 and Ki = 40 
Part E Folder
Each of the file names is of the format “kp<>_ki<>” where the values for are mentioned in the file name. Videos are named in the same manner.

2. Part E Explanation 

When Ki is zero and kp is non zero:
As can be seen from the files corresponding to kp=10 and ki=0; the error plot has no overshoot whatsoever. This is in line with the fact that the overshoot is introduced only by the integral term in the control law.
When Ki is extremely high:
Looking at the file with kp = 5 and ki = 150, the error plot overshoots several times and the 2% settling time increases. This again is in line with the fact that high values of Ki render the system unstable. 
High kp:
Looking at the files corresponding to kp = 30, and ki = 50, we see that the settling time decreases rapidly and the amplitude of overshoot has decreased. This is not favourable because high values of proportional gain lead to extremely high acceleration during the beginning which may lead to hardware failure in the robot.
3. Remarks
For relatively similar values for kp and ki, unexpected peaks in error occurred towards the end of the simulation. Adding the “NearZero” function from the library to check the division by zero, didn’t help either. However this error was negligible for other values of kp and ki. The results submitted in the assignment were calculated at these values. The probable cause of the error is the integration method. More detailed research is needed to find the actual reason.
