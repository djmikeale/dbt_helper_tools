# dbt YAML Cleaner

## Overview

The dbt YAML cleaner is a Python-based tool designed to standardize and clean up YAML files commonly used in dbt (data build tool) projects. It helps ensure consistency and readability by applying specific formatting rules to YAML files within a dbt project.

## Purpose

YAML files in dbt projects can vary. This tool provides a solution to standardize and clean up these YAML files, ensuring a consistent formatting style throughout the project.

## Features

- **Quoting Style Standardization**: The tool enforces a consistent quoting style for strings containing Jinja expressions, converting them to a preferred format.
- **Readability Enhancement**: By standardizing the formatting of YAML files, it improves readability and reduces inconsistencies within the dbt project.
- **Customization**: Users can tailor the tool to meet specific formatting requirements by adjusting the included rules and customization options.

## Usage

1. **Installation with bash/zsh**:

```shell
git clone https://github.com/djmikeale/dbt_yaml_cleaner.git
cd dbt_yaml_cleaner
python3 -m venv venv
source venv/bin/activate
python3 -m pip install --upgrade pip
python3 -m pip install -r requirements.txt
```


   - Install the required dependencies using `pip install -r requirements.txt`.

2. **Execution**:
   - Modify `yaml_cleanup.ipynb` to the directory containing your dbt project and run the notebook

## Contributions

Contributions and suggestions for improvements are welcome! Feel free to open an issue or submit a pull request to enhance the tool's functionality or documentation.

## License

This project is licensed under the [GPL-3.0 license](LICENSE).
