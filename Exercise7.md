# Lab Guide

## Governing access with Conditional Access policies

### Overview

In this lab you will learn to use Conditional Access policies to govern access to cloud apps.

### More Information

- [Microsoft Learn Azure Marketplace Documentation](https://learn.microsoft.com/en-us/marketplace/azure-marketplace-overview)

### Time Estimate

- 30 minutes

## Task 1 – Creating Conditional Access Policies

A conditional access policy in Entra ID is important because it allows you to apply the right access controls when needed to keep your organization secure. A conditional access policy is an if-then statement that evaluates various signals, such as user, device, location, application, and risk, and enforces organizational policies based on the conditions and access controls you specify. For example, you can create a policy that requires multifactor authentication for users who access sensitive applications from outside your trusted network. Conditional access policies can help you achieve the following goals:

-   Empower users to be productive wherever and whenever they need to work.
-   Protect your organization's assets from unauthorized access and potential security breaches.
-   Comply with regulatory and organizational requirements for data retention and reporting.
-   Optimize your identity and access strategy and improve your user experience.

**HOWEVER, PLEASE NOTE:** Security Defaults provide baseline protection for a tenant out of the box (require MFA for all users including Admins, block legacy auth) but its functionality is superseded by conditional access. Conditional Access policies are a way for organizations to customize access based on the needs and/or organizational policies and it may not be necessary to create Conditional Access policies for your organization. Take great care to ensure it’s absolutely necessary and even then consider using the provided templates to start with instead of creating something entirely new.

Conditional Access templates provide a convenient method to deploy new policies aligned with Microsoft recommendations. These templates are designed to provide maximum protection aligned with commonly used policies across various customer types and locations.

In this task, let’s go through and review some popular Conditional Access Policy templates.

1.  Open the browser tab to the home page of the Microsoft Entra admin center. If you previously closed the browser tab, open Microsoft Edge and in the address bar enter +++**https://entra.microsoft.com+++** and sign in with the Microsoft 365 admin credentials provided by the ALH.
2.  From the left navigation pane, expand **Protection** then select **Conditional Access**.
3.  The Conditional access overview page is displayed. Here you will see tiles showing the Policy summary and general alerts. From the left navigation panel, select **Policies**.
4.  Any existing Conditional Access Policies are listed here. Select **+ New policy from template**.
5.  Here you’ll see several template categories. 16 Conditional Access policy templates are organized into the following categories: Secure foundation, Zero Trust, Remote Work, Protect Administrator, and Emerging threats.
6.  When finished reviewing the Conditional Access policy options, close the Templates window by clicking the **X** at the top right of the windows in the Entra admin center.
7.  Details about the provided templates can be found here: ++++https://learn.microsoft.com/en-us/azure/active-directory/conditional-access/concept-conditional-access-policy-common++++

## Task 2 – The Conditional Access What If tool

The **What If** tool in Conditional Access is powerful when trying to understand why a policy was or wasn't applied to a user in a specific circumstance or if a policy would apply in a known state.

1.  The **What If** tool is located in the **Microsoft Entra admin center \> Protection \> Conditional Access \> Policies \>** **What If**. (What If is in the center of the window in the top policy menu)
2.  The What If tool requires only a User or Workload identity to get started. The following additional information is optional but helps narrow the scope for specific cases:
-   Cloud apps, actions, or authentication context
-   IP address
-   Country/Region
-   Device platform
-   Client apps
-   Device state
-   Sign-in risk
-   User risk level
-   Service principal risk (Preview)
-   Filter for devices
1.  This information can be gathered from the user, their device, or the Microsoft Entra sign-in log
2.  For details, see: ++++https://learn.microsoft.com/en-us/azure/active-directory/conditional-access/troubleshoot-conditional-access-what-if++++

### Summary

In this exercise, you learned to use Conditional Access policies to govern access to cloud apps. 
