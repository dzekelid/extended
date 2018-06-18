---
swagger: "2.0"
x-collection-name: Azure Recovery Services
x-complete: 0
info:
  title: Azure Recovery Service API Vault Extended Info Update
  version: 1.0.0
  description: Update vault extended info.
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/extendedInformation/vaultExtendedInfo
  : get:
      summary: Vault Extended Info Get
      description: Get the vault extended info.
      operationId: VaultExtendedInfo_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaultsvaultnameextendedinformationvaultextendedinfo-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Vault Extended Info
    put:
      summary: Vault Extended Info Create Or Update
      description: Create vault extended info.
      operationId: VaultExtendedInfo_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaultsvaultnameextendedinformationvaultextendedinfo-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: resourceResourceExtendedInfoDetails
        description: resourceResourceExtendedInfoDetails
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Vault Extended Info
    patch:
      summary: Vault Extended Info Update
      description: Update vault extended info.
      operationId: VaultExtendedInfo_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaultsvaultnameextendedinformationvaultextendedinfo-patch
      parameters:
      - in: query
        name: No Name
      - in: body
        name: resourceResourceExtendedInfoDetails
        description: resourceResourceExtendedInfoDetails
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Vault Extended Info
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---