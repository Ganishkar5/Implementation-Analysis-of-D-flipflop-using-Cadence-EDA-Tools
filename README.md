## Ex No: 02--Design-Implementation-of-Full-Custom-2-1-MUX-using-Cadence-EDA-Tools

### Aim:

To design and implement a 2:1 multiplexer (MUX) circuit using Cadence EDA tools, analyse its functionality and performance, and understand the principles of digital logic design, including schematic creation, layout design, and simulation.

### Tools Required:

- Personal Computer
- Cadence Virtuoso Software

### Circuit Diagram:

![WhatsApp Image 2024-11-13 at 17 18 04_bc5d2779](https://github.com/user-attachments/assets/7d01593f-2198-432d-90a8-c78652784498)

### S C H E M A T I C S I M U L A T I O N:

PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION
Commands to get into Cadence

1.	Right Click and open the terminal window
2.	Type the following commands as follows and press enter.
	- csh
	- source /cadence/install/cshrc
	- virtuoso

Procedure for Schematic simulation using Cadence

1.	Now two windows must open i)virtuoso/command interpreter window ii)”Whats New…”

2.	Close the 2nd window
3.	Use 1st window i.e virtuoso window(CIW) for further processing.
	
  - Create a New Library
  - Create Schematic Cell view.
  - Create the Symbol for schematic Cell view.
  - Create the test Cell view.
  - Analog simulation by spectre



i)	Procedure for Creating New Library.

- File –New – Library
- Name : Give name for ur library Ex: VLSILAB_EXP_2
- Enable Attach to an existing technology library, Click OK
- Attach the library to the technology library gpdk045.Click OK

ii)	Create Schematic Cell view.

- Go to 1st window i.e virtuoso(CIW)
- File-New-Cell view
- Setup the new file form
	 + Library: Select the one you a created.
	 + Cell : Give the experiment name Ex: Inverter View_Schematic
	 + Type: Schematic press OK
    
- Add the required components from the libraries and make the connections.
	 + Go to instance fixed menu or use shortcut key “I” from keypad to go instances
	+ Click on browse. This opens the library browser
	+ Now select the appropriate library for components like 
	+ Gpdk45 ------------------------nmos1v,  pmos1v
	+ Create Input and Output pins
	+ Make the connections by using fixed narrow wire key
	+ Click Check and Save button

![Screenshot (90)](https://github.com/user-attachments/assets/45a26ca0-717e-4f90-80b6-680108c84f3c)
	
 
iii)	Creating the Symbol for schematic Cell view

- In the schematic window, execute 
	+	Create – Cell view – From Cell view
	+	The cell view from cell view window appears
	+	Check Lib Name, Cell Name, From View name must be schematic Press ok
- Now Symbol generation form appears. Click Ok If No changes required
- A new window with with default symbol is created.
- Edit the symbol if you want to give actual symbol shape else continue.
- Execute Create-Cell view-from cell view
- Library Name and Cell Name must be same which you have used for schematic. Press OK
- Check for the position of pin side.Prss OK
- Edit for the shape by Create-Shape-Choose required options to edit.

![Screenshot (93)](https://github.com/user-attachments/assets/fc96fe90-456d-4112-a666-af948daa9085)
 
iv)	Creating the new test cell view

- Go to CIW window, Execute File-New-Cell view
	+ Setup the new file form
	+ Library: Select the one you created.
	+ Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test
	+ View: Schematic
	+ Type: Schematic press OK
- Follow the step 3(ii) d to make the required connections

![Screenshot (95)](https://github.com/user-attachments/assets/1d9510b0-c803-440b-9b5a-4532194dd2ef)

### Analog simulation by SPECTRE.

- In test cell view window
- Launch – ADE L(Analog Design Environment)
	+ Execute Setup—Simulation/directory/Host A new window opens
	+ Set the simulation window to spectre and click ok
	+ Execute Analysis – Choose. A window opens.
	+ Select the type and set the specifications and press OK
	+ Execute Output s—to be plotted – Select on Schematic
	+ Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
- Execute Simulation -- Net list and Run

![IMG-20241019-WA0010](https://github.com/user-attachments/assets/e532f49e-b60f-4629-bb39-9f9b4085b36f)

### For Transient Analysis Settings and Output

![IMG-20241019-WA0013](https://github.com/user-attachments/assets/92433262-d11d-460f-899b-5c3d1e661266)


 ![IMG-20241019-WA0014](https://github.com/user-attachments/assets/eef27219-4166-4c49-8662-ee7e0ddb6894)

### Results:

1. The experiment successfully demonstrated the design and implementation of a 2:1 MUX using Cadence EDA tools. 
2. The successful verification through schematic, layout, and simulation underscores the effectiveness of using Cadence EDA tools for digital circuit design.
