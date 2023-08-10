# `NrmlizAddSAl.py` README

## Overview

The `NrmlizAddSAl.py` script is a data cleaning and manipulation tool designed to process and refine multiple `.CSV` files within a directory. Its primary purpose is to generate 'Addressee' and 'Salutation' fields based on various conditions and logic. The header names need to be in the formatt of RE export i.e. ConsID/Constituent ID needs to be CnBio_ID 

## Features

- **CSV File Processing**: 
  - Automatically detects and processes all `.CSV` files in the script's directory.

- **Title Classification**: 
  - Utilizes predefined lists to classify titles into 'AllREtitles', 'specialTitle', and 'commonTitles'.

- **Data Cleaning**: 
  - Performs several data cleaning operations such as:
    * Replacing spaces with NaN values.
    * Removing duplicate rows based on the `CnBio_ID` column.

- **Dynamic Address and Salutation Generation**: 
  - Creates 'Addressee' and 'Salutation' fields based on the logic related to marital status, gender, and other data fields.

- **Output**: 
  - Saves the cleaned data to a new `.CSV` file with a "_clean" suffix to distinguish it from the original file.

## Usage

1. **Dependencies**: 
   - Before running the script, ensure you have the following Python libraries installed:
     * `glob`
     * `pandas`
     * `numpy`
     * `os`

2. **Running the Script**: 
   - Place the script in the directory containing the `.CSV` files you want to process and run the script. The cleaned files will be saved in the same directory with a "_clean" suffix.

3. **Configuration**: 
   - If you want to modify the logic or add new title classifications, adjust the lists at the beginning of the script.

## Notes

- The script contains several commented-out sections that could be previous approaches or alternative methods. Review and uncomment them if needed for your use case.
- Ensure you always back up your original data before running any data cleaning or manipulation scripts.

## License

This script is provided as-is without any warranties. Users are advised to review and test the script thoroughly before applying it to critical datasets.
