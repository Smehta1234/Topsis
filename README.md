# thapar-102218071-topsis

## Description
\`thapar-102218071-topsis\` is a Python package that implements the **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution) method. This method is widely used for ranking and decision-making tasks. The package allows users to apply TOPSIS on datasets with multiple criteria, providing scores and ranks for each alternative.

## Installation
Install the package using pip:

\`\`\`bash
pip install thapar-102218071-topsis
\`\`\`

## Usage

You can use the package from the command line by running:

\`\`\`bash
python -m my_topsis_package.__main__ <InputDataFile> <Weights> <Impacts> <ResultFileName>
\`\`\`

### Example
\`\`\`bash
python -m my_topsis_package.__main__ 102218071.csv "1,1,1,1,1" "+,+,+,+,+" st.csv
\`\`\`

### Parameters
1. **InputDataFile**: The path to the CSV file containing the dataset.
2. **Weights**: A comma-separated string specifying the weights for each criterion (e.g., \`"1,1,1,1,1"\`).
3. **Impacts**: A comma-separated string of impacts (\`"+"\` for positive, \`"-"\` for negative) for each criterion.
4. **ResultFileName**: The name of the output file that will contain the results.

## Input File Format
The input CSV file should have the following structure:

| Alternative | Criterion 1 | Criterion 2 | Criterion 3 | Criterion 4 | Criterion 5 |
|-------------|-------------|-------------|-------------|-------------|-------------|
| A1          | 250         | 16          | 12          | 5           | 0.7         |
| A2          | 200         | 20          | 8           | 6           | 0.9         |
| A3          | 300         | 14          | 10          | 4           | 0.8         |

## Output File Format
The output CSV file will include the original data along with two additional columns:
1. **TOPSIS Score**: The calculated score for each alternative.
2. **Rank**: The ranking of each alternative based on the TOPSIS score.

Example output:

| Alternative | Criterion 1 | Criterion 2 | Criterion 3 | Criterion 4 | Criterion 5 | TOPSIS Score | Rank |
|-------------|-------------|-------------|-------------|-------------|-------------|--------------|------|
| A1          | 250         | 16          | 12          | 5           | 0.7         | 0.78         | 1    |
| A2          | 200         | 20          | 8           | 6           | 0.9         | 0.65         | 2    |
| A3          | 300         | 14          | 10          | 4           | 0.8         | 0.60         | 3    |

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
EOL

