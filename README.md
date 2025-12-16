# Patient-Treatment-in-Emergency-Department
Business information system's exam

This project contains an in-depth analysis of the patient treatment process within an Emergency Department (ED) using Process Mining techniques. The objective is to identify inefficiencies, bottlenecks, and deviations from the ideal workflow, linking patients' initial clinical characteristics with process performance.

Key Objectives

Identification of Performance Bottlenecks: Measure temporal metrics (Lead Time, Action Time) to identify the slowest activities, particularly "Vital sign check" and the "Transfer" phase.

Analysis of Clinical Variants: Create process variants based on clinical patterns (Acuity, Fever, Urgent Transport, Pain, Top 5 Diagnosis) to identify patient groups experiencing the longest delays.

Process Model Discovery: Reconstruct the actual process model (using the Inductive Miner) and evaluate its Conformance against real event logs.

Main Results

Critical Variant: The clinical variant '10100' (High Acuity, Urgent Transport, etc.) was identified as the pathway with the highest median Lead Time (631 minutes).

Low Standardization: The process exhibits very low standardization; only 11.54% of cases are covered by the 10 most frequent variants.

Deviations from the Model: Activities related to medication management ("Medicine dispensations" and "Medicine reconciliation") are the main sources of deviation from the discovered process model.

Repository Structure

exam.ipynb / exam_en.ipynb: Contains all Process Mining code, from data cleaning (pre-processing) to performance analysis, process model discovery (Petri Net), and clinical variant analysis.

dataset_for_exam.csv: (Not included, reference only) Event log used for the analysis.

README.md: This file.

Technologies Used

Python

Pandas (Data Manipulation)

pm4py (Process Mining Framework)

Matplotlib / Seaborn (Visualization)
