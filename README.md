## Automatic Non-Intrusive WiFi-Based Framework for Depression classification in Older Adults Using Machine Learning

This repository contains the code and resources for a novel machine learning model designed to classify depression in older adults using a non-intrusive WiFi-based motion sensor. The model is part of a feasibility study that aims to explore remote physical activity monitoring and its effectiveness in early frailty detection.

## Background

Depression is a prevalent mental health disorder characterized by persistent sadness and a loss of interest in daily activities, significantly diminishing an individual's quality of life. Early detection of depressive symptoms are critical for effective treatment and timely intervention. Numerous studies have explored the use of wearable devices to differentiate between individuals with and without depression based on their physical activity data; however, these methods often involve intrusive or semi-intrusive techniques. Furthermore, current depression classification studies are typically conducted on a relatively large number of participants and use single-stage classifiers without any explainability analysis.

## Objective

In this study, we aim to assess the feasibility of classifying depression using non-intrusive WiFi-based motion sensor data, employing a novel machine learning model on a limited number of participants. We also conduct an explainability analysis to interpret the model's predictions and identify key features associated with depression classification.

## Methodology

### Data Collection

- **Participants:** The study involved four older adult participants from Montreal, Quebec, Canada. The participants were aged 65 and above, with two identified as non-frail and two as potentially frail.
- **Data Sources:** Data were collected using WiFi signals over six months to monitor contextual human activity and sleep-related patterns. Additionally, participants completed the Edmonton Frailty Scale (EFS) and Geriatric Depression Scale (GDS) questionnaires.

### Model Architecture

The proposed model employs a three-stage architecture:

1. **Feature Selection:** Sequential Forward Selection (SFS) is used to identify the most relevant features.
2. **Dimensionality Reduction:** Principal Component Analysis (PCA) reduces the dimensionality of the selected features.
3. **Classification:** Decision Tree (DT) classifies participants into non-frail and potentially frail categories.

The model was evaluated using various combinations of techniques for each stage, and the best-performing combination was selected.

## Results

The model demonstrated high classification performance with the following metrics:

- **Accuracy:** 87.50%
- **Sensitivity:** 90.00%
- **Precision:** 88.34%

The model successfully identified key features related to sleep interruptions that have a strong correlation with depression.

