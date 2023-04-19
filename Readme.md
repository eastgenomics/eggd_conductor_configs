# 🤖 eggd_conductor configs 🤖

The files contained in the `app_configs` and `assay_configs` folders are essential for the running of eggd_conductor.

## 🔧 App configs 🔧

The files in this repository are placeholders for the actual **app** config files stored in DNAnexus as those contain tokens.

Other than that, those files contain:

- `DEMULTIPLEX_APP_ID`
- `AUTH_TOKEN`
- `ASSAY_CONFIG_PATH`
- `SLACK_TOKEN`
- `SLACK_LOG_CHANNEL`
- `SLACK_ALERT_CHANNEL`
- `JIRA_EMAIL`
- `JIRA_TOKEN`
- `JIRA_QUEUE_URL`
- `JIRA_ISSUE_URL`

## 🔧 Assay configs 🔧

The assay config file for the conductor app is designed to be written as a JSON file, with each workflow or apps defined as an executable. For each workflow/app, there are several required and optional keys to add, with a required structure. Each assay requires its own assay config file to define all required executables and inputs, which are stored in DNAnexus under the `ASSAY_CONFIG_PATH` as defined in the app config file.

Full details on the assay config design and structure may be found [here](https://github.com/eastgenomics/eggd_conductor#assay-config-file).

For each assay config file, there is both an `assay_code` and `version` field in the top level of the config. The `assay_code` determines if to use the config file for the current samples by checking for presence of the code in sample names, and the `version` is parsed to keep the highest version of each config file for each assay (this should follow semantic versioning).

To update an assay config file, a new copy of the file should be created in the respective assays directory. When updating the config, both the verion number in the `version` field of the config **and** the filename should be incremented, and the changelog should have a brief description added for the new version as to the changes made:

i.e.
- current file:
  ```
  # assay_configs/CEN/eggd_conductor_dias_CEN_config_v1.0.0.json
  
  {
    "name": "Config for CEN assay",
    "assay": "CEN",
    "assay_code": "EGG5",
    "version": "1.0.0",
    "details": "Includes main Dias workflow, single, multi, QC and reports",
    "changelog": {
        "v1.0.0": "Initial working version"
    },
    "demultiplex": true,
    ...
  ```
 
- new file:
  ```
  # assay_configs/CEN/eggd_conductor_dias_CEN_config_v1.1.0.json
  
  {
    "name": "Config for CEN assay",
    "assay": "CEN",
    "assay_code": "EGG5",
    "version": "1.1.0",
    "details": "Includes main Dias workflow, single, multi, QC and reports",
    "changelog": {
        "v1.0.0": "Initial working version",
        "v1.1.0": "Details on changes for v1.1.0"
    },
    "demultiplex": true,
    ...
  ```
