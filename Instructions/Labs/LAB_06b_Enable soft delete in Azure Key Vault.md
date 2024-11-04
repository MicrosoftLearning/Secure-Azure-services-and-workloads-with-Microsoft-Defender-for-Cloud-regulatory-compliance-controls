---
lab:
    title: 'Exercise 06b - Enable soft delete in Azure Key Vault'    
    module: 'Module 07 - Configure Azure Key Vault networking settings'
---


>**Note**: To complete this lab, you will need an [Azure subscription.](https://azure.microsoft.com/en-us/free/?azure-portal=true) in which you have administrative access. 


Deleting a key vault without soft delete enabled permanently deletes all secrets, keys, and certificates stored in the key vault. Accidental deletion of a key vault can lead to permanent data loss. Soft delete allows you to recover an accidentally deleted key vault for a configurable retention period.

---

## Skilling tasks

- Verify if soft delete is enabled on a key vault and enable soft delete.

## Exercise instructions 

### Verify if soft delete is enabled on a key vault and enable soft delete

1. In the search box at the top of the portal, enter **Key vaults.** Select **Key vaults** in the search results.
   
2. Browse to the key vault you previously created.

3. From the **Settings** blade, select **Properties.**

4. Verify if the radio button next to soft-delete is set to **Enable purge protection (enforce a mandatory retention period for deleted vaults and vault objects).**

5. If soft-delete is not enabled on the key vault, click the **Enable purge protection (enforce a mandatory retention period for deleted vaults and vault objects)** radio button to enable soft delete and click **Save.**

![image](https://github.com/user-attachments/assets/b2d5380b-5625-40de-9df6-e1c512dec973)

> **Results**: You have successfully enabled soft delete, ensuring that deleted resources are retained for 90 days (by default) and can be recovered, effectively undoing the deletion through the Azure portal.
