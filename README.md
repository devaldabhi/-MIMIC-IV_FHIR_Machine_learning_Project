# -MIMIC-IV_FHIR_Machine_learning_Project

Data Sources: 
1. Data Set: https://physionet.org/content/mimic-iv-fhir-demo/2.0/mimic-fhir/
2. https://physionet.org/static/published-projects/mimic-iv-fhir-demo/mimic-iv-clinical-databasedemo-on-fhir-2.0.zip


The main files used for this project are:
1. Patient.ndjson
2. Condition.ndjson
3. Encounter.ndjson
4. EncounterICU.ndjson (this file has the same format as Encounter.json)

The "Patient.ndjson" file describes the information connected to the patient.
The "Condition.ndjson" file represents the diseases and conditions of the Patients.
The "Encounter.ndjson" file comprises of the encounter of the Patients.

All the four files are connected via respective Ids.

The objectives of the project includes:
1. To read the format of the 4 files mentioned above.
2. To create a dictionary for every patient where the Key:Value are patient_id: Patient Condition array.
3. To create a assigned time for the condition using the corresponding encounter data. We need to choose the start_time in the Encounter to associate time to each condition. (This step is still underway)
4. The final step is to create a csv containing the Patient ID, Time Stamp in UNIX, Patient Code and Condition Description.
