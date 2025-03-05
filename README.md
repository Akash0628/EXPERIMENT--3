# EXPERIMENT--3

A differential amplifier is a fundamental circuit in analog electronics that amplifies the difference between two input signals while rejecting common-mode signals. It is widely used in instrumentation, communication systems, and operational amplifier applications.

### Given Parameters
* Vdd=3.3v
* p<=3mw
* Vincm=1.72v
* Vocm=1.81v
* Vp=0.7v

### Extracting parameters from the given values are:-
1. Iss=P/Vdd
=3*10^-3/3.3k
=0.90mA
2. Id=Iss/2=0.45mA
3. Rd=Vdd-Vocm/Id=3.3kohm
4. Rss=Vp/Iss=777ohm
## Circuit Diagram

![ckt](https://github.com/user-attachments/assets/c7315d6c-fc71-474a-ba49-8541ccccb0ee)

## Procedure
* Design a cirtcuit diagram in ltspice as per given.
* Give the extracted values for each components.
* To get an accurate output vary the both transistors width.
* Attach the library file before simulation.
* Run DC, AC and transient anlysis and compare the simulation value with calculated value.
* Observe waveform and bandwidth.
* Replace Rss with the current source and observe the DC,AC and transient analysis.
* Again replace MOSFET with MOSFET and observe the DC,AC and transient analysis.
* Replace both Rd with MOSFET and set a Vb value and width of the transistor, Do same DC,AC and transient anlysis.

### DC Analysis
with MOSFET Length=180nm and Width=7.8um
![dc output](https://github.com/user-attachments/assets/e70dbc15-245d-4f99-a311-49f103d2bb5b)

### AC Analysis

!(https://github.com/user-attachments/assets/5e610a88-f0c0-4db8-ae69-9599f11d691d)
