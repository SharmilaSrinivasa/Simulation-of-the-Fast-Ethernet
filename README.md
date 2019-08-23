# Simulation-of-the-Fast-Ethernet
This project is to simulate the Fast Ethernet. The goal of the project is to practice basic socket API programming through a client/server application. It is a simulation in the sense that the fast Ethernet is simulated by multiple processes on multiple machines. Each station in the Ethernet is simulated by a process. The switch of the fast Ethernet is also simulated by a process. Those processes can run on different workstations in the Linux lab.

The simulation is composed of the following processes:

Station Process (SP):
One station process for each simulated station. For flexibility the
number of such station processes allowed should be a variable. This simulating an Ethernet consisting of at most ten stations.

Communication Switch Process (CSP):
There is only one such process, which simulates
the function of a switch in a fast Ethernet.
For every station, the sequence of frames to be sent, together with the destination station
number, is specified as simulation input data file that will be read by that particular station

The project is implemented using C programming language. 
The project contains a program ‘CSPtcp.c’ that implements the functionalities and it acts as server in the client/server implementation. 
It contains 10 station process ‘Station_Process1.txt’, ‘Station_Process2.txt’, ‘Station_Process3.txt’, ‘Station_Process4.txt’, ‘Station_Process5.txt’, 
‘Station_Process6.txt’, ‘Station_Process7.txt’, ‘Station_Process8.txt’, ‘Station_Process9.txt’, ‘Station_Process10.txt’’ which acts as input files. Hence, we can access at most 10-station processes for the communication bus process. TCP.IP protocol is chosen as the underlying protocol of the communication in this project.
