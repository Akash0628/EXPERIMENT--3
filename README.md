# EXPERIMENT--3

A differential amplifier amplifies the difference between two input signals while rejecting common-mode noise, making it essential for precision applications like instrumentation and communication systems. It consists of two transistors or an operational amplifier with resistors to set the gain. The differential gain (Ad) is determined by resistor ratios, while the common-mode rejection ratio (CMRR) indicates how well the amplifier suppresses noise. Ideally, a high CMRR ensures minimal interference from external sources. Practical applications include signal conditioning, sensor amplification, and audio processing, where accurate differential signal amplification is crucial.
## Question:- 
Design the defferntial amplifier for the given parameters and do DC, AC and Transisent analysis by replacing the Rss with current source and current source, Rd with MOSFET.
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

![AC output](https://github.com/user-attachments/assets/2504d1db-f47c-4997-8ec1-ccd072471917)

### Transient analysis

![transient output](https://github.com/user-attachments/assets/a2e796a2-f1fb-443f-9aa5-924ab7f3792a)

## Replaced Rss with a Current Source(0.90mA)

### DC Analysis


### AC Analysis


### Transient Analysis



## Replaced Current source and Rd with MOSFET 

### DC Analysis



### AC Analysis



### Transient Analysis


## Inference 
* The Id depends on Vb or Vincm value.
* If Vincm increases that side Id will decreases and vout will increase.
* Iss always in constant.
* High CMRR value indicates effective common mode noise rejection.
* Resistor mismatch affects the gain stability and reduces CMRR.
* To act as amplifeir, biasing ensures symmetrical.

## Final Conclusion
* Amplifies the difference between inputs while rejecting common-mode signals.
* Demonstrates a high CMRR when resistors are well-matched.
* Shows expected gain values, validating theoretical calculations.
* Exhibits some practical limitations, like resistor mismatch and power supply sensitivity.
