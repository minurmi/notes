# Algorithm testing

- Show that data recorded with different devices can be used for Aino medical
- Show that the algorithm on the wrist device produces the wanted output (same as on PC)
- Dataset should represent the expected use of the device
    + Different activities
    + Synthetic dataset

# TODO
1. Add arrhythmia output (IBI, SQE, ADL data) to the 'Algorithm tests'
2. Remove unused output form the 'Algorithm tests'
3. Integrate test code from Serj to the main codebase
    - Workshop to inform others about the tests
4. Create a dataset of synthetic data
    - a separate meeting to define the dataset
    - a sinusoid to test the perfect case
    - no false positives from noise
4. Select a representative dataset from recordings for automated testing
    - classify it into different activities

