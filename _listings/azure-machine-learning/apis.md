---
name: Azure Machine Learning
x-slug: azure-machine-learning
description: Azure Machine Learning lets you easily design, test, operationalize,
  and manage predictive analytics solutions in the cloud. Azure Machine Learning was
  designed for applied machine learning. Use best-in-class algorithms and a simple
  drag-and-drop interface&mdash;and go from idea to deployment in a matter of clicks.
  Try it free. If youre a developer who wants the data science built in, check out
  our APIs and Azure Marketplace.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-simple-scalable-cutting-edge.jpg
x-kinRank: "10"
x-alexaRank: "0"
tags: Keys
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-machine-learning/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Machine Learning API Web Services List Keys
  x-api-slug: azure-machine-learning-api
  description: Gets the access keys for the specified web service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-simple-scalable-cutting-edge.jpg
  humanURL: https://azure.microsoft.com/en-us/services/machine-learning/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MachineLearning/webServices/{webServiceName}/listKeys
  tags: Machine Learning,Web Services Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-machine-learning/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-machinelearningwebserviceswebservicenamelistkeys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-machine-learning/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-machinelearningwebserviceswebservicenamelistkeys-get-openapi.md
- name: Azure Machine Learning API
  x-api-slug: azure-machine-learning-api
  description: Azure Machine Learning lets you easily design, test, operationalize,
    and manage predictive analytics solutions in the cloud. Azure Machine Learning
    was designed for applied machine learning. Use best-in-class algorithms and a
    simple drag-and-drop interface&mdash;and go from idea to deployment in a matter
    of clicks. Try it free. If youre a developer who wants the data science built
    in, check out our APIs and Azure Marketplace.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-simple-scalable-cutting-edge.jpg
  humanURL: https://azure.microsoft.com/en-us/services/machine-learning/
  baseURL: ://management.azure.com//
  tags: Keys
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/keys/master/_listings/azure-machine-learning/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/machine-learning/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/machine-learning/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/machine-learning/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/machine-learning/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---