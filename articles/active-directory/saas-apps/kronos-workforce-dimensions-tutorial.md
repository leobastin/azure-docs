---
title: 'Tutorial: Azure AD SSO integration with Kronos Workforce Dimensions'
description: Learn how to configure single sign-on between Azure Active Directory and Kronos Workforce Dimensions.
services: active-directory
author: jeevansd
manager: CelesteDG
ms.reviewer: CelesteDG
ms.service: active-directory
ms.subservice: saas-app-tutorial
ms.workload: identity
ms.topic: tutorial
ms.date: 01/27/2021
ms.author: jeedes

---

# Tutorial: Azure AD SSO integration with Kronos Workforce Dimensions

In this tutorial, you'll learn how to integrate Kronos Workforce Dimensions with Azure Active Directory (Azure AD). When you integrate Kronos Workforce Dimensions with Azure AD, you can:

* Control in Azure AD who has access to Kronos Workforce Dimensions.
* Enable your users to be automatically signed-in to Kronos Workforce Dimensions with their Azure AD accounts.
* Manage your accounts in one central location - the Azure portal.

## Prerequisites

To get started, you need the following items:

* An Azure AD subscription. If you don't have a subscription, you can get a [free account](https://azure.microsoft.com/free/).
* Kronos Workforce Dimensions single sign-on (SSO) enabled subscription.

> [!NOTE]
> This integration is also available to use from Azure AD US Government Cloud environment. You can find this application in the Azure AD US Government Cloud Application Gallery and configure it in the same way as you do from public cloud.

## Scenario description

In this tutorial, you configure and test Azure AD SSO in a test environment.

* Kronos Workforce Dimensions supports **SP** initiated SSO.

## Add Kronos Workforce Dimensions from the gallery

To configure the integration of Kronos Workforce Dimensions into Azure AD, you need to add Kronos Workforce Dimensions from the gallery to your list of managed SaaS apps.

1. Sign in to the Azure portal using either a work or school account, or a personal Microsoft account.
1. On the left navigation pane, select the **Azure Active Directory** service.
1. Navigate to **Enterprise Applications** and then select **All Applications**.
1. To add new application, select **New application**.
1. In the **Add from the gallery** section, type **Kronos Workforce Dimensions** in the search box.
1. Select **Kronos Workforce Dimensions** from results panel and then add the app. Wait a few seconds while the app is added to your tenant.

## Configure and test Azure AD SSO for Kronos Workforce Dimensions

Configure and test Azure AD SSO with Kronos Workforce Dimensions using a test user called **B.Simon**. For SSO to work, you need to establish a link relationship between an Azure AD user and the related user in Kronos Workforce Dimensions.

To configure and test Azure AD SSO with Kronos Workforce Dimensions, perform the following steps:

1. **[Configure Azure AD SSO](#configure-azure-ad-sso)** - to enable your users to use this feature.
    1. **[Create an Azure AD test user](#create-an-azure-ad-test-user)** - to test Azure AD single sign-on with B.Simon.
    1. **[Assign the Azure AD test user](#assign-the-azure-ad-test-user)** - to enable B.Simon to use Azure AD single sign-on.
1. **[Configure Kronos Workforce Dimensions SSO](#configure-kronos-workforce-dimensions-sso)** - to configure the single sign-on settings on application side.
    1. **[Create Kronos Workforce Dimensions test user](#create-kronos-workforce-dimensions-test-user)** - to have a counterpart of B.Simon in Kronos Workforce Dimensions that is linked to the Azure AD representation of user.
1. **[Test SSO](#test-sso)** - to verify whether the configuration works.

## Configure Azure AD SSO

Follow these steps to enable Azure AD SSO in the Azure portal.

1. In the Azure portal, on the **Kronos Workforce Dimensions** application integration page, find the **Manage** section and select **single sign-on**.
1. On the **Select a single sign-on method** page, select **SAML**.
1. On the **Set up single sign-on with SAML** page, click the pencil icon for **Basic SAML Configuration** to edit the settings.

   ![Edit Basic SAML Configuration](common/edit-urls.png)

1. On the **Basic SAML Configuration** section, perform the following steps:

    a. In the **Identifier (Entity ID)** text box, type a URL using the following pattern:
    `https://<SUBDOMAIN>.<ENVIRONMENT>.mykronos.com/authn/<TENANT_ID/hsp/<TENANT_NUMBER>`

    b. In the **Sign on URL** text box, type a URL using one of the following patterns:
    
    | **Sign on URL** |
    |-----|
    | `https://<CUSTOMER>-<ENVIRONMENT>-sso.<ENVIRONMENT>.mykronos.com/` |
    | `https://<CUSTOMER>-sso.<ENVIRONMENT>.mykronos.com/` |

	> [!NOTE]
	> These values are not real. Update these values with the actual Identifier and Sign on URL. Contact [Kronos Workforce Dimensions Client support team](mailto:support@kronos.com) to get these values. You can also refer to the patterns shown in the **Basic SAML Configuration** section in the Azure portal.

1. On the **Set up single sign-on with SAML** page, In the **SAML Signing Certificate** section, click copy button to copy **App Federation Metadata Url** and save it on your computer.

	![The Certificate download link](common/copy-metadataurl.png)

### Create an Azure AD test user

In this section, you'll create a test user in the Azure portal called B.Simon.

1. From the left pane in the Azure portal, select **Azure Active Directory**, select **Users**, and then select **All users**.
1. Select **New user** at the top of the screen.
1. In the **User** properties, follow these steps:
   1. In the **Name** field, enter `B.Simon`.  
   1. In the **User name** field, enter the username@companydomain.extension. For example, `B.Simon@contoso.com`.
   1. Select the **Show password** check box, and then write down the value that's displayed in the **Password** box.
   1. Click **Create**.

### Assign the Azure AD test user

In this section, you'll enable B.Simon to use Azure single sign-on by granting access to Kronos Workforce Dimensions.

1. In the Azure portal, select **Enterprise Applications**, and then select **All applications**.
1. In the applications list, select **Kronos Workforce Dimensions**.
1. In the app's overview page, find the **Manage** section and select **Users and groups**.
1. Select **Add user**, then select **Users and groups** in the **Add Assignment** dialog.
1. In the **Users and groups** dialog, select **B.Simon** from the Users list, then click the **Select** button at the bottom of the screen.
1. If you are expecting a role to be assigned to the users, you can select it from the **Select a role** dropdown. If no role has been set up for this app, you see "Default Access" role selected.
1. In the **Add Assignment** dialog, click the **Assign** button.

## Configure Kronos Workforce Dimensions SSO

To configure single sign-on on **Kronos Workforce Dimensions** side, you need to send the **App Federation Metadata Url** to [Kronos Workforce Dimensions support team](mailto:support@kronos.com). They set this setting to have the SAML SSO connection set properly on both sides.

### Create Kronos Workforce Dimensions test user

In this section, you create a user called Britta Simon in Kronos Workforce Dimensions. Work with [Kronos Workforce Dimensions support team](mailto:support@kronos.com) to add the users in the Kronos Workforce Dimensions platform. Users must be created and activated before you use single sign-on.

## Test SSO 

In this section, you test your Azure AD single sign-on configuration with following options. 

* Click on **Test this application** in Azure portal. This will redirect to Kronos Workforce Dimensions Sign-on URL where you can initiate the login flow. 

* Go to Kronos Workforce Dimensions Sign-on URL directly and initiate the login flow from there.

* You can use Microsoft My Apps. When you click the Kronos Workforce Dimensions tile in the My Apps, this will redirect to Kronos Workforce Dimensions Sign-on URL. For more information about the My Apps, see [Introduction to the My Apps](https://support.microsoft.com/account-billing/sign-in-and-start-apps-from-the-my-apps-portal-2f3b1bae-0e5a-4a86-a33e-876fbd2a4510).

## Next steps

Once you configure Kronos Workforce Dimensions you can enforce session control, which protects exfiltration and infiltration of your organization’s sensitive data in real time. Session control extends from Conditional Access. [Learn how to enforce session control with Microsoft Defender for Cloud Apps](/cloud-app-security/proxy-deployment-aad).