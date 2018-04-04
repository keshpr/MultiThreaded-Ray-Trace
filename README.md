# MultiThreaded-Ray-Trace
Multi-threaded ray tracing program

Modified the code to implement multi-threading. The original, single-threaded program was gotten from
Brian Allen's SRT implementation (http://web.cs.ucla.edu/classes/winter18/cs35L/assign/srt.tgz). I changed 
main.c and the Makefile to implement a multi-threaded version of this ray-tracing algorithm. The program
creates an image which is always the same as baseline.ppm (provided in the zip file)
regardless of the number of threads used (as expected).

To run, unzip Ray_Trace.zip. On the command line (perhaps bash), go to the srt folder gotten after unzipping Ray_trace. Run
"make clean check". This creates the srt executable and creates 4 images, each made using 1, 2, 4 and 8 threads respectively.
It also prints the amount of time taken to execute the program.
The images will be labelled 1-test.ppm, 2-test.ppm, and so on. To create an image using a particular number of threads, 
run the srt executable just made with the number of threads you wish to use as the argument.
For example, on bash, you would run "./srt 32 > 32-test.ppm" if you wished to use 32 threads and save the result in 
an image named 32-test.ppm. 

