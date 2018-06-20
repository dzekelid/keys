---
swagger: "2.0"
x-collection-name: Azure Machine Learning
x-complete: 1
info:
  title: Azure ML Web Services Management Client
  description: these-apis-allow-end-users-to-operate-on-azure-machine-learning-web-services-resources--they-support-the-following-operationsullicreate-or-update-a-web-serviceliliget-a-web-servicelilipatch-a-web-servicelilidelete-a-web-serviceliliget-all-web-services-in-a-resource-group-liliget-all-web-services-in-a-subscriptionliliget-web-services-keysliul
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MachineLearning/webServices/{webServiceName}/listKeys
  : get:
      summary: Web Services List Keys
      description: Gets the access keys for the specified web service.
      operationId: WebServices_ListKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-machinelearningwebserviceswebservicenamelistkeys-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Web Services Keys
---