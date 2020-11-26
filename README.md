# @samret/azure-backup-job

Please be advised that the supervening code snippet will need to be utilized in order for this backup job to be successful.  Of course, you will need to modify accordingly with your unique credentials. If you find an issue with this code, please feel free to submit an issue.  I will be eternally grateful for the feedback.

## Prerequisites

1. Please ensure that you have the LTS version of NodeJS/NPM installed on your workstation.
2. You will need to run this command at the root of your project:

   ```javascript
    npm i @samret/azure-backup-job
   ```

## Code Snippet

```typescript
const azureBackupJob = require('@samret/azure-backup-job');

router.post('/api/v1/User/Replace/:originalUserId/:replacementUserId', azureBackupJob(), replaceUser]);

let options = { tenantName: process.env.TENANT_NAME,
    clientId: process.env.CLIENT_ID,
    clientSecret: process.env.CLIENT_SECRET,
    subscriptionId: process.env.subscriptionId,
    resourceGroupName: process.env.resourceGroupName,
    vaultName: process.env.vaultName,
    fabricName: process.env.fabricName,
    containerName: process.env.containerName,
    protectedItemName: process.env.protectedItemName,
    }
```
