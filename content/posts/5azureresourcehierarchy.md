+++
date = '2025-06-12T19:25:26+03:00'
draft = true
title = 'Azure Resource Hierarchy'
+++

# Understanding Azure Resource Hierarchy: From Management Groups to Resources

Organizing and managing cloud resources effectively is crucial for cost control, security, and operational efficiency. In Microsoft Azure, the resource hierarchy defines how resources are structured, organized, and managed. Understanding this hierarchy is essential for setting governance policies, managing permissions, and ensuring a scalable cloud environment.

In this article, we’ll break down the Azure resource hierarchy, explain each layer, and show how they work together.

# The Azure Resource Hierarchy

Azure resources are organized in a layered structure that allows administrators to apply policies, access controls, and governance at different levels. The hierarchy consists of four main levels:

1.  Management Groups

2.  Subscriptions

3.  Resource Groups

4.  Resources

# 1. Management Groups

Management Groups are at the top of the hierarchy. They are used to organize subscriptions into a unified structure, making it easier to apply governance policies across multiple subscriptions.

### Key Features:

- Can contain other management groups or subscriptions.

- Policies and role-based access control (RBAC) assigned at this level are inherited by all child elements.

- Ideal for large organizations with multiple business units or environments (e.g., Dev, Test, Prod).

### Example Use Case:

A company with multiple Azure subscriptions for different departments can group them under a single management group to apply global compliance rules.

# 2. Subscriptions

A subscription is a logical container that holds Azure resources and is linked to an Azure account. It is also the billing boundary, meaning all usage within a subscription is billed together.

### Key Points:

- Each subscription has its own limits and quotas.

- Can be used to separate environments (e.g., development, testing, production).

- Linked to Azure Active Directory (Azure AD) for identity and access management.

# 3. Resource Groups

Resource Groups are logical containers for Azure resources. Every resource in Azure must belong to a single resource group.

### Benefits:

- Simplifies management by grouping related resources.

- Enables bulk operations like deployment, deletion, or policy application.

- Supports role-based access control at the group level.

### Example:

A web app, its associated database, and storage account can all be placed in the same resource group for easier management.

# 4. Resources

Resources are the actual Azure services you create and use — such as virtual machines, storage accounts, databases, and virtual networks.

### Key Points:

- The lowest level in the hierarchy.

- Each resource is deployed within a resource group and subscription.

- Inherits access controls and policies from higher levels.

# Why the Hierarchy Matters

Understanding the Azure resource hierarchy is important because:

- Governance – Apply policies and compliance rules at the right scope.

- Security – Implement RBAC to control who can access what.

- Cost Management – Monitor and manage costs per subscription or resource group.

- Scalability – Organize resources to support future growth without chaos.

# Best Practices

- Use management groups to mirror your organizational structure.

- Create separate subscriptions for production and non-production workloads.

- Group related resources into a single resource group.

- Apply policies at the highest relevant scope for consistency.

# Conclusion

The Azure resource hierarchy — from management groups down to resources — provides a structured way to manage and secure your cloud environment. By applying governance, access controls, and policies at the right levels, you can ensure your Azure environment remains organized, compliant, and scalable.
