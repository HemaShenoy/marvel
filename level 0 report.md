## **Task 2: API**
<br>
<br>

APIs act as intermediaries that allow different software applications to communicate and share data seamlessly. They define the methods and data formats that applications can use to request and exchange information. APIs can be categorized into different types, including web APIs, library-based APIs, and operating system APIs.<br><br>

### **Building a Weather App using OpenWeather API:**
<br>
Steps: 
<br> 

+ Sign up for an API key from OpenWeather.
+ Identify the API endpoint for the desired functionality (e.g., "current weather").
+ Make API calls from your app using the obtained API key and necessary parameters (e.g., city name).
+ Extract relevant information from the API response.
+ Display the extracted information in your app's user interface.<br>

LINK: https://github.com/HemaShenoy/HemaAIML<br>

![weather](https://github.com/HemaShenoy/images/assets/122464897/bcc8822c-9cc8-4e9d-aa58-ba65721651ac)

---

## **TASK 4: Get familiar with the command line on ubuntu and do the following subtasks:** <br><br>

### **Ubuntu Command line subtasks:**
Create a folder - Use command<br>
 ``` 
mdkir < name of folder >
```
 <br>

cd into that folder -<br>
 ```
cd < name of folder >
``` 
<br>

Creating a blank file -<br>
 ```
touch < name of file>
```

 <br>
and ls to list all folders.
Create 2600 folders in this folder -<br>

```
mkdir -p a[1..2600] 
```
 <br>
where a is the common name of the folders.
Now list all using ls. 
<br>
 Concatente 2 text files and display -<br>

```echo "< text content-1 >" >> f1 
echo "< text content-2 >" >> f2
cat f1 f2 > f3 
//Creating f3 to store values of f1 and f2
cat f3 - Displays the Output 
```

![ubantu](https://github.com/HemaShenoy/images/assets/122464897/5c400c6b-07e0-4f7f-855f-d3c05c5ca91a)

![ubantu](https://github.com/HemaShenoy/images/assets/122464897/27d7dad6-01a6-47c8-b022-715dab48c780)

---

## **TASK 6: Working with Pandas and Matplotlib:**
<br>
<br>
1.Set Up Your Environment.

![panda1](https://github.com/HemaShenoy/images/assets/122464897/e6746530-7537-412a-9e77-6b7a07f5250e)

2.Create Your First Pandas Plot.<br>
3.Look Under the Hood: Matplotlib.<br>
4.Survey Your Data.<br>
5.Distributions and Histograms.<br>
6.Outliers.<br>
7.Check for Correlation.<br>
8.Analyze Categorical Data.<br>
9.Grouping.<br>
10.Determining Ratios.



	
![panda2](https://github.com/HemaShenoy/images/assets/122464897/09711717-acae-441c-ace8-090c7bdf637e)

**HISTOGRAM**
![panda3histogram](https://github.com/HemaShenoy/images/assets/122464897/7a1ef320-934e-417d-bf4f-3b968f9c28dd)


	
 
**SCATTER PLOT**
![panda4](https://github.com/HemaShenoy/images/assets/122464897/7e2507e8-5b87-4e11-a27d-cfec6b1a9ba5)




**BAR SLOTS**
![panda5barslot](https://github.com/HemaShenoy/images/assets/122464897/4fd3c36f-07d9-475f-bbe4-928fbc113475)


 
**PIE CHART**
![panda6piechart](https://github.com/HemaShenoy/images/assets/122464897/eea3b7b2-1f93-4e48-aa78-886f9231fe82)



![panda7](https://github.com/HemaShenoy/images/assets/122464897/c6fa0f04-cf14-473e-832a-7d74599d5e45)

---

## **TASK 7: Create a Portfolio Webpage**<br><br>
Creating a portfolio webpage involves several steps, including setting up the project structure, designing the layout, incorporating content, styling with CSS, and deploying it to a Git repository. Below is a simplified guide using HTML, CSS, and Git:
<br>
**Step 1: Project Setup**


-	Create a new directory for your project.
-	Initialize a Git repository.
-	Create necessary files.
<br><br>

**Step 2: HTML Structure**
<br><br>

**Step 3: CSS Styling**
<br><br>

**Step 4: Git Operations**

+ Add all files to the staging area.
+ Commit the changes.
+ Create a new repository on GitHub.
+  Link your local repository to the remote repository on GitHub.
+ Push your code to GitHub.
<br><br>
   
**Step 5: Deployment**
+ Go to your GitHub repository.
+ Navigate to the "Settings" tab.
+ Scroll down to the "GitHub Pages" section.
+ Choose the branch you want to deploy (usually the "master" branch).
+ Your portfolio will be accessible at `https://<your-username>.github.io/<repository-name>`.
<br>

**Link:** https: //github.com/HemaShenoy/HemaAIML
![Screenshot (5)](https://github.com/HemaShenoy/images/assets/122464897/7cc20967-fb0e-4dda-9b26-4d0208b08580)

---


## **TASK 9: Tinkercad**

<br>
<br>

**Components Required:**
<br>
+ Arduino Uno R3 board
+ Ultrasonic sensor (HC-SR04)
+ 16×2 LCD I2C Display
+ Jumper Wires
<br>
**Setup:**
<br>
+ Connect the Echo pin of the sensor to the D2 pin of the Arduino.
+ Connect the Trig pin of the sensor to the D3 pin of the Arduino.
+ Navigate to Tools and select board and port.
+ Verify and compile the code, then upload the code to the Arduino Uno R3 board.
+ Monitor the output in the Serial monitor (Set the baud rate as 9600). To open Serial monitor Tools>Serial Monitor or (Ctrl+Shift+M).
<br>
**CIRCUIT:**
<br>
![tinkercad1](https://github.com/HemaShenoy/images/assets/122464897/aa9e4945-bc30-4218-b7fe-49774c48f3ce)


 
 
**OUTPUT:**
![tinkercad2](https://github.com/HemaShenoy/images/assets/122464897/3d0be7f3-3c22-41e7-a08e-6374427e3a1c)

---

## **TASK 11: LED Toggle Using ESP32**
<br>
<br>
1)Installing the ESP32 board in Arduino IDE<br>
2)Components Required.

+ ESP32 development board –  read ESP32 Development. 
+ Boards Review and Comparison.
+ 2x 5mm LED.
+ 2x 330 Ohm Resistor.
+ Breadboard.
+ Jumper wires.

3)Pinout and Schematic<br>
![toggle1](https://github.com/HemaShenoy/images/assets/122464897/05f740b7-8efb-49ec-814a-2c7f06c96d74)


4)ESP32 Web Server Code<br>
5)Main Execution Code <br>
6)Uploading the Code<br>
7)Finding the ESP IP Address<br>
8)Accessing the Web Server<br>
9)Testing Results with Web Server<br>
![toggle2](https://github.com/HemaShenoy/images/assets/122464897/ba5ad8f4-9992-4315-9c33-78d15fd3992b)

---

## **TASK 12: Soldering Prerequisites**<br><br>

Soldering is a fundamental skill in electronics, and it's crucial to perform it safely and effectively. Here's a guide to the soldering prerequisites, equipment, and a basic soldering task (LED circuit on a perf board).<br>
### **Soldering Equipment:**<br>
**Soldering Iron:**
The soldering iron is the primary tool used to heat and melt solder. It comes with various tips for different applications.
<br>
**Solder:**
Solder is a metal alloy with a low melting point. It is used to create a conductive joint between components.
<br>
**Soldering Wick:**
Solder wick (desoldering braid) is used to remove excess solder or unsolder components.
<br>
**Flux:**
Flux is a chemical substance that aids in soldering by removing oxidation from the metal surfaces and improving solder flow.
<br>
**Soldering Stand:**
A stand to hold the soldering iron when not in use prevents accidents and damage.
<br>
**Safety Gear:**
Safety glasses to protect eyes from solder splatter.
Adequate ventilation to avoid inhaling solder fumes.
<br>
 
### **SOILDERING STEPS :**

- Gather components (e.g., LED, resistors, wires) for soldering onto the perf board.
- Apply a small amount of solder to the iron's tip before use (tinning).
+ Place components on the perf board in the desired arrangement.
+ Apply a small amount of flux to solder joints to enhance soldering.
+ Touch the soldering iron to the joint, heating both the component lead and board pad.
+ Once the joint is hot, touch solder to it; solder should melt and flow smoothly.
+ Remove the iron but keep the joint undisturbed until solder solidifies.
+ Visually inspect for a shiny, smooth appearance; a good joint should be concave, not bulging.
+ Use solder wick to remove excess solder or desolder components if necessary.

![soilder1](https://github.com/HemaShenoy/images/assets/122464897/3c718109-7a01-4d7e-9c9d-055d4a216167)

---

## **TASK 13:**<br><br>
         Design a 555 astable multivibrator with duty cycle 60%, rig up the circuit on a breadboard and by using the probes observe the output of your circuit on the DSO.

<br>

**Basic Astable 555 Oscillator:**
The 555 IC can function as an astable oscillator to generate continuous square wave pulses.
It operates by continuously re-triggering itself, allowing it to function as a free-running oscillator.<br><br>

**Circuit Configuration:**
Connect pins 2 (trigger) and 6 (threshold) together to enable re-triggering for astable operation.
The timing resistor from the monostable circuit is split into two resistors, R1 and R2.
<br><br>

**Waveform Generation:**
During each cycle, the capacitor charges through both R1 and R2 but discharges only through R2.
Output waveform voltage level is approximately Vcc−1.5V.
<br><br>

**Charge and Discharge Times**:
Charge time (t1) and discharge time (t2) determine the frequency of oscillations.
T=t1+t2, where T is the total periodic time.
<br><br>

**Output Frequency Equation:**
f=1/T=1/(t1+t2).<br><br>

**Duty Cycle Adjustment:**
Duty cycle  can be adjusted by changing the ratio of resistors R2 to R1.
Duty cycle is the ratio of the "ON" time to the "OFF" time.
<br><br>

**Summary**

The 555 IC in astable mode generates stable square wave output.
Duty cycle can be adjusted for specific applications.
The 50% duty cycle can be achieved by modifying the circuit configuration.
Changing resistor and capacitor values alters the oscillation frequency.

  

![task13 1](https://github.com/HemaShenoy/images/assets/122464897/1d2727bd-0baf-40f2-852d-e0ff666425b5)
![task13 2](https://github.com/HemaShenoy/images/assets/122464897/c6d465e0-45a0-47ea-8bd4-78c50124a85b)

---


## **TASK 15: Active Participation:**<br><br>

	Enroll for a MOOC and complete the course.
I enrolled for IBM SKILLBUID -Open Source Origin Stories: Adventures in Hybrid Cloud, AI Ethics, and Open Source Technologies and also completed the course.
![screenshot3](https://github.com/HemaShenoy/images/assets/122464897/195591c4-cdfb-4891-9a21-4091d9f0b910)
<br>
<br>
<br>
<br>








