# Ancora-Education-Ucertify-Lab60
# Managing System Processes

> **Original Lab Source**
> 
> This lab was available through:
>
> [https://ancoraeducation.ucertify.com/app/?func=navigate_items&item_sequence=13]

## Objective of the Lab
In this lab, you will learn to manage system processes. System processes will be managed using the top, ps, pgrep commands. You will also execute the gnome-calculator in the background. 
## Instructions
### STEP 1
From the desktop, open the Terminal window. 
### STEP 2 
Execute the following command to list the processes that are running in the current shell:
```bash
ps
```
### STEP 3 
Execute the following command to list all processes that are running on this system:
```bash
ps -e
```
### STEP 4 
Execute the following ps command to list all processes that are running on this system that end in sh:
```bash
ps -e | grep "sh$"
```
### STEP 5
Execute the following pgrep command to list all processes that are running on this system that end in sh:
```bash
pgrep "sh$"
```
### STEP 6 
Execute the following command to display all processes that are running:
```bash
top
```
### STEP 7
Press s and provide Change delay from 3.0 to 5 then press the Enter key.
### STEP 8
Execute the following command to quit the top command:
```bash
q
```
### STEP 9
Execute the following command to execute the gnome-calculator program in the background:
```bash
gnome-calculator &
```
### STEP 10 
In the Terminal window, execute the following command to list all running jobs:
```bash
jobs
```
### STEP 11 
In the Terminal window, execute the following command to use the job number of the gnome-calculator program with the kill command to stop (kill) the program:
```bash
kill %1
```
### STEP 12 
In the Terminal window, execute the following commands five times to execute the gnome-calculator program in the background (Note: Enter one command at a time.):
```bash
gnome-calculator &
```
```bash
gnome-calculator &
```
```bash
gnome-calculator &
```
```bash
gnome-calculator &
```
```bash
gnome-calculator &
```
### STEP 13 
Execute the following command to stop (kill) all instances of the gnome-calculator program:
```bash
killall gnome-calculator
```
### STEP 14 
Execute the following command to execute the gnome-calculator program in the background:
```bash
gnome-calculator &
```
### STEP 15 
In the Terminal window, execute the following command to list all running processes:
```bash
ps
```
### STEP 16 
In the Terminal window, execute the following command to change the process priority of the gnome-calculator program to a nice value of 15: 
### Caution 
* Replace 12345 with the first PID of the gnome-calculator process obtained in the previous step.
```bash
renice -n 15 -p 12345
```
## Disclaimer

This repository is for **educational and personal learning purposes only**.  

The original lab content belongs to **uCertify / Ancora Education** and remains their copyrighted material.  
This repository is not affiliated with, endorsed by, or sponsored by uCertify or Ancora Education.  

No copyright infringement is intended.  
Use of any tools or techniques mentioned here should only be performed in authorized, legal environments.  
