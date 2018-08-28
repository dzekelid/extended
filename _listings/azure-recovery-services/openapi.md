---
swagger: "2.0"
x-collection-name: Azure Recovery Services
x-complete: 1
info:
  title: RecoveryServicesClient
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
---