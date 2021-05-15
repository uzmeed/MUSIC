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
- 
*doc* includes the Javadoc files for the classes.

# Execution of the code
Compile and execute the appropriate Java class depending on the type of attack to be simulated.
If different cardinalities, t values or iterations are required, just change the variables in the Java classes, recompile and execute.
