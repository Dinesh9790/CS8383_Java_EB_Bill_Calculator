# Electricity Bill Generator Application

*Platform: JAVA*
*Author: Rajasekaran S*
*E-mail: kite.rajasekaran@gmail.com*

## Problem Statement
Develop a Java application to generate Electricity bill. Create a class with the following members: *Consumer no., consumer name, previous month reading, current month reading, type of EB connection(i.e domestic or commercial).* Compute the bill amount using the following tariff.
If the type of the EB connection is domestic, calculate the amount to be paid as follows:
- First 100 units - Rs. 1 per unit
- 101-200 units - Rs. 2.50 per unit
-  201 -500 units - Rs. 4 per unit
-  More than 501 units - Rs. 6 per unit

If the type of the EB connection is commercial, calculate the amount to be paid as follows:

- First 100 units - Rs. 2 per unit
- 101-200 units - Rs. 4.50 per unit
- 201 -500 units - Rs. 6 per unit
- More than 501 units - Rs. 7 per unit

## Problem Identified

Need to create a class Main with following members:

**Attributes**
- Consumer Number
- Consumer Name
- Previous Month Reading
- Current Month Reading
- isDomestic [To Check with user for domestic or commercial connection]
- totalBillAmount

**Methods**
- getDetails [To get the user details mentioned in above attributes].
- displayCommercialFare [For user identification]
- displayDomesticFares [For user identification]
- generateBill [For calculating the bill amount according to their connection type]
- displayBill [For display the bill details to user]
- main [Default and Primary need]

## Algorithm

1. Start the Process.
2. Create an Object for class Main.
3. Using Main class object get the user informations using getDatils method and read the information using scanner object.
4. Call displayBill method
	1. Call generateBill.
		1. Calculate number of units consumed by current month reading - previous month reading.
		2. If current user is domestic
			1. Compute with domestic scale using loop and find the sum
		3. Else
			1. Compute with commercial scale using loop and find the sum
		4. Store final sum as totalBillAmmount
	3. Display user's details [Consumer Number, Name, Number of units consumed].
	4. Display bill amount.
	5. Display Fare details.
		1. If user is domestic display domestic scale.
		2. Else display commercial scale.
5. Stop the process
