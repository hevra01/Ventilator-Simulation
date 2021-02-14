# Ventilator-Simulation
A smart ventilator simulation program to help the governmental hospital to estimate how many ventilators they will need to respond to this crisis, accounting for increased, uncertain patient arrival rates and lengths of stay.

In a hospital, there is a single queue and all patients are located in this queue when they need a
ventilator. There are three types of patients and they have a different level of priority based on their
diseases level.

The number of patients, the number of ventilators, the maximum arrival time, and the maximum
service time should be provided as an input at the beginning of the program.

Also need to maintain a simulated clock which keeps the time of the latest event handled.
There are three types of events which are as follows: (1) patient arrival, (2) start service and (3)
complete service. At the beginning, the simulated clock should be equal to 0. Regarding the
simulated clock, two examples of scenarios are given below.
    • If the first event is "patient arrival" at the 5th minute, then you need to advance the
simulated clock to 5.
    • If the current clock is 21 and the nearest event is "complete service" at the 25th minute, then
you need to advance the simulated clock to 25.

Functions:
          • parseInput: This function should parse the input and set the values of the number of
          patients, the number of ventilators, the maximum arrival time and the maximum service
          time.
          • createPatientList: This function should randomly create patients based on the input
          (the number of patients, the number of ventilators, the maximum arrival time, the maximum
          service time). The patients should be stored in a linked list in ascending order based on their
          arrival time.
          • initialiseSimulator: This function should create an empty queue, and also an integer
          array to keep the availability of the ventilators.
          • newPatient: This function takes a patient from the patient list based on the arrival time and
          add him/her to the queue.
          • servePatient: This function takes a patient from the queue to be served by a ventilator.
          • reportStatistics: This function reports the statistics, such as the average time spent in
          the queue, maximum waiting time, etc. (see above).
          • main: The main function is responsible to coordinate all the functions, simulated clock and
          other required operations to run the simulator successfully.
