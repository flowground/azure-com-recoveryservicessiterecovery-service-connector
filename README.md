# ![LOGO](logo.png) SiteRecoveryManagementClient **flow**ground Connector

## Description

A generated **flow**ground connector for the SiteRecoveryManagementClient API (version 2018-07-10).

Generated from: https://api.apis.guru/v2/specs/azure.com/recoveryservicessiterecovery-service/2018-07-10/swagger.json<br/>
Generated at: 2019-05-07T17:38:42+03:00

## API Description



## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Returns the list of available operations.

> Operation to return the list of available operations.

*Tags:* `Operations`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.

### Gets the list of configured email notification(alert) configurations.

> Gets the list of email notification(alert) configurations for the vault.

*Tags:* `ReplicationAlertSettings`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.

### Gets an email notification(alert) configuration.

> Gets the details of the specified email notification(alert) configuration.

*Tags:* `ReplicationAlertSettings`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `alertSettingName` - _required_ - The name of the email notification configuration.

### Configures email notifications for this vault.

> Create or update an email notification(alert) configuration.

*Tags:* `ReplicationAlertSettings`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `alertSettingName` - _required_ - The name of the email notification(alert) configuration.

### Gets the list of Azure Site Recovery events.

> Gets the list of Azure Site Recovery events for the vault.

*Tags:* `ReplicationEvents`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `$filter` - _optional_ - OData filter options.

### Get the details of an Azure Site recovery event.

> The operation to get the details of an Azure Site recovery event.

*Tags:* `ReplicationEvents`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `eventName` - _required_ - The name of the Azure Site Recovery event.

### Gets the list of ASR fabrics

> Gets a list of the Azure Site Recovery fabrics in the vault.

*Tags:* `ReplicationFabrics`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.

### Purges the site.

> The operation to purge(force delete) an Azure Site Recovery fabric.

*Tags:* `ReplicationFabrics`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - ASR fabric to purge.

### Gets the details of an ASR fabric.

> Gets the details of an Azure Site Recovery fabric.

*Tags:* `ReplicationFabrics`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.

### Creates an Azure Site Recovery fabric.

> The operation to create an Azure Site Recovery fabric (for e.g. Hyper-V site)

*Tags:* `ReplicationFabrics`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Name of the ASR fabric.

### Checks the consistency of the ASR fabric.

> The operation to perform a consistency check on the fabric.

*Tags:* `ReplicationFabrics`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.

### Migrates the site to AAD.

> The operation to migrate an Azure Site Recovery fabric to AAD.

*Tags:* `ReplicationFabrics`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - ASR fabric to migrate.

### Perform failover of the process server.

> The operation to move replications from a process server to another process server.

*Tags:* `ReplicationFabrics`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - The name of the fabric containing the process server.

### Deletes the site.

> The operation to delete or remove an Azure Site Recovery fabric.

*Tags:* `ReplicationFabrics`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - ASR fabric to delete

### Renews certificate for the fabric.

> Renews the connection certificate for the ASR replication fabric.

*Tags:* `ReplicationFabrics`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - fabric name to renew certs for.

### Gets the list of logical networks under a fabric.

> Lists all the logical networks of the Azure Site Recovery fabric

*Tags:* `ReplicationLogicalNetworks`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Server Id.

### Gets a logical network with specified server id and logical network name.

> Gets the details of a logical network.

*Tags:* `ReplicationLogicalNetworks`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Server Id.
* `logicalNetworkName` - _required_ - Logical network name.

### Gets the list of networks under a fabric.

> Lists the networks available for a fabric.

*Tags:* `ReplicationNetworks`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name

### Gets a network with specified server id and network name.

> Gets the details of a network.

*Tags:* `ReplicationNetworks`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Server Id.
* `networkName` - _required_ - Primary network name.

### Gets all the network mappings under a network.

> Lists all ASR network mappings for the specified network.

*Tags:* `ReplicationNetworkMappings`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Primary fabric name.
* `networkName` - _required_ - Primary network name.

### Delete network mapping.

> The operation to delete a network mapping.

*Tags:* `ReplicationNetworkMappings`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Primary fabric name.
* `networkName` - _required_ - Primary network name.
* `networkMappingName` - _required_ - ARM Resource Name for network mapping.

### Gets network mapping by name.

> Gets the details of an ASR network mapping

*Tags:* `ReplicationNetworkMappings`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Primary fabric name.
* `networkName` - _required_ - Primary network name.
* `networkMappingName` - _required_ - Network mapping name.

### Updates network mapping.

> The operation to update an ASR network mapping.

*Tags:* `ReplicationNetworkMappings`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Primary fabric name.
* `networkName` - _required_ - Primary network name.
* `networkMappingName` - _required_ - Network mapping name.

### Creates network mapping.

> The operation to create an ASR network mapping.

*Tags:* `ReplicationNetworkMappings`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Primary fabric name.
* `networkName` - _required_ - Primary network name.
* `networkMappingName` - _required_ - Network mapping name.

### Gets the list of protection container for a fabric.

> Lists the protection containers in the specified fabric.

*Tags:* `ReplicationProtectionContainers`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.

### Gets the protection container details.

> Gets the details of a protection container.

*Tags:* `ReplicationProtectionContainers`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `protectionContainerName` - _required_ - Protection container name.

### Create a protection container.

> Operation to create a protection container.

*Tags:* `ReplicationProtectionContainers`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Unique fabric ARM name.
* `protectionContainerName` - _required_ - Unique protection container ARM name.

### Adds a protectable item to the replication protection container.

> The operation to a add a protectable item to a protection container(Add physical server.)

*Tags:* `ReplicationProtectionContainers`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - The name of the fabric.
* `protectionContainerName` - _required_ - The name of the protection container.

### Removes a protection container.

> Operation to remove a protection container.

*Tags:* `ReplicationProtectionContainers`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Unique fabric ARM name.
* `protectionContainerName` - _required_ - Unique protection container ARM name.

### Gets the list of migration items in the protection container.

> Gets the list of ASR migration items in the protection container.

*Tags:* `ReplicationMigrationItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `protectionContainerName` - _required_ - Protection container name.

### Delete the migration item.

> The operation to delete an ASR migration item.

*Tags:* `ReplicationMigrationItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `migrationItemName` - _required_ - Migration item name.
* `deleteOption` - _optional_ - The delete option.

### Gets the details of a migration item.

*Tags:* `ReplicationMigrationItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric unique name.
* `protectionContainerName` - _required_ - Protection container name.
* `migrationItemName` - _required_ - Migration item name.

### Updates migration item.

> The operation to update the recovery settings of an ASR migration item.

*Tags:* `ReplicationMigrationItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `migrationItemName` - _required_ - Migration item name.

### Enables migration.

> The operation to create an ASR migration item (enable migration).

*Tags:* `ReplicationMigrationItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `migrationItemName` - _required_ - Migration item name.

### Migrate item.

> The operation to initiate migration of the item.

*Tags:* `ReplicationMigrationItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `migrationItemName` - _required_ - Migration item name.

### Gets the recovery points for a migration item.

*Tags:* `MigrationRecoveryPoints`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric unique name.
* `protectionContainerName` - _required_ - Protection container name.
* `migrationItemName` - _required_ - Migration item name.

### Gets a recovery point for a migration item.

*Tags:* `MigrationRecoveryPoints`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric unique name.
* `protectionContainerName` - _required_ - Protection container name.
* `migrationItemName` - _required_ - Migration item name.
* `migrationRecoveryPointName` - _required_ - The migration recovery point name.

### Test migrate item.

> The operation to initiate test migration of the item.

*Tags:* `ReplicationMigrationItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `migrationItemName` - _required_ - Migration item name.

### Test migrate cleanup.

> The operation to initiate test migrate cleanup.

*Tags:* `ReplicationMigrationItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `migrationItemName` - _required_ - Migration item name.

### Gets the list of protectable items.

> Lists the protectable items in a protection container.

*Tags:* `ReplicationProtectableItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `$filter` - _optional_ - OData filter options.

### Gets the details of a protectable item.

> The operation to get the details of a protectable item.

*Tags:* `ReplicationProtectableItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `protectableItemName` - _required_ - Protectable item name.

### Gets the list of Replication protected items.

> Gets the list of ASR replication protected items in the protection container.

*Tags:* `ReplicationProtectedItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `protectionContainerName` - _required_ - Protection container name.

### Purges protection.

> The operation to delete or purge a replication protected item. This operation will force delete the replication protected item. Use the remove operation on replication protected item to perform a clean disable replication for the item.

*Tags:* `ReplicationProtectedItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `replicatedProtectedItemName` - _required_ - Replication protected item name.

### Gets the details of a Replication protected item.

> Gets the details of an ASR replication protected item.

*Tags:* `ReplicationProtectedItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric unique name.
* `protectionContainerName` - _required_ - Protection container name.
* `replicatedProtectedItemName` - _required_ - Replication protected item name.

### Updates protection.

> The operation to update the recovery settings of an ASR replication protected item.

*Tags:* `ReplicationProtectedItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `replicatedProtectedItemName` - _required_ - Replication protected item name.

### Enables protection.

> The operation to create an ASR replication protected item (Enable replication).

*Tags:* `ReplicationProtectedItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Name of the fabric.
* `protectionContainerName` - _required_ - Protection container name.
* `replicatedProtectedItemName` - _required_ - A name for the replication protected item.

### Resolve health errors.

> Operation to resolve health issues of the replication protected item.

*Tags:* `ReplicationProtectedItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Unique fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `replicatedProtectedItemName` - _required_ - Replication protected item name.

### Add disk(s) for protection.

> Operation to add disks(s) to the replication protected item.

*Tags:* `ReplicationProtectedItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Unique fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `replicatedProtectedItemName` - _required_ - Replication protected item name.

### Change or apply recovery point.

> The operation to change the recovery point of a failed over replication protected item.

*Tags:* `ReplicationProtectedItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - The ARM fabric name.
* `protectionContainerName` - _required_ - The protection container name.
* `replicatedProtectedItemName` - _required_ - The replicated protected item's name.

### Execute commit failover

> Operation to commit the failover of the replication protected item.

*Tags:* `ReplicationProtectedItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Unique fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `replicatedProtectedItemName` - _required_ - Replication protected item name.

### Execute planned failover

> Operation to initiate a planned failover of the replication protected item.

*Tags:* `ReplicationProtectedItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Unique fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `replicatedProtectedItemName` - _required_ - Replication protected item name.

### Execute Reverse Replication\Reprotect

> Operation to reprotect or reverse replicate a failed over replication protected item.

*Tags:* `ReplicationProtectedItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Unique fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `replicatedProtectedItemName` - _required_ - Replication protected item name.

### Get recovery points for a replication protected item.

> Lists the available recovery points for a replication protected item.

*Tags:* `RecoveryPoints`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - The fabric name.
* `protectionContainerName` - _required_ - The protection container name.
* `replicatedProtectedItemName` - _required_ - The replication protected item's name.

### Get a recovery point.

> Get the details of specified recovery point.

*Tags:* `RecoveryPoints`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - The fabric name.
* `protectionContainerName` - _required_ - The protection container name.
* `replicatedProtectedItemName` - _required_ - The replication protected item's name.
* `recoveryPointName` - _required_ - The recovery point name.

### Disables protection.

> The operation to disable replication on a replication protected item. This will also remove the item.

*Tags:* `ReplicationProtectedItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `replicatedProtectedItemName` - _required_ - Replication protected item name.

### Removes disk(s).

> Operation to remove disk(s) from the replication protected item.

*Tags:* `ReplicationProtectedItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Unique fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `replicatedProtectedItemName` - _required_ - Replication protected item name.

### Resynchronize or repair replication.

> The operation to start resynchronize/repair replication for a replication protected item requiring resynchronization.

*Tags:* `ReplicationProtectedItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - The name of the fabric.
* `protectionContainerName` - _required_ - The name of the container.
* `replicatedProtectedItemName` - _required_ - The name of the replication protected item.

### Gets the list of target compute sizes for the replication protected item.

> Lists the available target compute sizes for a replication protected item.

*Tags:* `TargetComputeSizes`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `protectionContainerName` - _required_ - protection container name.
* `replicatedProtectedItemName` - _required_ - Replication protected item name.

### Execute test failover

> Operation to perform a test failover of the replication protected item.

*Tags:* `ReplicationProtectedItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Unique fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `replicatedProtectedItemName` - _required_ - Replication protected item name.

### Execute test failover cleanup.

> Operation to clean up the test failover of a replication protected item.

*Tags:* `ReplicationProtectedItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Unique fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `replicatedProtectedItemName` - _required_ - Replication protected item name.

### Execute unplanned failover

> Operation to initiate a failover of the replication protected item.

*Tags:* `ReplicationProtectedItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Unique fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `replicatedProtectedItemName` - _required_ - Replication protected item name.

### Update the mobility service on a protected item.

> The operation to update(push update) the installed mobility service software on a replication protected item to the latest available version.

*Tags:* `ReplicationProtectedItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - The name of the fabric containing the protected item.
* `protectionContainerName` - _required_ - The name of the container containing the protected item.
* `replicationProtectedItemName` - _required_ - The name of the protected item on which the agent is to be updated.

### Gets the list of protection container mappings for a protection container.

> Lists the protection container mappings for a protection container.

*Tags:* `ReplicationProtectionContainerMappings`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `protectionContainerName` - _required_ - Protection container name.

### Purge protection container mapping.

> The operation to purge(force delete) a protection container mapping

*Tags:* `ReplicationProtectionContainerMappings`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `mappingName` - _required_ - Protection container mapping name.

### Gets a protection container mapping/

> Gets the details of a protection container mapping.

*Tags:* `ReplicationProtectionContainerMappings`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `mappingName` - _required_ - Protection Container mapping name.

### Update protection container mapping.

> The operation to update protection container mapping.

*Tags:* `ReplicationProtectionContainerMappings`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `mappingName` - _required_ - Protection container mapping name.

### Create protection container mapping.

> The operation to create a protection container mapping.

*Tags:* `ReplicationProtectionContainerMappings`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `mappingName` - _required_ - Protection container mapping name.

### Remove protection container mapping.

> The operation to delete or remove a protection container mapping.

*Tags:* `ReplicationProtectionContainerMappings`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `protectionContainerName` - _required_ - Protection container name.
* `mappingName` - _required_ - Protection container mapping name.

### Switches protection from one container to another or one replication provider to another.

> Operation to switch protection from one container to another or one replication provider to another.

*Tags:* `ReplicationProtectionContainers`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Unique fabric name.
* `protectionContainerName` - _required_ - Protection container name.

### Gets the list of registered recovery services providers for the fabric.

> Lists the registered recovery services providers for the specified fabric.

*Tags:* `ReplicationRecoveryServicesProviders`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name

### Purges recovery service provider from fabric

> The operation to purge(force delete) a recovery services provider from the vault.

*Tags:* `ReplicationRecoveryServicesProviders`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `providerName` - _required_ - Recovery services provider name.

### Gets the details of a recovery services provider.

> Gets the details of registered recovery services provider.

*Tags:* `ReplicationRecoveryServicesProviders`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `providerName` - _required_ - Recovery services provider name

### Adds a recovery services provider.

> The operation to add a recovery services provider.

*Tags:* `ReplicationRecoveryServicesProviders`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `providerName` - _required_ - Recovery services provider name.

### Refresh details from the recovery services provider.

> The operation to refresh the information from the recovery services provider.

*Tags:* `ReplicationRecoveryServicesProviders`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `providerName` - _required_ - Recovery services provider name.

### Deletes provider from fabric. Note: Deleting provider for any fabric other than SingleHost is unsupported. To maintain backward compatibility for released clients the object "deleteRspInput" is used (if the object is empty we assume that it is old client and continue the old behavior).

> The operation to removes/delete(unregister) a recovery services provider from the vault

*Tags:* `ReplicationRecoveryServicesProviders`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `providerName` - _required_ - Recovery services provider name.

### Gets the list of storage classification objects under a fabric.

> Lists the storage classifications available in the specified fabric.

*Tags:* `ReplicationStorageClassifications`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Site name of interest.

### Gets the details of a storage classification.

> Gets the details of the specified storage classification.

*Tags:* `ReplicationStorageClassifications`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `storageClassificationName` - _required_ - Storage classification name.

### Gets the list of storage classification mappings objects under a storage.

> Lists the storage classification mappings for the fabric.

*Tags:* `ReplicationStorageClassificationMappings`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `storageClassificationName` - _required_ - Storage classification name.

### Delete a storage classification mapping.

> The operation to delete a storage classification mapping.

*Tags:* `ReplicationStorageClassificationMappings`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `storageClassificationName` - _required_ - Storage classification name.
* `storageClassificationMappingName` - _required_ - Storage classification mapping name.

### Gets the details of a storage classification mapping.

> Gets the details of the specified storage classification mapping.

*Tags:* `ReplicationStorageClassificationMappings`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `storageClassificationName` - _required_ - Storage classification name.
* `storageClassificationMappingName` - _required_ - Storage classification mapping name.

### Create storage classification mapping.

> The operation to create a storage classification mapping.

*Tags:* `ReplicationStorageClassificationMappings`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `storageClassificationName` - _required_ - Storage classification name.
* `storageClassificationMappingName` - _required_ - Storage classification mapping name.

### Gets the list of vCenter registered under a fabric.

> Lists the vCenter servers registered in a fabric.

*Tags:* `ReplicationvCenters`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.

### Remove vCenter operation.

> The operation to remove(unregister) a registered vCenter server from the vault.

*Tags:* `ReplicationvCenters`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `vCenterName` - _required_ - vCenter name.

### Gets the details of a vCenter.

> Gets the details of a registered vCenter server(Add vCenter server.)

*Tags:* `ReplicationvCenters`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `vCenterName` - _required_ - vCenter name.

### Update vCenter operation.

> The operation to update a registered vCenter.

*Tags:* `ReplicationvCenters`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `vCenterName` - _required_ - vCenter name

### Add vCenter.

> The operation to create a vCenter object..

*Tags:* `ReplicationvCenters`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `fabricName` - _required_ - Fabric name.
* `vCenterName` - _required_ - vCenter name.

### Gets the list of jobs.

> Gets the list of Azure Site Recovery Jobs for the vault.

*Tags:* `ReplicationJobs`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `$filter` - _optional_ - OData filter options.

### Exports the details of the Azure Site Recovery jobs of the vault.

> The operation to export the details of the Azure Site Recovery jobs of the vault.

*Tags:* `ReplicationJobs`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.

### Gets the job details.

> Get the details of an Azure Site Recovery job.

*Tags:* `ReplicationJobs`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `jobName` - _required_ - Job identifier

### Cancels the specified job.

> The operation to cancel an Azure Site Recovery job.

*Tags:* `ReplicationJobs`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `jobName` - _required_ - Job identifier.

### Restarts the specified job.

> The operation to restart an Azure Site Recovery job.

*Tags:* `ReplicationJobs`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `jobName` - _required_ - Job identifier.

### Resumes the specified job.

> The operation to resume an Azure Site Recovery job

*Tags:* `ReplicationJobs`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `jobName` - _required_ - Job identifier.

### Gets the list of migration items in the vault.

*Tags:* `ReplicationMigrationItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `skipToken` - _optional_ - The pagination token.
* `$filter` - _optional_ - OData filter options.

### Gets all the network mappings under a vault.

> Lists all ASR network mappings in the vault.

*Tags:* `ReplicationNetworkMappings`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.

### Gets the list of networks. View-only API.

> Lists the networks available in a vault

*Tags:* `ReplicationNetworks`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.

### Gets the list of replication policies

> Lists the replication policies for a vault.

*Tags:* `ReplicationPolicies`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.

### Delete the policy.

> The operation to delete a replication policy.

*Tags:* `ReplicationPolicies`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `policyName` - _required_ - Replication policy name.

### Gets the requested policy.

> Gets the details of a replication policy.

*Tags:* `ReplicationPolicies`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `policyName` - _required_ - Replication policy name.

### Updates the policy.

> The operation to update a replication policy.

*Tags:* `ReplicationPolicies`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `policyName` - _required_ - Policy Id.

### Creates the policy.

> The operation to create a replication policy

*Tags:* `ReplicationPolicies`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `policyName` - _required_ - Replication policy name

### Gets the list of replication protected items.

> Gets the list of ASR replication protected items in the vault.

*Tags:* `ReplicationProtectedItems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `skipToken` - _optional_ - The pagination token. Possible values: "FabricId" or "FabricId_CloudId" or null
* `$filter` - _optional_ - OData filter options.

### Gets the list of all protection container mappings in a vault.

> Lists the protection container mappings in the vault.

*Tags:* `ReplicationProtectionContainerMappings`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.

### Gets the list of all protection containers in a vault.

> Lists the protection containers in a vault.

*Tags:* `ReplicationProtectionContainers`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.

### Gets the list of recovery plans.

> Lists the recovery plans in the vault.

*Tags:* `ReplicationRecoveryPlans`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.

### Deletes the specified recovery plan.

> Delete a recovery plan.

*Tags:* `ReplicationRecoveryPlans`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `recoveryPlanName` - _required_ - Recovery plan name.

### Gets the requested recovery plan.

> Gets the details of the recovery plan.

*Tags:* `ReplicationRecoveryPlans`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `recoveryPlanName` - _required_ - Name of the recovery plan.

### Updates the given recovery plan.

> The operation to update a recovery plan.

*Tags:* `ReplicationRecoveryPlans`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `recoveryPlanName` - _required_ - Recovery plan name.

### Creates a recovery plan with the given details.

> The operation to create a recovery plan.

*Tags:* `ReplicationRecoveryPlans`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `recoveryPlanName` - _required_ - Recovery plan name.

### Execute commit failover of the recovery plan.

> The operation to commit the fail over of a recovery plan.

*Tags:* `ReplicationRecoveryPlans`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `recoveryPlanName` - _required_ - Recovery plan name.

### Execute planned failover of the recovery plan.

> The operation to start the planned failover of a recovery plan.

*Tags:* `ReplicationRecoveryPlans`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `recoveryPlanName` - _required_ - Recovery plan name.

### Execute reprotect of the recovery plan.

> The operation to reprotect(reverse replicate) a recovery plan.

*Tags:* `ReplicationRecoveryPlans`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `recoveryPlanName` - _required_ - Recovery plan name.

### Execute test failover of the recovery plan.

> The operation to start the test failover of a recovery plan.

*Tags:* `ReplicationRecoveryPlans`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `recoveryPlanName` - _required_ - Recovery plan name.

### Execute test failover cleanup of the recovery plan.

> The operation to cleanup test failover of a recovery plan.

*Tags:* `ReplicationRecoveryPlans`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `recoveryPlanName` - _required_ - Recovery plan name.

### Execute unplanned failover of the recovery plan.

> The operation to start the failover of a recovery plan.

*Tags:* `ReplicationRecoveryPlans`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.
* `recoveryPlanName` - _required_ - Recovery plan name.

### Gets the list of registered recovery services providers in the vault. This is a view only api.

> Lists the registered recovery services providers in the vault

*Tags:* `ReplicationRecoveryServicesProviders`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.

### Gets the list of storage classification mappings objects under a vault.

> Lists the storage classification mappings in the vault.

*Tags:* `ReplicationStorageClassificationMappings`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.

### Gets the list of storage classification objects under a vault.

> Lists the storage classifications in the vault.

*Tags:* `ReplicationStorageClassifications`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.

### Gets the data of supported OSes by SRS.

*Tags:* `SupportedOperatingSystems`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.

### Gets the health summary for the vault.

> Gets the health details of the vault.

*Tags:* `ReplicationVaultHealth`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.

### Refreshes health summary of the vault.

*Tags:* `ReplicationVaultHealth`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.

### Gets the list of vCenter registered under the vault.

> Lists the vCenter servers registered in the vault.

*Tags:* `ReplicationvCenters`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `resourceName` - _required_ - The name of the recovery services vault.
* `resourceGroupName` - _required_ - The name of the resource group where the recovery services vault is present.
* `subscriptionId` - _required_ - The subscription Id.

## License

**flow**ground :- Telekom iPaaS / azure-com-recoveryservicessiterecovery-service-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
