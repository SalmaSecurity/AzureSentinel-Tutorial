# How to start: Step-by-Step Guide

## Creating a Log Analytics Workspace and Activating Azure Sentinel

To deploy Azure Sentinel, it's recommended to create a dedicated Log Analytics workspace rather than using an existing one. Here’s a simplified guide to get started:

### **Step 1: Set Up Your Azure Environment**
- **Choose an Active Azure Subscription:** Make sure you have an active Azure subscription.
- **Create or Select a Resource Group:** Organize and manage resources associated with the project by selecting or creating a resource group.

### **Step 2: Create a Log Analytics Workspace**
- Follow the guided steps to create a Log Analytics workspace in Azure.
  
  <p align="center">
    <img src="images/workspace creation copy.png" alt="Creation of Log Analytics Workspace in Azure" width="1000"/>
  </p>

### **Step 3: Add Microsoft Sentinel**
- Navigate to the Azure Portal and search for "Microsoft Sentinel" in the search bar.
- Select Microsoft Sentinel and follow the prompts to configure the necessary settings. This includes linking the Log Analytics workspace to Microsoft Sentinel.

  <p align="center">
    <img src="images/add MS to a workspace cpy.png" alt="Microsoft Sentinel in Azure Portal" width="1000"/>
  </p>

### **Step 4: Configure Advanced Settings**
Once Azure Sentinel is added to your Log Analytics workspace, you can configure its advanced settings. Key aspects to consider include:

#### **Environment Settings**
- Managed within Azure Sentinel and the Log Analytics workspace.
- Access "Settings" from the left navigation pane in Azure Sentinel.

  <p align="center">
    <img src="images/param avancés.png" alt="Workspace Settings in Sentinel" width="1000"/>
  </p>

#### **Cost Optimization and Data Retention**
- **Daily Cap:** Set a daily ingestion limit to control the volume of data entering the Log Analytics workspace, which helps manage costs.

  <p align="center">
    <img src="images/daily cap setting.png" alt="Daily Cap Configuration" width="1000"/>
  </p>

- **Data Retention:** Adjust the data retention period from 30 to 2555 days based on legal, regulatory, and operational needs. Keep in mind that longer retention periods can lead to higher storage costs.

  <p align="center">
    <img src="images/data retention setting.png" alt="Log Retention Configuration" width="1000"/>
  </p>

### **Step 5: Manage Access with IAM**
- Use the IAM (Identity and Access Management) page to assign roles and manage access to Azure resources, ensuring rigorous security in the Azure environment.

  <p align="center">
    <img src="images/iam.png" alt="IAM Settings" width="1000"/>
  </p>
