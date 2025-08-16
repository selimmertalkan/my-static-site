+++
date = '2025-03-14T13:01:00+03:00'
draft = true
title = 'Azure Management Tools'
+++

# An Overview of Azure CLI, Azure PowerShell, and Azure Portal

When working with Microsoft Azure, efficient management is key to deploying, monitoring, and scaling resources. Azure offers several management tools that cater to different preferences and use cases — whether you prefer a graphical interface, a command-line environment, or automation scripts. In this article, we’ll explore what Azure Management Tools are, the types available, and dive deeper into Azure CLI, Azure PowerShell, and Azure Portal.

# What Are Azure Management Tools?

Azure Management Tools are interfaces or utilities that allow you to interact with Azure resources. They enable you to create, configure, monitor, and delete resources in a controlled and efficient way. These tools range from fully graphical dashboards to command-line utilities designed for automation.

### The main categories of Azure Management Tools include:

- Graphical tools – such as Azure Portal

- Command-line tools – such as Azure CLI and Azure PowerShell

- SDKs and APIs – for programmatic access via supported programming languages

# Azure CLI

The Azure Command-Line Interface (CLI) is a cross-platform command-line tool for managing Azure resources. It is designed for those who prefer scripting or automation over graphical interfaces.

### Key Features of Azure CLI:

#### Cross-platform:

Works on Windows, macOS, and Linux.

#### Automation-friendly:

Can be integrated into CI/CD pipelines or shell scripts.

#### Simplicity:

Uses commands with a straightforward syntax, often easier for those familiar with Bash or similar shells.

### Example Command:

```bash
az group create --name MyResourceGroup --location eastus
```

This command creates a new resource group in the East US region.

# Azure PowerShell

Azure PowerShell is a set of cmdlets (command-lets) that allow you to manage Azure resources directly from PowerShell.

## Why Use Azure PowerShell?

### Deep integration with Windows PowerShell:

Ideal for administrators familiar with PowerShell scripting.

### Automation:

Easily automate repetitive tasks in Azure.

### Consistency:

Works with Azure Resource Manager (ARM) to ensure resource management is predictable.

## Versions of PowerShell for Azure:

### Windows PowerShell:

The original version, Windows-only.

### PowerShell Core (pwsh):

Cross-platform version based on .NET Core, supported on Windows, macOS, and Linux.

### Az PowerShell Module:

The recommended module for managing Azure resources (replaces the older AzureRM module).

## Example Command:

`New-AzResourceGroup -Name "MyResourceGroup" -Location "EastUS"`

This creates a new resource group similar to the Azure CLI example, but using PowerShell syntax.

# Azure Portal

The Azure Portal is a web-based graphical interface for managing Azure resources. It is ideal for users who prefer a visual approach and want to explore Azure without memorizing commands.

## Key Features:

- Visual dashboards for monitoring resources.

- Resource creation wizards to guide you through deployments.

- Built-in cost management tools.

- Accessible at: https://portal.azure.com

## Use Cases:

- Quick resource creation and management.

- Visualizing metrics and performance.

- Accessing Azure services without installing local tools.

# How They Work Together

Although these tools can be used independently, many Azure professionals use a combination of them:

- Azure Portal for quick checks and visual management.

- Azure CLI for fast, script-based operations.

- Azure PowerShell for automation in Windows-heavy environments or complex scripts.

# Conclusion

Azure Management Tools give you the flexibility to work the way you prefer — whether that’s through a user-friendly web portal, a cross-platform CLI, or the powerful automation capabilities of PowerShell. Understanding when and how to use each tool is a crucial skill for anyone working in cloud computing and DevOps.
