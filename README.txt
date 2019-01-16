Data description:
A set of three test have been applied to three Li-ion cells (#1, #2, and #3). 
All the experiments start with a training phase executed keeping the cell to a temperature of 25°C thanks to the thermal chamber. 
The various steps of the training procedure are reported in Table 1.
The training phase is a repetition of charge/discharge cycles that aims at improving the cell performance before starting the real test.
The charging and the discharging processes are based on a two-stage profile: a first one with constant-current until the cell reaches the cut-off voltages, followed by a constant-voltage phase.

Table 1.
+-------------+------+-----------+--------------------------+
| Repetitions | Step | Type      | Description              |
+-------------+------+-----------+--------------------------+
| 1           | 1    | Charge    | I= 0.7 C		    |
+-------------+------+-----------+--------------------------+
| 1           | 2    | Pause     | 30 minute                |
+-------------+------+-----------+--------------------------+
| 10          | 3    | Discharge | I= 1 C   		    |
+             +------+-----------+--------------------------+
|             | 4    | Pause     | 30 minute                |
+             +------+-----------+--------------------------+
|             | 5    | Charge    | I= 0.7 C                 |
+             +------+-----------+--------------------------+
|             | 6    | Pause     | 30 minute                |
+-------------+------+-----------+--------------------------+
| 1           | 7    | Pause     | 60 minute                |
+-------------+------+-----------+--------------------------+

In order to reproduce the ageing effects, we use two different ageing profiles.
Ageing A phase consists on the repetition of 50 charge/discharge cycles with a current of 0.7C and 1C, respectively, and divided by a short pause, as described in Table 2. 

Table 2. 
+-------------+------+-----------+--------------------------+
| Repetitions | Step | Type      | Description              |
+-------------+------+-----------+--------------------------+
| 50          | 1    | Discharge | I= 1 C                   |
+             +------+-----------+--------------------------+
|             | 2    | Pause     | 30 minute                |
+             +------+-----------+--------------------------+
|             | 3    | Charge    | I= 0.7 C                 |
+             +------+-----------+--------------------------+
|             | 4    | Pause     | 30 minute                |
+-------------+------+-----------+--------------------------+

Ageing B phase is similar to the previous one, where the charge current has been set to 5 A in order to allow the analysis of the ageing in relation with the current rate (Table 3).

Table 3.
+-------------+------+-----------+------------------------+
| Repetitions | Step | Type      | Description            |
+-------------+------+-----------+------------------------+
| 50          | 1    | Discharge | I= 1 C                 |
+             +------+-----------+------------------------+
|             | 2    | Pause     | 30 minute              |
+             +------+-----------+------------------------+
|             | 3    | Charge    | I= 2 C                 |
+             +------+-----------+------------------------+
|             | 4    | Pause     | 30 minute              |
+-------------+------+-----------+------------------------+

A characterization procedure based on a PCT test has been also defined in order to extract the cell parameters (Table 4). 
The PCT uses a train of current pulses to change the state of charge value of the cell, followed by a pause that allows us to analyse the relaxation effects and to determine the open circuit voltage values.

Table 4.
+-------------+------+-----------+--------------------------+
| Repetitions | Step | Type      | Description              |
+-------------+------+-----------+--------------------------+
| 1           | 1    | Charge    | I= 0.7 C                 |
+-------------+------+-----------+--------------------------+
| 1           | 2    | Pause     | 60 minute                |
+-------------+------+-----------+--------------------------+
| 1           | 3    | Discharge | I= 1 C                   |
+-------------+------+-----------+--------------------------+
| 1           | 4    | Pause     | 30 minute                |
+-------------+------+-----------+--------------------------+
| 1           | 5    | Charge    | I= 0.7 C                 |
+-------------+------+-----------+--------------------------+
| 1           | 6    | Pause     | 30 minute                |
+-------------+------+-----------+--------------------------+
| 20          | 7    | Discharge | I= 1 C                   |
+             +------+-----------+--------------------------+
|             | 8    | Pause     | 3 minute                 |
+-------------+------+-----------+--------------------------+
| 1           | 9    | Pause     | 60 minute                |
+-------------+------+-----------+--------------------------+
| 20          | 10   | Charge    | I= 1 C  		    |
+             +------+-----------+--------------------------+
|             | 11   | Pause     | 3 minute                 |
+-------------+------+-----------+--------------------------+
| 1           | 12   | Pause     | 60 minute                |
+-------------+------+-----------+--------------------------+
| 1           | 13   | Discharge | I= 1 C  	            |
+-------------+------+-----------+--------------------------+
| 1           | 14   | Pause     | 30 minute                |
+-------------+------+-----------+--------------------------+
| 1           | 15   | Charge    | I= 0.7 C                 |
+-------------+------+-----------+--------------------------+
| 1           | 16   | Pause     | 30 minute                |
+-------------+------+-----------+--------------------------+

The tests performed on the three cells are composed of the different repetitions of the described phases. 
Their descriptions are reported in Table 5, 6, and 7, together with the temperature imposed by the thermal chamber during each specific phase.

Table 5.
+-------------+------------------+-------------------+
| Repetitions | Phase            | Temperature       |
+-------------+------------------+-------------------+
| 1           | Training         | 25 °C             |
+-------------+------------------+-------------------+
| 6           | Characterization | 25 °C             |
+             +------------------+-------------------+
|             | Ageing A         | 25 °C             |
+-------------+------------------+-------------------+
| 1           | Characterization | 25 °C             |
+-------------+------------------+-------------------+

Table 6.
+-------------+------------------+-------------------+
| Repetitions | Phase            | Temperature       |
+-------------+------------------+-------------------+
| 1           | Training         | 25 °C             |
+-------------+------------------+-------------------+
| 6           | Characterization | 25 °C             |
+             +------------------+-------------------+
|             | Ageing B         | 25 °C             |
+-------------+------------------+-------------------+
| 1           | Characterization | 25 °C             |
+-------------+------------------+-------------------+

Table 7.
+-------------+------------------+-------------------+
| Repetitions | Phase            | Temperature       |
+-------------+------------------+-------------------+
| 1           | Training         | 25 °C             |
+-------------+------------------+-------------------+
| 1           | Characterization | 25 °C             |
+-------------+------------------+-------------------+
| 2           | Ageing A         | 40 °C             |
+             +------------------+-------------------+
|             | Characterization | 25 °C             |
+             +------------------+-------------------+
|             | Characterization | 40 °C             |
+-------------+------------------+-------------------+


Files:
C1.mat	Data for Battery #1
C2.mat	Data for Battery #2
C3.mat	Data for Battery #3

Data Structure:
cycle: top level structure array containing the charge, discharge and pause steps
- type: operation  type, can be charge, discharge or pause
- ambient_temperature: ambient temperature (degree C)
- time: the date and time of the start of the cycle, in MATLAB  date vector format
-- data: data structure containing the measurements
-- for charge the fields are:
--- Voltage_measured: 	Battery terminal voltage (Volts)
--- Current_measured:	Battery output current (Amps)
--- Time:			Time vector for the cycle (secs)
-- for discharge the fields are:
--- Voltage_measured: 	Battery terminal voltage (Volts)
--- Current_measured:	Battery output current (Amps)
--- Time:			Time vector for the cycle (secs)
--- Capacity:			Battery capacity (Ahr) for discharge till 2.75V
-- for pause the fields are:
--- Voltage_measured: 	Battery terminal voltage (Volts)
--- Current_measured:	Battery output current (Amps)
--- Time:			Time vector for the cycle (secs)
--- for the last pause step after a characterization phase:
---- params: top level structure array containing the parameters of an equivalent circuit model with two RC branches of the battery, extracted from the discharge pulses of the PCT test
----- ocv: open-circuit voltage (Volts)
----- soc: state of charge
----- r0: series resistance (Ohms)
----- r1: resistance of the first RC branch (Ohms)
----- c1: capacity of the first RC branch (Farad)
----- r2: resistance of the second RC branch (Ohms)
----- c2: capacity of the second RC branch (Farad)
----- Q: charge extracted from the discharge pulses of the PCT test (Coulomb)


			
			
