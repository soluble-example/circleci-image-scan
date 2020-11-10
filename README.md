# example-image-scan

[![Soluble-OSS](https://circleci.com/gh/soluble-oss/example-image-scan/tree/main.svg?style=svg)](https://circleci.com/gh/soluble-oss/example-image-scan)

This simple example demonstrates:

1) Installing the soluble cli from within a Circle CI pipeline
2) Scanning a container image with trivy and uploading the results to Soluble Fusion

## Note

Two variables are set in the Circle CI context:

* `SOLUBLE_API_TOKEN`
* `SOLUBLE_ORG_ID`

When the following is run as part of the pipeline:

`curl -sL https://raw.githubusercontent.com/soluble-ai/soluble-cli/master/linux-install.sh | sh`

The installer configured `${HOME}/.soluble/cli-config.json` with the values from the environment.

