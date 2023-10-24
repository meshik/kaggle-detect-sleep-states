Collaboration to detect sleep states with accelerometor data

## File Descriptions and Usage
### 1. `train_series.parquet`:
- **Description**: This file contains the training data where each series represents continuous accelerometer recordings for a single subject over multiple days.
- **Usage**:
  - Load this data to train your models.
  - Split a portion of this data as a validation set to evaluate your model's performance during development.

### 2. `test_series.parquet`:
- **Description**: This file contains the test data formatted similarly to the training data but for a different set of subjects.
- **Usage**:
  - Use this data to evaluate your models in the competition.
  - Make predictions on this data for submission to Kaggle.

### 3. `train_events.csv`:
- **Description**: This file contains the annotated sleep logs for the training set, recording the onset and wake-up events.
- **Usage**:
  - Use this data as ground truth labels to train your models.
  - Evaluate the performance of your models using a portion of this data as a validation set.

### 4. `sample_submission.csv`:
- **Description**: This file is a template showing how your submission should be formatted.
- **Usage**:
  - Refer to this file to understand the format in which your predictions should be submitted to Kaggle.
  - Prepare your submission file accordingly to ensure it complies with the competition's submission requirements.

### General Workflow:
1. Load `train_series.parquet` and `train_events.csv` to train your models.
2. Split a portion of `train_series.parquet` and `train_events.csv` as a validation set to evaluate your model's performance.
3. Once satisfied with your model's performance, load `test_series.parquet` to make predictions.
4. Format your predictions according to `sample_submission.csv` and submit to Kaggle.
