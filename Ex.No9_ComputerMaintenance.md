# Ex.No: 9  Logic Programming –  Computer Maintenance Expert System
### DATE:25-03-2024                                                                            
### REGISTER NUMBER : 212221220006
### AIM: 
Write a Prolog program to build a computer maintenance expert system.
###  Algorithm:
1. Start the program.
2. Write the rules for each fault in computer.
3. If system have printing problem, missing dots and no uniform printing then system fault on printer head.
4. If system have not printing, missing dots and spread inks then system fault on ribbon
5. If system have not printing, paper jam and out of paper then system fault on paper stuck in printer
6. Similarly define rules for all faults.
7. Define facts for system problems.
8. Find the fault of computer by passing query to system.
### Program:
~~~
fault(printer_head) :- 
 problem(not_printing), 
 problem(missing_dots), 
 problem(nonuniform_printing). 
fault(ribbon) :- 
 problem(not_printing), 
 problem(missing_dots), 
 problem(spread_ink). 
fault(paper) :- 
 problem(not_printing), 
 problem(paper_jam), 
 problem(out_of_paper). 
fault(motherboard) :- 
 problem(long_beep), 
 problem(short_beep). 
fault(hard_disc) :- 
 problem(two_short_beeps), 
 problem(blank_display). 
problem(not_printing). 
problem(missing_dots). 
problem(spread_ink). 
problem(two_short_beeps). 
problem(blank_display).
~~~
### Output:
![318455937-d29c4f9d-152e-4e7f-bb93-ed890a599bbd](https://github.com/andralikitha/AI_Lab_2023-24/assets/131592130/57cf8069-9a04-4a69-bf63-2c7a0a58111a)
### Result:
Thus the simple omputer maintenance expert system was built sucessfully.
