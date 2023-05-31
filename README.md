# Helm Chart Repository - Groep2Rekeningrijden/charts

This Helm Chart repository, hosted
at [https://groep2rekeningrijden.github.io/charts/](https://groep2rekeningrijden.github.io/charts/), is dedicated to storing and
managing Helm charts for the school project Rekeningrijden.

## Description

[Rekeningrijden](https://dev.azure.com/FontysVerkeer/Rekeningrijden) is a road pricing platform developed as a school
project. Thisrepository serves as the central location to store and distribute Helm charts for Rekeningrijden. Helm
charts provide an efficient and reproducible way to package, deploy, and manage Kubernetes applications.

## Usage

To use this Helm Chart repository and access the available charts, follow these steps:

1. Add the repository to your Helm configuration:

   ```shell
   helm repo add rekeningrijden https://groep2rekeningrijden.github.io/charts/
   ```

2. Update the Helm repositories:

   ```shell
   helm repo update
   ```

3. Search for available charts:

   ```shell
   helm search repo rekeningrijden
   ```

4. Install a chart:

   ```shell
   helm install <release-name> rekeningrijden/<chart-name>
   ```

5. Customize the chart values by providing a `values.yaml` file or using the `--set` flag during installation.

6. Manage the deployed release using Helm commands like `helm upgrade`, `helm rollback`, or `helm uninstall`.

## Maintaining the Repository

To maintain this Helm Chart repository and add new charts, follow these steps:

1. Package your chart:

   ```shell
   helm package <chart-directory>
   ```

2. Index the repository:

   ```shell
   helm repo index --url https://groep2rekeningrijden.github.io/charts/ --merge index.yaml .
   ```

3. Commit and push the updated repository files:

   ```shell
   git add .
   git commit -m "Add new chart or update repository"
   git push
   ```

4. The chart will be available for others to use after the repository is updated.

## Issues and Contributions

If you encounter any issues with the charts or have suggestions for improvement, please open an issue on
the [GitHub repository](https://github.com/Groep2Rekeningrijden/charts). Contributions, such as bug fixes or new charts, are
highly welcome.
