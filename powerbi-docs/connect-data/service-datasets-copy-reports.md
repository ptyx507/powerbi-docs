---
title: Copy reports from other apps or workspaces - Power BI
description: Learn how you can create a copy of a report and save it to your own workspace.
author: maggiesMSFT
ms.reviewer: kayu
ms.service: powerbi
ms.subservice: powerbi-service
ms.topic: how-to
ms.date: 04/30/2020
ms.author: maggies

LocalizationGroup: Share your work
---
# Copy reports from other workspaces

When you find a report you like in a workspace or an app, you can make a copy of it and save it to a different workspace. Then you can modify your copy of the report, adding or deleting visuals and other elements. You don't have to worry about creating the data model. It's already created for you. And it's much easier to modify an existing report than it is to start from scratch. However, when you make an app from your workspace, sometimes you can't publish your copy of the report in the app. See [Considerations and limitations in the article "Use datasets across workspaces"](service-datasets-across-workspaces.md#considerations-and-limitations) for details.

> [!NOTE]
> To make a copy, you need a Pro license, even if the original report is in a workspace in a Premium capacity.

## Save a copy of a report in a workspace

1. In a workspace, go to the Reports list view.

    ![Reports list view](media/service-datasets-copy-reports/power-bi-report-list-view.png)

1. Under **Actions**, select **Save a copy**.

    ![Save a copy of a report](media/service-datasets-copy-reports/power-bi-dataset-save-report-copy.png)

    You only see the **Save a copy** icon if the report is in a new experience workspace, and you have [Build permission](service-datasets-build-permissions.md). Even if you have access to the workspace, you have to have Build permission for the dataset.

3. In **Save a copy of this report**, give the report a name and select the destination workspace.

    ![Save a copy dialog box](media/service-datasets-copy-reports/power-bi-dataset-save-report.png)

    You can save the report to the current workspace or a different one in the Power BI service. You only see workspaces that are new experience workspaces, in which you're a member. 
  
4. Select **Save**.

    Power BI automatically creates a copy of the report, and an entry in the list of datasets if the report is based on a dataset outside of the workspace. The icon for this dataset is different from the icon for datasets in the workspace: ![Shared dataset icon](media/service-datasets-discover-across-workspaces/power-bi-shared-dataset-icon.png)
    
    That way, members of the workspace can tell which reports and dashboards use datasets that are outside the workspace. The entry shows information about the dataset, and a few select actions.

    ![Dataset actions](media/service-datasets-across-workspaces/power-bi-dataset-actions.png)

    See [Your copy of the report](#your-copy-of-the-report) in this article for more about the report and related dataset.

## Copy a report in an app

1. In an app, open the report you want to copy.
2. In the menu bar, select **More options** (**...**) > **Save a copy**.

    ![Save a copy of the report](media/service-datasets-copy-reports/power-bi-save-copy.png)

    You only see the **Save a copy** option if the report is in a new experience workspace, and you have [Build permission](service-datasets-build-permissions.md).

3. Give your report a name > **Save**.

    ![Name your copy of the report](media/service-datasets-copy-reports/power-bi-save-report-from-app.png)

    Your copy is automatically saved to your My Workspace.

4. Select **Go to report** to open your copy.

## Your copy of the report

When you save a copy of the report, you create a live connection to the dataset, and you can open the report creation experience with the full dataset available. 

![Edit your copy of the report](media/service-datasets-copy-reports/power-bi-edit-report-copy.png)

You haven't made a copy of the dataset. The dataset still resides in its original location. You can use all tables and measures in the dataset in your own report. Row-level security (RLS) restrictions on the dataset are in effect, so you only see data you have permissions to see based on your RLS role.

## View related datasets

When you have a report in one workspace based on a dataset in another workspace, you may need to know more about the dataset it's based on.

1. In the Reports list view, select **View related**.

    ![Screenshot shows the View related icon under Actions.](media/service-datasets-copy-reports/power-bi-dataset-view-related.png)

1. The **Related content** dialog box shows all related items. In this list, the dataset looks like any other. You can't tell it resides in a different workspace. This issue is known.
 
    ![Related content dialog box](media/service-datasets-copy-reports/power-bi-dataset-related.png)

## Delete a report and its shared dataset

You may decide you no longer want the report and its associated shared dataset in workspace.

1. Delete the report. In the list of reports in the workspace, select the **Delete** icon.

    ![Delete report icon](media/service-datasets-across-workspaces/power-bi-datasets-delete-report.png)

2. In the list of datasets, you see the shared datasets don't have **Delete** icons. Refresh the page, or go to a different page and return. The dataset will be gone. If not, check **View related**. It may be related to another table in your workspace.

    ![Screenshot shows a dataset with View related option to check for related tables.](media/service-datasets-across-workspaces/power-bi-dataset-view-related-icon.png)

    > [!NOTE]
    > Deleting the shared dataset in this workspace doesn't delete the dataset. It just deletes the reference to it.


## Next steps

- [Use datasets across workspaces](service-datasets-across-workspaces.md)
- Questions? [Try asking the Power BI Community](https://community.powerbi.com/)
