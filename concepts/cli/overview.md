---
title: "Microsoft Graph command-line interface (CLI) overview"
description: "Learn about the features of the Microsoft Graph command-line interface that can help you derive insights and analytics, and build unique, intelligent apps."
ms.localizationpriority: medium
author: jasonjoh
ms.date: 11/07/2024
---

# Microsoft Graph command-line interface (CLI) overview

The Microsoft Graph PowerShell command-line interface (CLI) acts as an API wrapper for the Microsoft Graph APIs, exposing the entire API set for use from the command line.

## Microsoft Graph CLI features & benefits

The Microsoft Graph CLI provides the following benefits:

- **Access to all Microsoft Graph APIs**: The Microsoft Graph CLI is based on Microsoft Graph API. In addition to Microsoft Entra ID, the Microsoft Graph API includes APIs from other Microsoft services like SharePoint, Exchange, and Outlook, all accessed through a single endpoint with a single access token.
- **Cross-platform support**: The Microsoft Graph CLI works on all platforms including Windows, macOS, and Linux.
- **Supports modern authentication**: The Microsoft Graph CLI supports the Microsoft Authentication Library (MSAL) which offers more security.
- **Uses least privilege**: Microsoft Graph CLI permissions aren't preauthorized and users must perform one-time request for app permissions depending on their needs.
- **Open source**: Feature teams and the community can create great command-line experiences and share them with everyone.
- **Receives regular updates**: Microsoft Graph CLI commands are updated regularly to support the latest Graph API updates.

## Install the Microsoft Graph CLI

The Microsoft Graph CLI is published on [GitHub](https://github.com/microsoftgraph/msgraph-cli). Follow the [Install the CLI](installation.md) instructions to install the Microsoft Graph PowerShell SDK.

## Get started

To perform basic tasks, see [Get started with the Microsoft Graph CLI](get-started.md).

## Next steps

- If you don't have a Microsoft 365 tenant, you might qualify for one through the [Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program); for details, see the [FAQ](/office/developer-program/microsoft-365-developer-program-faq#who-qualifies-for-a-microsoft-365-e5-developer-subscription-). Alternatively, you can [sign up for a 1-month free trial or purchase a Microsoft 365 plan](https://www.microsoft.com/en-us/microsoft-365/try).
- If you already have access to a Microsoft 365 tenant, [Install the SDK](installation.md).
