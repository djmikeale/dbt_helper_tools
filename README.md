# Info

This repo contains helper tools for dbt.

1. Installation:

```shell
git clone https://github.com/djmikeale/dbt_helper_tools.git
cd dbt_helper_tools
python3 -m venv venv
source venv/bin/activate
python3 -m pip install --upgrade pip
python3 -m pip install -r requirements.txt
```

## Automated Model Renaming and File Update in dbt Projects

*Do you have a lot of legacy models that don't follow best naming practices?*

This script streamlines the process of updating model names and related files within a dbt (Data Build Tool) project.

- **Prefix Enforcement:** Identifies models in a specific layer that do not adhere to the intended prefix convention.
- **Model Renaming:** Automatically renames models to align with the latest best practices.
- **File Synchronization:** Updates the names and contents of corresponding `.yml` and `.md` files (if they exist).
- **Reference Management:** Adjusts references in downstream models to ensure they point to the newly renamed models.

### Important Considerations

- The script only processes `.yml` files, not `.yaml` files.
- It assumes `.yml` files share the same name and directory as their associated SQL files.
- Downstream models may still use old aliases, which aren't updated automatically. These instances will be flagged in the output for manual correction.

## dbt YAML Cleaner

### Overview

The dbt YAML cleaner is a Python-based tool designed to standardize and clean up YAML files commonly used in dbt (data build tool) projects. It helps ensure consistency and readability by applying specific formatting rules to YAML files within a dbt project.

### Purpose

YAML files in dbt projects can vary. This tool provides a solution to standardize and clean up these YAML files, ensuring a consistent formatting style throughout the project.

### Features

- **Quoting Style Standardization**: The tool enforces a consistent quoting style for strings containing Jinja expressions, converting them to a preferred format.
- **Readability Enhancement**: By standardizing the formatting of YAML files, it improves readability and reduces inconsistencies within the dbt project.
- **Customization**: Users can tailor the tool to meet specific formatting requirements by adjusting the included rules and customization options.

### Usage

1. Install the required dependencies using `pip install -r requirements.txt`.
2. Modify `yaml_cleanup.ipynb` to the directory containing your dbt project and run the notebook

## Contributions

Contributions and suggestions for improvements are welcome! Feel free to open an issue or submit a pull request to enhance the tool's functionality or documentation.
