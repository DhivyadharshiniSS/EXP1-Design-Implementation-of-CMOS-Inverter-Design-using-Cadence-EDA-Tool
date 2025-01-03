## Ex No: 01   Design & Implementation of CMOS Inverter Design Using Cadence EDA Tools   

### Aim:
To design and implement a CMOS inverter circuit using Cadence EDA tools, analyse its electrical characteristics, and understand the fundamental principles of CMOS technology, including the design process, layout, and simulation techniques.
### Tools Required:
-	Personal Computer
-	Cadence Virtuoso Software
### Circuit Diagram:
![WhatsApp Image 2024-11-13 at 16 02 51_d0a9f496](https://github.com/user-attachments/assets/1fa282d8-4a5e-4473-b7d9-555d3d9f7862)

# S C H E M A T I C S I M U L A T I O N - 
PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION -Commands to get into Cadence
1.	Right Click and open the terminal window
2.	Type the following commands as follows and press enter.
-	csh
-	source /cadence/install/cshrc
-	virtuoso
 Procedure for Schematic simulation using Cadence
1.	Now two windows must open i) virtuoso/command interpreter window ii)”Whats New…”
2.	Close the 2nd window
3.	Use 1st window i.e virtuoso window (CIW) for further processing.
i.	Create a New Library
ii.	Create Schematic Cell view.
iii.	Create the Symbol for schematic Cell view.
iv.	Create the test Cell view.
v.	Analog simulation by spectre

i)	Procedure for Creating New Library.
•	File –New – Library
•	Name: Give name for ur library Ex: VLSILAB_EXP_1
•	Enable Attach to an existing technology library, Click OK
•	Attach the library to the technology library gpdk045.Click OK

ii)	Create Schematic Cell view.

•	Go to 1st window i.e virtuoso (CIW)
•	File-New-Cell view
•	Setup the new file form
	Library: Select the one you created.
	Cell: Give the experiment name Ex: Inverter ViewSchematic
	Type: Schematic press OK
•	Add the required components from the libraries and make the connections.
	Go to instance fixed menu or use shortcut key “I” from keypad to go instances
	Click on browse. This opens the library browser
	Now select the appropriate library for components like 
	Gpdk45 ------------------------nmos1v, pmos1v
	Create Input and Output pins
	Make the connections by using fixed narrow wire key
	Click Check and Save button.

![Screenshot 2024-08-28 154026](https://github.com/user-attachments/assets/2e8841cc-5b2c-4153-84f4-561ebcd82767)

 
iii)	Creating the Symbol for schematic Cell view

•	In the schematic window, execute 
	Create – Cell view – From Cell view
	The cell view from cell view window appears
	Check Lib Name, Cell Name, From View name must be schematic Press ok
•	Now Symbol generation form appears. Click Ok If No changes required
•	A new window with with default symbol is created.
•	Edit the symbol if you want to give actual symbol shape else continue.
•	Execute Create-Cell view-from cell view
•	Library Name and Cell Name must be same which you have used for schematic. Press OK
•	Check for the position of pin side.Prss OK
•	Edit for the shape by Create-Shape-Choose required options to edit.

![Screenshot 2024-08-28 154626](https://github.com/user-attachments/assets/a7ccce19-d502-4509-a4d3-d42f3e3de0fa)


iv)	Creating the new test cell view

•	Go to CIW window, Execute File-New-Cell view
	Setup the new file form
	Library: Select the one you created.
	Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test
	View: Schematic
	Type: Schematic press OK
•	Follow the step 3(ii) d to make the required connections.

![Screenshot 2024-08-28 155627](https://github.com/user-attachments/assets/b4a161c0-079a-4b16-a255-004a5720b13a)


Analog simulation by SPECTRE.

•	In test cell view window
•	Launch – ADE L(Analog Design Environment)
	Execute Setup—Simulation/directory/Host A new window opens
	Set the simulation window to spectre and click ok
	Execute Analysis – Choose. A window opens.
	Select the type and set the specifications and press OK
	Execute Output s—to be plotted – Select on Schematic
	Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
•	Execute Simulation -- Net list and Run

 ![image](https://github.com/user-attachments/assets/3aac50ec-bc0f-406e-be2e-a504b8afa8c9)


### For Transient Analysis Settings and Output
 

 ![image](https://github.com/user-attachments/assets/92d14f32-8ba5-4fed-978a-38c360b8e305)
 
 ![Screenshot (18)](https://github.com/user-attachments/assets/e6080575-7bef-4f59-85e8-37caaa085145)


### For DC Analysis Settings and Output

![image](https://github.com/user-attachments/assets/0ee74107-e03a-4204-b685-83ced611c993)

![Screenshot (24)](https://github.com/user-attachments/assets/a693bfe9-7704-4483-9bd5-06b88e13d42e)



 




 

### Results:

1.	Successfully designed the CMOS inverter schematic using Cadence EDA tools.
2.	The simulation results demonstrated the correct logic operation of the inverter, where the output voltage switches between high (Vdd) and low (0V) levels, corresponding to the input voltage transitions.
3.	The Voltage Transfer Characteristic (VTC) curve was plotted, showing the relationship between input and output voltages.











