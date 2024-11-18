ECG algorithm development
- jira taski
- design dokumentti
- desing change
- kelpoistus
    - yksikkötestit
    - datan esiprosessointi
      1. clinical study and pulseon demo system
      2. download dms data as csv
      3. parse csv with dms_patient_data_parser.py
      4. use script to pick 30s of long enough ECGs and run cardiolund 2.2.2
      5. use script to generate images of cardiolund results
      6. use script to classify images manually
      7. use script to run algorithm and produce results with different parameters
      8. pick best parameters
