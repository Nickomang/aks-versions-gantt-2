# AKS Kubernetes Versions Mermaid Gantt Chart

The [Microsoft Learn](https://learn.microsoft.com/) site does not support live
rendering of Mermaid charts, and so charts must be generated as images, hosted
in the Learn repository as an image, and inserted into the relevant page as an
image.

The downside to this is that some elements of a Mermaid chart can be dynamic, 
for example the "today" line on Mermaid Gantt charts. If we generate the chart
as an image file, the "today" line will be stuck on the day we generated the
image, which will be misleading or confusing for readers.

The solution, while the Learn site does not support live rendering of Mermaid
charts, is to generate a new image every day, with the correct "today" line, and
then either push the new image into the Learn repository, or update the relevant
Learn page(s) to reference the updated image.

This repository auto-builds a new version of the "Supported Kubernetes versions 
in Azure Kubernetes Service (AKS)" Gantt chart, as seen [here](https://learn.microsoft.com/en-us/azure/aks/supported-kubernetes-versions?tabs=azure-cli#aks-kubernetes-release-schedule-gantt-chart)
