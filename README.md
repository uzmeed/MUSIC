# DoA Estimation using optimized MUSIC Algorithm
This repository includes the code in Xilinx System Generator / Vivado 2016.3 as used for the paper:

Uzma M. Butt, Shoab A. Khan, Anees Ullah, Abdul Khaliq, Pedro Reviriego, Ali Zahir "Towards Low Latency and Resource-Efficient FPGAImplementations of the MUSIC Algorithm forDirection of Arrival Estimation", under submission to IEEE Transactions on Circuit and Systems I.

# Dependencies
Matlab 2016
Vivado 2016.3

# Content
*src* directory includes the following files:
- MUSIC_repo_DA_I.slx (implementation of Design Approach I)
- MUSIC_rep_DA_I.tcl (vivado project for Design Approach I)
- MUSIC_repo_DA_II.slx (implementation of Design Approach II)
- MUSIC_rep_DA_II.tcl (vivado project for Design Approach I__)
- ROM_Data_gen_MUSIC_repo.m (Generates the data to be stored in ROM)


# Execution of the code
-	Run the ROM_Data_gen_music_repo.m. It will generate the ROM data for .slx program
-	Open MUSIC_repo_DA_I.slx / MUSIC_repo_DA_II.slx
-	Run the program 
-	Plot the Final_Angle_DA_I / Final_Angle_DA_II.
-	Hold on the figure.
-	Plot the Angle _in
-	Angle_in and Final_Angle_DA_I / Final_Angle_DA_II should follow each other.
-	The step Angle can be varied from the Simulink HDL counter in MUSIC_repo _final. It is noteworthy that initial and final value of the angle should not exceed the intersect point of the antenna patterns. However the angle can be changed in upward downward direction.
-	The Amplitude of the intercepted data (sig_st) can be changed using matlab function in the range of 1000 to 13000 digital level.
-	Variation in data sample is adjusted by up_var and down_var variables.

# Results
-	The resources utilized by the algorithm can be evaluated from MUSIC_repo_DA_I.tcl and MUSIC_repo_DA_II.tcl for DA-I and DA-II respectively.
-	The linearity of output angle vs the input angle can be seen from .slx output.
