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

Each assay requires a config file to work with eggd_conductor. They are stored in folders named after the assay that they work with. Those will mainly specify:

- workflows/apps
  - name
  - version
  - arguments for use in eggd_conductor
- inputs of said workflows/apps
- links between outputs of the stages and inputs of subsequent stages

Additionally, details about the config file itself are stored such as version, assay or allowed users.

Full details on the assay config design and structure may be found [here](https://github.com/eastgenomics/eggd_conductor#assay-config-file).
