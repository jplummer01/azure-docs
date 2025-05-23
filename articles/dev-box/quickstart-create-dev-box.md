---
title: 'Quickstart: Create a dev box'
titleSuffix: Microsoft Dev Box
description: In this quickstart, learn how developers can create a dev box in the Microsoft Dev Box developer portal, and remotely connect to it through the browser.
services: dev-box
ms.service: dev-box
ms.custom:
  - build-2024
ms.topic: quickstart
author: RoseHJM
ms.author: rosemalcolm
ms.date: 03/03/2025
#Customer intent: As a dev box user, I want to understand how to create and access a dev box so that I can start work.
---

# Quickstart: Create and connect to a dev box by using the Microsoft Dev Box developer portal

[!INCLUDE [note-build-2025](includes/note-build-2025.md)]


In this quickstart, you get started with Microsoft Dev Box by creating a dev box through the developer portal. After you create the dev box, you can connect to it through a browser or through a Remote Desktop client like Windows App.

You can create and manage multiple dev boxes as a dev box user. Create a dev box for each task that you're working on, and create multiple dev boxes within a single project to help streamline your workflow. For example, you might switch to another dev box to fix a bug in a previous version, or if you need to work on a different part of the application.

## Prerequisites

To complete this quickstart, you need:

| Product | Requirements |
|---------|--------------|
| Microsoft Dev Box | Your organization must configure Microsoft Dev Box with at least one project and dev box pool before you can create a dev box. <br> - Platform engineers can follow these steps to configure Microsoft Dev Box: [Quickstart: Configure Microsoft Dev Box](quickstart-configure-dev-box-service.md). <br>**Permissions** <br> - You must have permissions as a [Dev Box User](quickstart-configure-dev-box-service.md#provide-access-to-a-dev-box-project) for a project that has an available dev box pool. If you don't have permissions to a project, contact your administrator.|
| Windows App | To connect to a dev box by using the Windows App, you need to install the Windows App on your device. <br> - [Download Windows App](https://apps.microsoft.com/detail/9n1f85v9t8bn?hl=en-us&gl=US) |

## Create a dev box

Microsoft Dev Box enables you to create cloud-hosted developer workstations in a self-service way. You can create and manage dev boxes by using the developer portal.

Depending on the project configuration and your permissions, you have access to different projects and associated dev box configurations. If you have a choice of projects and dev box pools, select the project and dev box pool that best fits your needs. For example, you might choose a project that has a dev box pool located near to you for least latency.

> [!IMPORTANT]
> Your organization must configure Microsoft Dev Box with at least one project and dev box pool before you can create a dev box. If you don't see any projects or dev box pools, contact your administrator.

To create a dev box in the Microsoft Dev Box developer portal:

[!INCLUDE [developer-portal-landing-page](includes/developer-portal-landing-page.md)]

4. In **Add a dev box**, enter the following values:

   | Setting | Value |
   |---|---|
   | **Name** | Enter a name for your dev box. Dev box names must be unique within a project. |
   | **Project** | Select a project from the dropdown list. |
   | **Dev box pool** | Select a pool from the dropdown list, which includes all the dev box pools for that project. Choose a dev box pool near to you for least latency.|

   :::image type="content" source="./media/quickstart-create-dev-box/developer-portal-create-dev-box.png" alt-text="Screenshot of the dialog for adding a dev box." lightbox="./media/quickstart-create-dev-box/developer-portal-create-dev-box.png":::

   After you make your selections, the page shows you the following information:

   - How many dev boxes you can create in the project that you selected, if the project has limits configured.
   - Whether *Hibernation* is supported or not.
   - Whether *Customizations* is enabled or not.
   - A shutdown time if the pool where you're creating the dev box has a shutdown schedule.
   - A notification that the dev box creation process can take 25 minutes or longer.
   
5. Select **Create** to begin creating your dev box.

6. Track the progress of creation by using the dev box tile in the developer portal. The status changes from *Creating* to *Running* when the dev box is ready for you to connect to it.
      
   :::image type="content" source="./media/quickstart-create-dev-box/dev-box-tile-creating.png" alt-text="Screenshot of the developer portal that shows the dev box card with a status of Creating." lightbox="./media/quickstart-create-dev-box/dev-box-tile-creating.png":::
   
   > [!Note]
   > If you encounter a vCPU quota error with a *QuotaExceeded* message, ask your administrator to [request an increased quota limit](/azure/dev-box/how-to-request-quota-increase). If your admin can't increase the quota limit at this time, try selecting another pool with a region close to your location. 

[!INCLUDE [dev box runs on creation note](./includes/note-dev-box-runs-on-creation.md)]

## Connect to a dev box

After you create a dev box, you can connect to it remotely through the developer portal on your desktop, laptop, tablet, or phone. Microsoft Edge gives you the best experience. The developer portal provides the option to connect by using Windows App. 

### Connect by using Windows App

[!INCLUDE [connect-with-windows-app](includes/connect-with-windows-app.md)]

## Use multiple monitors

[!INCLUDE [configure-multiple-monitors](includes/configure-multiple-monitors.md)]

## Clean up resources

In this quickstart, you created a dev box through the developer portal and connected to it by using a browser. 

When you no longer need your dev box, you can delete it:

[!INCLUDE [dev box runs on creation note](./includes/clean-up-resources.md)] 

## Related content

In this quickstart, you created a dev box through the developer portal and connected to it by using a browser. 

- Find out [What's new in Microsoft Dev Box](https://aka.ms/devbox/WhatsNew)
- Discover what's coming up next in Microsoft Dev Box: [Microsoft Dev Box roadmap](dev-box-roadmap.md)
- Learn how to [Manage a dev box by using the Microsoft Dev Box developer portal](how-to-create-dev-boxes-developer-portal.md)