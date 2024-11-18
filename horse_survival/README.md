
# Horse Survival Prediction Using Machine Learning

## Introduction
This project analyzes the Horse Colic Dataset, a collection of medical records for horses suffering from colic, a common equine emergency. 


![image](./horse.png)


The goal is to predict the outcome (survival or non-survival) of horses based on their medical conditions, treatment, and other factors.

## Dataset Information
The dataset contains 1235 rows and 29 columns, which are categorized as follows:

| **Variable Name**        | **Description**                                                                                                   | **Type**  | **Possible Values**                                                                                                     |
|--------------------------|-------------------------------------------------------------------------------------------------------------------|-----------|--------------------------------------------------------------------------------------------------------------------------|
| `surgery`                | Indicates whether surgery was performed.                                                                          | Categorical | 1 = Yes, it had surgery<br>2 = It was treated without surgery                                                             |
| `Age`                    | Age category of the horse.                                                                                        | Categorical | 1 = Adult horse<br>2 = Young (< 6 months)                                                                                |
| `Hospital_Number`        | Numeric ID assigned to the horse (not unique if treated multiple times).                                          | Numeric   | Case number assigned to the horse.                                                                                       |
| `rectal_temperature`     | Rectal temperature in degrees Celsius.                                                                            | Numeric   | Continuous (e.g., 37.8).                                                                                                 |
| `pulse`                  | Heart rate in beats per minute.                                                                                   | Numeric   | Continuous (e.g., 30-40).                                                                                                |
| `respiratory_rate`       | Respiratory rate in breaths per minute.                                                                           | Numeric   | Continuous (e.g., 8-10).                                                                                                 |
| `temperature_of_extremities` | Subjective indication of peripheral circulation based on extremity temperature.                                 | Categorical | 1 = Normal<br>2 = Warm<br>3 = Cool<br>4 = Cold                                                                           |
| `peripheral_pulse`       | Subjective assessment of peripheral pulse strength.                                                               | Categorical | 1 = Normal<br>2 = Increased<br>3 = Reduced<br>4 = Absent                                                                 |
| `mucous_membranes`       | Subjective assessment of mucous membrane color.                                                                   | Categorical | 1 = Normal pink<br>2 = Bright pink<br>3 = Pale pink<br>4 = Pale cyanotic<br>5 = Bright red / Injected<br>6 = Dark cyanotic|
| `capillary_refill_time`  | Time taken for capillary refill.                                                                                  | Categorical | 1 = < 3 seconds<br>2 = >= 3 seconds                                                                                       |
| `pain`                   | Subjective judgment of the horse's pain level.                                                                     | Categorical | 1 = Alert, no pain<br>2 = Depressed<br>3 = Intermittent mild pain<br>4 = Intermittent severe pain<br>5 = Continuous severe pain |
| `peristalsis`            | Gut activity level.                                                                                               | Categorical | 1 = Hypermotile<br>2 = Normal<br>3 = Hypomotile<br>4 = Absent                                                            |
| `abdominal_distension`   | Degree of abdominal distension.                                                                                   | Categorical | 1 = None<br>2 = Slight<br>3 = Moderate<br>4 = Severe                                                                     |
| `nasogastric_tube`       | Presence of gas coming out of the nasogastric tube.                                                               | Categorical | 1 = None<br>2 = Slight<br>3 = Significant                                                                                |
| `nasogastric_reflux`     | Amount of reflux.                                                                                                 | Categorical | 1 = None<br>2 = > 1 liter<br>3 = < 1 liter                                                                               |
| `nasogastric_reflux_PH`  | pH level of the nasogastric reflux.                                                                               | Numeric   | Continuous (e.g., 3-4).                                                                                                  |
| `rectal_examination_feces` | Results of the rectal examination regarding feces.                                                              | Categorical | 1 = Normal<br>2 = Increased<br>3 = Decreased<br>4 = Absent                                                               |
| `abdomen`                | Condition of the abdomen based on examination.                                                                    | Categorical | 1 = Normal<br>2 = Other<br>3 = Firm feces in the large intestine<br>4 = Distended small intestine<br>5 = Distended large intestine |
| `packed_cell_volume`     | Number of red cells by volume in the blood.                                                                       | Numeric   | Continuous (normal range is 30-50).                                                                                      |
| `total_protein`          | Total protein in g/dL.                                                                                            | Numeric   | Continuous (normal range is 6-7.5 g/dL).                                                                                 |
| `abdominocentesis_appearance` | Appearance of fluid obtained from the abdominal cavity.                                                     | Categorical | 1 = Clear<br>2 = Cloudy<br>3 = Serosanguinous                                                                            |
| `abdomcentesis_total_protein` | Total protein in the fluid obtained from abdominocentesis in g/dL.                                           | Numeric   | Continuous.                                                                                                              |
| `outcome`                | The final outcome for the horse.                                                                                  | Categorical | 1 = Lived<br>2 = Died<br>3 = Was euthanized                                                                              |
| `surgical_lesion`        | Whether the problem was determined to be surgical.                                                                | Categorical | 1 = Yes<br>2 = No                                                                                                        |
| `lesion_type_site`       | Site of the lesion.                                                                                               | Categorical | 1 = Gastric<br>2 = Small intestine<br>3 = Large colon<br>4 = Large colon and cecum<br>5 = Cecum<br>6 = Transverse colon<br>7 = Rectum/descending colon<br>8 = Uterus<br>9 = Bladder<br>11 = All intestinal sites<br>00 = None |
| `lesion_type_type`       | Type of lesion.                                                                                                   | Categorical | 1 = Simple<br>2 = Strangulation<br>3 = Inflammation<br>4 = Other                                                          |
| `lesion_type_subtype`    | Subtype of lesion.                                                                                                | Categorical | 1 = Mechanical<br>2 = Paralytic<br>0 = N/A                                                                               |
| `lesion_type_specific_code` | Specific code for the lesion.                                                                                 | Categorical | 1 = Obturations<br>2 = Intrinsic<br>3 = Extrinsic<br>4 = Adynamic<br>5 = Volvulus/torsion<br>6 = Intussuption<br>7 = Thromboembolic<br>8 = Hernia<br>9 = Lipoma/splenic incarceration<br>10 = Displacement<br>0 = N/A |
| `cp_data`                | Indicates if pathology data is present.                                                                         | Categorical | 1 = Yes<br>2 = No      

# Executive Summary

This document summarizes the health and surgical outcomes of horses:

1. **Surgery Statistics**: 71% of horses had surgery; 28% did not.
2. **Age Distribution**: Predominantly adults (93%).
3. **Lesion Insights**: 68% have surgical lesions, often linked to distended intestines.
4. **Surgical Outcomes**: 
    - 61% mortality for horses with distended small intestines post-surgery.
    - 57% of operated horses did not survive; 56% survival in non-operated horses.
5. **Mucous Membrane Color**: Abnormal colors indicate higher mortality risk; normal pink suggests better survival.
6. **Abdominal Distention**: 63% survival with slight distention; 72% death with moderate to severe distention.

## Insights Deep Dive

1. **Surgery Statistics**: 71% of the horses had surgery, while 28% did not.
2. **Age Distribution**: Adults (93%) are much more common than young horses (6%).
3. **Lesion Insights**: 
    - 68% of horses have surgical lesions, indicating serious issues that typically require surgery.
    - Distended small and large intestines usually signify surgical lesions.
4. **Outcome Based on Surgery and Intestinal Condition**:
    - In cases of distended small intestine and surgery:
        - 61% of the horses died.
        - 49% were euthanized.
        - There’s a 61% chance of survival for horses with this condition if surgery is performed.
5. **Surgical Outcomes**:
    - 57% of horses that underwent surgery did not survive.
    - 56% of horses that were not operated on lived.
    - Surgery does not guarantee survival.
6. **Surgical Lesion Outcomes**:
    - 56% of horses with surgical lesions that underwent surgery died.
    - 43% of such cases survived.
7. **Mucous Membrane Color as a Predictor**:
    - Horses with pale, cyanotic, bright red, or dark cyanotic membranes are more likely to die.
    - Horses with pale pink, bright pink, or normal pink membranes are more likely to survive.
8. **Abdominal Distention Insights**:
    - With slight or no abdominal distention, there’s a 63% chance of survival.
    - With moderate or severe abdominal distention, there’s a 72% chance of death.

## Recommendations

1. **Targeted Surgical Interventions**: Prioritize surgery for horses with non-distended intestines to improve survival rates, given the high mortality (61%) associated with distended cases.

2. **Mucous Membrane Monitoring**: Regularly assess mucous membrane color in horses to identify those at higher risk of mortality and adjust treatment plans accordingly.

3. **Education on Distention Signs**: Train owners and caretakers to recognize signs of abdominal distention early, facilitating timely veterinary intervention to potentially avoid surgery.

## Caveats and Assumptions

1. **Data Completeness**: The analysis relies on the completeness of the dataset. Missing or incomplete records for any variable may lead to biased results or misinterpretations.

2. **Subjective Assessments**: Several variables, such as `temperature_of_extremities`, `peripheral_pulse`, `mucous_membranes`, `pain`, and `abdominal_distension`, are based on subjective assessments. Variability in interpretation among different veterinarians may affect consistency and reliability.

3. **Categorical Variables**: The use of categorical variables (e.g., `surgery`, `age`, `outcome`) may oversimplify complex clinical conditions. The binary or limited categorical nature may not capture the full spectrum of horse health status.

4. **Numeric Ranges**: Continuous variables like `rectal_temperature`, `pulse`, and `respiratory_rate` are subject to normal physiological variations. Values outside typical ranges may not always indicate pathology and should be interpreted in context.

5. **Potential Confounding Factors**: The analysis does not account for potential confounding factors such as breed, prior health history, or environmental conditions that may influence outcomes.

6. **Generalizability**: Findings from this dataset may not be generalizable to all horse populations, as the sample may be biased towards specific cases treated at particular facilities.

7. **Temporal Factors**: The timing of data collection (e.g., during acute illness vs. recovery) may influence the values of certain variables, particularly those related to physiological parameters.

8. **Outcome Definitions**: The definitions of outcomes (e.g., `lived`, `died`, `euthanized`) may vary based on clinical judgment and should be interpreted with caution.

9. **Surgical Lesion Classification**: The classification of lesions (`surgical_lesion`, `lesion_type_site`, `lesion_type_type`) is based on clinical findings and may not always correlate with histopathological results.

10. **Data Entry Errors**: The dataset may contain errors due to manual data entry, which could affect the accuracy of the analysis.

These caveats and assumptions should be considered when interpreting the results of the analysis to ensure a comprehensive understanding of the findings.

## How to Run the Notebook

1. Clone the repository:

   ```bash
   git clone https://github.com/dakshbhatnagar/projects/horse_survival.git
   ```

2. Switch to the directory:
   ```bash
   cd horse_survival
   ```

3. Install the required dependencies:
    ```
    pip install -r requirements.txt
    ```
4. Open the `analysis.ipynb` notebook and run all cells.

## Contributions
Contributions are welcome! Please fork the repository, make changes, and submit a pull request.

## Acknowledgements
The Horse Colic Dataset was originally published by the UCI Machine Learning [Database](https://archive.ics.uci.edu/dataset/47/horse+colic).

