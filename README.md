## 6. Analysis of the NHS Appointments in General Practice dataset for April 2021
Dataset: https://digital.nhs.uk/data-and-information/publications/statistical/appointments-in-general-practice/april-2021

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/RJBraith/Appointment_Dataset_April_21/HEAD)

**Python Version:** 3.9  

**Libraries Used:** Pandas, Matplotlib, Seaborn.

With a focus on looking at the UK as a whole, analysed tables 2a through 2d producing various figures showcasing the composition and distribution of various factors relating to appointments

The goal was to explore the dataset and derive useful information from it. This was a success.
Since the spreadsheet formatting was fairly consistent, I was able to just copy the notebook and make adjustments to labeling and importing to accommodate the different columns

---

Table 2a
	Contains data on appointment attendance throughout April 2021
	Some appointments were not followed up on -- ie, the staff did not mark whether or not
	the appointment was attended or not. These entries are marked as unknown and make up around 4%
	of the appointments in April
	
		Generate some summary information
		Compare relative size of appointment attendance
		Group by day and analyse

Table 2b
	Contains data on appointments broken divided into the healthcare professional seen
	The appointments are broken down into General Practitioner, Other Practice Staff and Unknown
	
	Other Practice Staff includes Acupuncturist, Chiropodist, Counsellor, Physiotherapist etc
	whereas GP extends to differing levels of GP seniority.
	
		Generate some summary information
		Compare how appointments are split
		Track how the split varies over time
			- Generate a percentage for each day and plot it?
			- Define a function to go through each row and return 3 percentages for you to plot
			  use apply to apply function to dataframe

Table 2c
	Contains data on appointments by method of meeting, whether this be a traditional 
	face-to-face meeting, a home visit, a telephone call or an online video call. There is also
	an unknown variable that captures any data that may have been misrecorded or omitted.
	
		Generate Summary information
		Compare distribution of appointments by mode
		Track how this changed over the course of the month
			- Could the function that you defined for table 2b be adapted / straight up used
			  to generate percentages for each column again?
			  May require tweaking the function
			  
Table 2d
	Contains data on the delay from booking an appointment to the appointment date
	
	Data is split into groups of days 
	
	There is scope here, given the formatting to say
	"how many appointments matured within one week?" which would require you to sum the three
	columns: 'Same Day2', '1 Day' and '2 to 7 Days'.
	
		Similar to previous tables,
		Generate some summary information and general percentages for the month
		Compare the relative size of each delay
		Group by day and perform analysis on delay by day
		Track how the appointment delay changed over the course of the month
