# DSC-563-DSC 563 – Module 2: Tableau Visualization and Verification
Research Focus and Audience
Research Question: How does workshop attendance differ by neighborhood, and how do utilization methods and missing attendance data shape the interpretation of results?
Intended Audience: Community workshop coordinators who track attendance and plan seating capacity.
Purpose: Compare attendance across neighborhoods and assess how methodological choices affect utilization measures and conclusions.
________________________________________
Data Source, Simulation, and Reuse
•	Dataset: DSC 563 course-provided workshop attendance dataset
•	Data Period: May–October 2026
•	Neighborhoods: East, North, South, and West
•	Data Type: Records of workshop attendance and seating capacity
•	Simulation Status: These simulated records do not reflect actual community workshop attendance.
•	Source Attribution: DSC 563 course-provided workshop dataset
•	Reuse Restrictions: Intended for educational analysis. No additional redistribution rights are claimed; follow any course-specific restrictions.
________________________________________
Repository File Guide
File	Description
tableau_workshops_tidy.csv	Simulated workshop data for Tableau analysis
m01_claim_check.csv	Python-verified October 2026 attendance values for checking claims
m01_after_chart.png	Module 1’s improved Python chart of neighborhood attendance
DSC563_Module2_Tableau.twbx	Packaged Tableau workbook with attendance, utilization, and coverage worksheets
tableau_comparison.png	Screenshot or crosstab showing the numerical comparison between Tableau and Python
README.md	Project documentation and steps to reproduce the analysis

Note: Use filenames that exactly match those uploaded to the GitHub repository.
________________________________________
Run the Module 1 Notebook in Google Colab
Colab Notebook
Tibbitts_Kaitlin_Moudle_01_Audience_First_Chart.ipynb - Colab
Reproduce the Python Analysis
1.	Use the link above to open the Module 1 notebook.
2.	If prompted, sign in to Google.
3.	Select Runtime → Run all.
4.	Wait for every cell to finish running.
5.	Examine the original and improved attendance charts.
6.	Find the October 2026 attendance results.
7.	Examine the graduate analysis of missing-attendance assumptions.
8.	Find and examine these files:
o	m01_after_chart.png
o	m01_claim_check.csv
Expected Analysis Outputs
•	Original attendance chart
•	Improved attendance chart
•	October 2026 attendance summary
•	Missing-attendance sensitivity analysis
•	Verification file with attendance values for comparison with Tableau
________________________________________
Tableau Settings for Reproducing the Python Chart
•	Selected Month: October 2026
•	Dimension: Neighborhood
•	Measure: Attendance Visits
•	Aggregation: SUM
•	Units: Seat visits
•	Chart Type: Horizontal bar chart
•	Sorting: Attendance, highest to lowest
Chart Design
•	Numeric data labels
•	Zero baseline
•	Neighborhood order matching the Python chart
This configuration reproduces Module 1’s improved Python chart.
________________________________________
Verified Values and Supporting Evidence
Python–Tableau Verification
Neighborhood	Python	Tableau	Difference
East	94	94	0
North	90	90	0
West	90	90	0
South	82	82	0


Verification Summary
•	Results matched exactly for all four neighborhoods.
•	Each difference was 0.
•	Tableau reproduced Python’s attendance results without discrepancies.
Where to Find the Evidence
•	Python validation values: m01_claim_check.csv
•	Tableau validation values: October 2026 Attendance worksheet
•	Supporting proof: tableau_comparison.png
________________________________________
Supporting Graduate Analysis
Module 1 Missing-Attendance Analysis
•	East’s attendance records covered 5 of 6 months (83.3% coverage).
•	All other neighborhoods had records for 6 of 6 months (100% coverage).
How Assumptions Change Utilization
Assumption	Utilization
Only Observed Months Included	73.57%
Missing Attendance Counted as Zero	62.42%
Difference	11.15 percentage points

These results show how missing-data assumptions can change utilization estimates and conclusions.
Evidence Location: The Module 1 Colab notebook’s graduate analysis section.
________________________________________
Comparing Utilization in Tableau
Utilization by Neighborhood
Neighborhood	Mean Monthly Utilization	Capacity-Weighted Utilization	Observed Months
East	73.4%	73.6%	5/6
North	73.1%	73.2%	6/6
South	79.9%	80.0%	6/6
West	59.2%	59.4%	6/6

Worksheets Supporting the Results
•	Utilization Comparison
•	Monthly Coverage
Main Findings
•	South’s utilization was highest, at about 80%.
•	West’s utilization was lowest, at about 59%.
•	Utilization percentages were similar under both methods.
•	Neighborhood rankings were identical under both methods.
________________________________________
A Key Analytical Assumption
The treatment of missing attendance is a key analytical choice.
A missing record does not necessarily indicate zero attendance. Counting East’s missing month as zero reduced utilization from 73.57% to 62.42%, a decline of 11.15 percentage points.
Missing data therefore needs to be identified, documented, and assessed before conclusions are drawn.
________________________________________
Analysis Limitations
•	The simulated dataset does not reflect actual community workshop attendance.
•	One month of East’s attendance data was missing.
•	The analysis shows how assumptions change utilization calculations but cannot establish attendance for the missing month.
________________________________________
Access the Tableau Workbook
Workbook Filename: DSC563_Module2_Tableau.twbx
Workbook Access Steps
1.	Download the packaged workbook (.twbx).
2.	Use Tableau Desktop or Tableau Public to open the file.
3.	Check attendance values in the October 2026 Attendance worksheet.
4.	Examine utilization metrics in the Utilization Comparison worksheet.
5.	Check data completeness in the Monthly Coverage worksheet.
6.	Check worksheet values against these files:
o	m01_claim_check.csv
o	tableau_comparison.png
________________________________________
Project Verification Checklist
1.	Run every cell in the Module 1 Google Colab notebook.
2.	Find m01_claim_check.csv and examine Python’s attendance results.
3.	Download the packaged Tableau workbook and open it.
4.	Open the October 2026 Attendance worksheet.
5.	Confirm that Tableau and Python match for all four neighborhoods.
6.	Examine the Utilization Comparison worksheet.
7.	Use the Monthly Coverage worksheet to verify that:
o	East has observations for 5 of 6 months.
o	North, South, and West have observations for 6 of 6 months.
8.	Examine the Module 1 notebook’s missing-attendance sensitivity analysis.
________________________________________
Analysis and Sharing Tools
•	Python (Google Colab)
•	Tableau
•	GitHub
________________________________________
Summary of Conclusions
Using the same data, filters, units, and aggregation settings, Tableau reproduced Python’s October 2026 attendance results exactly. Verification found zero differences across all four neighborhoods.
Mean monthly and capacity-weighted utilization yielded nearly identical percentages and the same neighborhood rankings. In contrast, the sensitivity analysis showed that missing-data assumptions can substantially change utilization estimates. These findings underscore the need for reproducible calculations, complete data, and transparent assumptions when presenting results.
