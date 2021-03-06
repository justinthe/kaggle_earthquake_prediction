# kaggle_earthquake_prediction

The goal of this competition is to use seismic signals to predict the timing of laboratory earthquakes. The data comes from a well-known experimental set-up used to study earthquake physics. The acoustic_data input signal is used to predict the time remaining before the next laboratory earthquake (time_to_failure).

The training data is a single, continuous segment of experimental data. The test data consists of a folder containing many small segments. The data within each test file is continuous, but the test files do not represent a continuous segment of the experiment; thus, the predictions cannot be assumed to follow the same regular pattern seen in the training file.

For each seg_id in the test folder, you should predict a single time_to_failure corresponding to the time between the last row of the segment and the next laboratory earthquake.

## File descriptions
 * train.csv - A single, continuous training segment of experimental data.   
 * test - A folder containing many small segments of test data.   
 * sample_sumbission.csv - A sample submission file in the correct format.   

## Data fields
* acoustic_data - the seismic signal [int16]   
* time_to_failure - the time (in seconds) until the next laboratory earthquake [float64]   
* seg_id - the test segment ids for which predictions should be made (one prediction per segment)   
