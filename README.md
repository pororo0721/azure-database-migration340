# Project: Azure Database Migration
This project involves the architecture and implementation of a cloud-based database system on Microsoft Azure. It showcases hands-on expertise in cloud engineering, focusing on data management, disaster recovery, and security.

## Getting Started
To get started with this project, you'll need a Microsoft Azure account. Detailed instructions on setting up the environment and implementing the features will be provided in the subsequent sections.

## Prerequisites
- Microsoft Azure account
- Basic understanding of cloud engineering and database management

## Milestone 2: Set up the Production Environment

### Task 1: Provision a Windows Virtual Machine
- Provision a Windows VM in Azure.
- Configure the VM based on your requirements.

### Task 2: Connect to the Windows Virtual Machine
- Use Remote Desktop Protocol (RDP) to connect to the VM.
- Ensure your network settings allow RDP connections.

### Task 3: Install SQL Server and SSMS
- Download and install SQL Server on your VM.
- Download and install SQL Server Management Studio (SSMS).

### Task 4: Create the Production Database
- Use SSMS to create a new SQL Server database.
- Configure the database based on your requirements.

## Milestone 3: Migrate to Azure SQL Database

### Task 1: Set up Azure SQL Database
By configuring SQL login authentication and firewall rules, you ensure secure access to the database while leveraging Azure's cloud infrastructure for enhanced scalability and reliability.
### Task 2: Prepare for Migration
### Task 3: Connect to Azure SQL Database
### Task 4: Schema Migration
### Task 5: Data Migration

## Milestone 4: Data Backup and Restore

### Task 1: Backup the On-Premise Database
1. Connect to SQL Server: Ensure you are connected to the SQL Server instance hosting the production database using SQL Server Management Studio (SSMS) or another preferred client tool.

2. Launch Backup Wizard: Right-click on the database you wish to backup in the Object Explorer pane of SSMS. Select "Tasks" > "Back Up..." to launch the Backup Database Wizard.

3. Select Backup Type: In the Backup Database Wizard, ensure that "Full" is selected as the backup type. This ensures a complete backup of the database.

4. Specify Backup Destination: Choose the destination for the backup. You can either backup to disk, tape, or a backup device. For this procedure, we'll backup to disk.

5. Define Backup Options: Specify the options for the backup, including backup set name, description, and whether to verify the backup when finished. Additionally, you can choose to perform a compression if desired.

6. Execute Backup: Review the backup options and click "OK" to execute the backup operation. Monitor the progress in the Backup and Restore progress window.

7. Verify Backup Completion: Once the backup process completes successfully, verify the backup file's location and ensure that it has been generated without errors.
### Task 2: Upload Backup to Blob Storage
1. Access Blob Storage Container: Use an Azure storage explorer tool, Azure CLI, or Azure portal to access the Blob Storage container created in the previous steps.

2. Upload Backup File: Upload the previously created database backup file (.bak) to the Blob Storage container. You can drag and drop the file or use the upload functionality provided by the storage explorer tool or Azure portal.

3. Verify Upload: After the upload process completes, verify that the backup file is present in the Blob Storage container. You can confirm this by viewing the contents of the container through the storage explorer tool or Azure portal.
### Task 3: Restore Database on Development Environment
Setting up a sandbox environment provides a safe and controlled space for software development and experimentation. By following the steps outlined in this guide, you can replicate the development setup, install SQL Server, and restore database backups to create an isolated environment for exploration and innovation.
### Task 4: Automate Backups for Development Database

 With a weekly backup schedule in place, you ensure consistent protection for your evolving work and simplify recovery for your development environment if needed.


### Features
 1. Production Environment Database: Establish a production environment database that will be migrated to Azure SQL Database.

2. Data Backup and Restoration: Focus on crucial aspects like data backup and restoration, including automated scheduling.

3. Disaster Recovery Scenario: Simulate a disaster recovery scenario with potential data loss, exploring the complexities of geo-replication and failover configuration to ensure data availability under challenging conditions.

4. Security: Enhance security through Microsoft Entra ID integration to define access roles, adding an extra layer of control and protection.


## License
This project is licensed under the MIT License. See the LICENSE file for details.