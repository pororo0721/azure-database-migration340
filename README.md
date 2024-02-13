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
- SQL Login Authentication
- Configure Firewall Rules
- Adavanced Firewall Configuration

### Task 2: Prepare for Migration
- Launch Azure Data Studio
- Connect to On-Premise Database
- Configure Connection Details
- Test Connection
- Save Connection Profile
### Task 3: Connect to Azure SQL Database
- Launch Azure Data Studio
- Connect to Azure SQL Database
- Perform Schema and Data Migration

### Task 4: Schema Migration
- Install SQL Server Schema Compare Extension
- Perform Schema Comparison
- Review and Apply Schema Changes

### Task 5: Data Migration
- Launch Azure Data Studio
- Install Azure SQL Migration Extension
- Perform Data Migration

### Task 6: Validate Migration Success
- Data Validation
- Schema Validation
- Configuration Validation
- Performance Testing

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
- Provision a New Windows VM
- Install SQL Server
- Restore Database Backup
- Explore and Experiment

### Task 4: Automate Backups for Development Database

- Launch SQL Server Management Studio (SSMS)
- Create a New Maintenance Plan
- Add Backup Database Task
- Set Backup Schedule
- Configure Maintenance Cleanup Task

## Milestone 5: Disaster Recovery Simulation

### Task 1: Mimic Data Loss in Production Environment

Steps to Simulate Data Loss:
1. Identify Critical Data
2. Document Data Removal Process
3. Perform Data Removal
4. Confirm Simulation Sucess

### Task 2: Restore Database from Azure SQL Database Backup

Steps to Restore Database from Backup

1. Identify Backup
2. Restore Database
3. Validation of Restoration
4. Update Production Environment
5. Delete Affected Database





## Features
 1. Production Environment Database: Establish a production environment database that will be migrated to Azure SQL Database.

2. Data Backup and Restoration: Focus on crucial aspects like data backup and restoration, including automated scheduling.

3. Disaster Recovery Scenario: Simulate a disaster recovery scenario with potential data loss, exploring the complexities of geo-replication and failover configuration to ensure data availability under challenging conditions.

4. Security: Enhance security through Microsoft Entra ID integration to define access roles, adding an extra layer of control and protection.


## License
This project is licensed under the MIT License. See the LICENSE file for details.