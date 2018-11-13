# helm.template

To create a new helm chart:

1. Install Heml (if you don't have it) from: https://docs.helm.sh/using_helm/#installing-helm
2. Copy this repo
3. Replace "replaceme" with name of your package
4. Run create.ps1 (this will generate a nested folder with the name of your package)
5. Go to templates folder and delete these files: deployment.yaml, ingress.yaml and service.yaml
6. Clear out the contents of NOTES.txt
7. Create folders for each type of resource: ingress, services, pods etc (Not mandatory but recommended)
8. Put your kubernetes yaml files in the appropriate folder
9. Go to Chart.yaml and update the description and the version
10. Run build.ps1 to build and create the tar files


Installing the chart

Just call helm install with the full path to your chart (tar file) on github (or any other web location)