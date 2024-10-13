
# Horse Survival Prediction Using Machine Learning

## Introduction
This project analyzes the Horse Colic Dataset, a collection of medical records for horses suffering from colic, a common equine emergency. 


![image](./horse.png)


The goal is to predict the outcome (survival or non-survival) of horses based on their medical conditions, treatment, and other factors.

## Dataset Information
The dataset contains 1235 rows and 29 columns, which are categorized as follows:
- **Demographic Information**: Includes details like age and hospital number.
- **Clinical Measurements**: Includes rectal temperature, pulse, respiratory rate, etc.
- **Subjective Assessments**: Evaluates pain level, mucous membranes, capillary refill time, and more.
- **Treatment and Diagnostics**: Covers information such as surgery, nasogastric tube use, and abdominocentesis.
- **Outcome**: The dataset records whether the horse lived, died, or was euthanized.

Additionally, lesion types, locations, and whether surgery was performed are included.

## Insights

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

