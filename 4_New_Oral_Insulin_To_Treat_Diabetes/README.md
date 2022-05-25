# New oral insulin to treat diabetes


This project is from Udacity's Data Analysis Nanodegree professional track

### Overview:
This application is written with Python script using Numpy, Pandas and Matplotlib libraries to explore data from csv files
for 350 patients participated in clinical trial by:

*	Gathering, assessing and cleaning data trying to understand more details about it and identify any issues and modify the dataset for easy and fast analysis.
*	Explore this data and try to find patterns in it, compute statistics and visualize the relationships to answer the required questions and detect the characteristics that affect patients insulin level.

### The main target from this application is to answer these questions:

1 - Is new oral treatment Auralin has more adverse reactions than injectable isnulin novodra?
2 - Is dose change on Auralin acceptable compared to novodra?
3 - What is the hba1c change difference between Auralin and novodra?

### Dataset descriptions:
This dataset has information about 350 patients participated in this clinical trial. None of the patients were using Novodra (a popular injectable insulin) or Auralin (the oral insulin being researched) as their primary source of insulin before. All were experiencing elevated HbA1c levels. All 350 patients were treated with Novodra to establish a baseline HbA1c level and insulin dose. After four weeks, which isn’t enough time to capture all the change in HbA1c that can be attributed by the switch to Auralin or Novodra:

175 patients switched to Auralin for 24 weeks
175 patients continued using Novodra for 24 weeks


patient dataset columns descriptions:

*	patient_id: the unique identifier for each patient.
*	assigned_sex: the assigned gender of each patient (male or female).
*	given_name: first name of each patient.
*	surname: last name of each patient.
*	address: the main address for each patient.
*	city: city for the main address.
*	state: state for the main address.
*	zip_code: zip code for the main address.
*	country: country for the main address (all United states for this clinical trial).
*	contact: phone number and email information.
*	birthdate: the date of birth of each patient (month/day/year).
*	weight: the weight in pounds (lbs).
*	height: the height in inches (in).
*	bmi: the Body Mass Index (BMI) of each patient. BMI is a simple calculation using a person's height and weight. The formula is BMI = kg/m2 where kg is a person's weight in kilograms and m2 is their height in metres squared. A BMI of 25.0 or more is overweight, while the healthy range is 18.5 to 24.9. bmi for this clinical trial is 16 >= BMI >= 38.*

treatment dataset columns descriptions:

*	given_name: first name of each patient.
*	surname: last name of each patient.
*	auralin: the baseline median daily dose of insulin from the week prior to switching to Auralin (the number before the dash) and the ending median daily dose of insulin at the end of the 24 weeks of treatment measured over the 24th week of treatment (the number after the dash).
*	novodra: same as above, except for patients that continued treatment with Novodra
*	hba1c_start: the patient's HbA1c level at the beginning of the first week of treatment. HbA1c stands for Hemoglobin A1c. measures what the average blood sugar has been over the past three months. It is thus a powerful way to get an overall sense of how well diabetes has been controlled. Everyone with diabetes should have this test 2 to 4 times per year. Measured in %.
*	hba1c_end: the patient's HbA1c level at the end of the last week of treatment
*	hba1c_change: the change in the patient's HbA1c level from the start of treatment to the end, i.e., hba1c_start - hba1c_end. For Auralin to be deemed effective, it must be "noninferior" to Novodra, the current standard for insulin. This "noninferiority" is statistically defined as the upper bound of the 95% confidence interval being less than 0.4% for the difference between the mean HbA1c changes for Novodra and Auralin (i.e. Novodra minus Auralin).

adverse_reactions dataset columns descriptions:

*	given_name: first name of each patient (includes both patients treated Auralin and Novodra).
*	surname: last name of each patient (includes both patients treated Auralin and Novodra).
*	adverse_reaction: the adverse reaction reported by the patient.

(Note: This data isn't real)
