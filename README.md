# Historical-Data-Transformation

The purpose of this Jupyter notebook is to convert employee data from a columnar format to a row-based versioning format that is historical and appropriate for database storage. Employee pay, engagement, and performance reviews are all included in the CSV input data that is transformed into a structured format that represents historical records during the transformation process.

1. **Loading the Data**: The input CSV file is loaded into a Pandas DataFrame for processing.I've also renamed the input scv file from input-input.csv to input.csv for better readability.

2. **Function of Data Transformation**: To carry out the transformation procedure, the core function transform_data is defined. This function builds rows with consistent data for each time by iterating through each row of the input DataFrame and extracting pertinent data.

3. **Effective and End Dates**: These are determined for every historical record by applying the prescribed rules. To prevent overlap, the termination date is set to one day prior to the next effective date. The end date for an employee's most recent record is set to a far-off date (like 2100-01-01).

4. **Output Creation**: The function generates a row for each record including the necessary fields in the preferred format, such as dates, employee identifiers, pay, performance evaluations, and engagement scores.

5. **Saving the Output**: The modified DataFrame is stored for further examination and keeping in a fresh CSV file.

6. **Displaying the Transformed Data**: To confirm the accuracy of the transformation procedure, the script prints the transformed DataFrame.
