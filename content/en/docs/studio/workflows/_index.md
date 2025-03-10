---
title: "Workflows"
url: /studio/workflows/
description: "Describes the workflows in Mendix Studio."
weight: 15
tags: ["workflow", "workflows", "Studio"]
#If moving or renaming this doc file, implement a temporary redirect and let the respective team know they should update the URL in the product. See Mapping to Products for more details.
---

## 1 Introduction

Workflow is a visual language in Mendix Studio and Mendix Studio Pro that allows you to build extendable business processes. It is fully integrated with other visual languages, such as the microflow editor and page editor. 

The main difference between workflows and [microflows](/studio/microflows/) is a waiting aspect – the workflow is paused until it gets an input from an end-user. For example, an employee sends a travel request (triggering the start of the workflow) and then the workflow is paused until a manager approves the request by clicking a button. 

To view the workflows of your app in Studio, click the **Workflows** icon in the left menu bar:

{{< figure src="/attachments/studio/workflows/workflow-icon.jpg" alt="Workflow Icon" >}}

Workflows are a visual way of processing logic in your application. A workflow looks like a flow chart. On a new workflow a *start event* (a starting point of the workflow) and an *end event* (an endpoint of the workflow) are created by default. You can add various activities to a flow of a workflow that is called a *path*.

{{< figure src="/attachments/studio/workflows/workflow-example.jpg" alt="Workflow Example" >}}

{{% alert type="note" %}}
Workflows are available in Studio from **Mendix version 9.12.1**. If you have an app with workflow functionality below this version, this app is most likely to be created in Studio Pro and requires a manual migration. For more information on how to migrate your app using Studio Pro, see [Migrating Workflow Apps](/refguide/workflow-beta-migration/). 
{{% /alert %}}

## 2 Performing Basic Functions

You can perform the following basic functions when configuring workflows:

* [Enable workflow functionality](#enable)
* [Create a workflow](#create)
* [Open a workflow](#open)
* [Duplicate a workflow](#duplicate)
* [Copy and paste a workflow](#copy-paste)
* [Delete a workflow](#delete)
* [Add elements to a workflow](#add-elements)

### 2.1 Enabling Workflows {#enable}

To enable workflow functionality, do the following:

1. Click the workflow icon in the left menu bar.
2. Before enabling workflows, you need to enable security. Click **Enable Security**:

    {{< figure src="/attachments/studio/workflows/enable-security.png" alt="Enable Security" >}}

3. After security is enabled, click **Enable Workflows**.

Workflows are enabled in your app and you can create a workflow. 

### 2.2 Creating a Workflow {#create}

There are two ways to create a workflow: 

* [Using a wizard to build an approval workflow](/studio-how-to/workflow-how-to-configure-using-wizard/) – the wizard helps you create the Approval Request workflow. If your workflow falls under the approval request use case, for example, approving vacation days for your employees, this is a good starting point that sets the whole app automatically for you – not only the workflow itself but also pages and navigation
* [Setting the workflow up manually](/studio-how-to/workflow-how-to-configure/) – if your use case does not fall under an approval request, then you can configure your workflow manually instead of using the wizard

### 2.3 Opening a Workflow {#open}

To open a workflow in Studio, do the following:

1. Click the workflow icon in the left menu bar.
2. In the displayed list of workflows, select the one you want to open and click it:

The selected workflow is opened.

### 2.4 Duplicating a Workflow {#duplicate}

To duplicate a workflow, do the following:

1. Click the **Workflows** icon in the left menu bar.
2. In the side panel, click the ellipsis icon and select **Duplicate** in the drop-down menu:

    {{< figure src="/attachments/studio/workflows/duplicate.jpg" alt="Duplicate a Workflow" >}}

The workflow is duplicated.

### 2.5 Copying and Pasting a Workflow {#copy-paste}

To copy and paste a workflow, do the following:

1. Click the **Workflows** icon in the left menu bar.
2. In the side panel, click the ellipsis icon and select **Copy to clipboard** in the drop-down menu:

    {{< figure src="/attachments/studio/workflows/copy.jpg" alt="Copy a Workflow" >}}

3. Open the Studio app where you want to paste the workflow and press <kbd>Ctrl</kbd> +<kbd>V</kbd> or <kbd>Cmd</kbd> +<kbd>V</kbd>. 

Your workflow is pasted. For more information on copy/paste function in Studio, see the [Copy/Paste Workflows, Pages, Microflows, and Enumerations](/studio/general/#copy-paste-documents) section in *General Info*. 

### 2.6 Deleting a Workflow {#delete}

To delete a workflow in Studio, do one of the following:

1. Open the workflow you want to delete and follow the steps below:
    1. Open the **Properties** tab.
    2. Click **Delete** at the bottom of the **Properties** tab.

2. Click the workflows icon in the left menu bar and do the following:
    1. In the side panel, click the ellipsis icon and select **Delete** in the drop-down menu:

        {{< figure src="/attachments/studio/workflows/delete-workflow.jpg" alt="Delete a Workflow" >}}

The selected workflow is deleted. 

### 2.7 Adding Elements to a Workflow {#add-elements}

To add an element to a workflow, do the following:

1. Open the **Toolbox** tab.
2. Select an element you would like to add and drag this element onto the workflow path.

The selected element is added.

### 2.8 Cutting/Coping/Pasting Elements in a Workflow

To cut/copy/paste elements, use <kbd>Ctrl</kbd> + <kbd>X</kbd> /  <kbd>Ctrl</kbd> + <kbd>C</kbd> / <kbd>Ctrl</kbd> + <kbd>V</kbd> or  <kbd>Cmd</kbd> + <kbd>X</kbd> /  <kbd>Cmd</kbd> + <kbd>C</kbd> / <kbd>Cmd</kbd> + <kbd>V</kbd>.

When using cut/copy/paste, note the following:

* When cutting or copying an element, the clipboard contains the whole structure of the element. For example, when copying a **User Task** with **Outcomes** which contain activities, the **User Task** and the **Outcomes** and its activities are copied. 
    
    Note that copying a **User Task** or a **Microflow** does not create a copy of the elements that are being referenced. Instead, the copied element will have the same references as the original. For example, when the original **User Task** has a task page configured, the copied **User Task** refers to the same task page.
* When no element is selected in the workflow, the clipboard content is pasted at the end of the workflow.
* When the start event is selected, the clipboard content is pasted at the start of the workflow.
* When an activity is selected, the clipboard content is pasted under the selected activity.
* When a flow is selected, the clipboard content is pasted at the beginning of the selected flow.
* When the clipboard contents has an **Annotation**, it can only be pasted into the workflow or into individual activities that support annotations.
* Pasting an activity after an **End** or **Jump** activity results in a consistency error as an **End** or **Jump** activity should be placed at the end of a flow.
* Pasting activity can result in a consistency error when the next activity becomes unreachable by either placing an **End** or **Jump** activity in front of it or when all flows before a merge end with an **End** or **Jump** activity.

#### 2.8.1 Elements that Cannot be Cut, Copied or Pasted

The following elements cannot be cut, copied or pasted in the workflow editor:

* Workflow (you can do it via the left menu bar; for more information, see the [Copying and Pasting a Workflow](#copy-paste) section above)
* WorkflowContext
* Start activity
* End activity (the final **End activity** which is at the end of the workflow)
* Outcomes (meaning outcomes of different outgoing flows from an activity that can have several flows, for example, a Decision)

### 2.9 Triggering a Workflow

You can trigger a workflow [from a page](#trigger-page) or [via a microflow](#trigger-microflow). 

#### 2.9.1 Triggering a Workflow from a Page {#trigger-page}

To start the workflow, you can add a widget with a specific on-click action on a page. For more information on on-click actions, see [Events Section](/studio/page-editor-widgets-events-section/).

Do the following:

1. Open a page from where you would like to trigger a workflow.
2. Drag a widget that has on-click action in its properties (for example, a button) into the data container with the workflow entity. 
3. Open button's properties > **Events** section. 
4. Set **On Click Action** to **More**.
5. Set **Action** to **Call Workflow**. 
6. Set **Workflow** to the workflow you would like to trigger.

You have configured the button to trigger the workflow.

#### 2.9.2 Triggering a Workflow via a Microflow {#trigger-microflow}

To trigger a workflow via a microflow, you can add a **Call workflow** activity to the microflow. For more information on this activity, see [Workflow Activities](/studio/microflows/#microflow-workflow-activities) section in *Microflows*.  

Do the following:

1. Open a microflow that will trigger a workflow.
2. Make sure the microflow has a necessary parameter with the **Workflow Context** entity. 
3. In the **Toolbox**, find **Call workflow** activity and drag it into the microflow.
4. Open the activity properties.
5. Set **Workflow** to to the workflow you would like to trigger.
6. Set **Workflow Object** to the workflow context.
7. Set **Workflow Name** for the variable, list, or object returned by this activity.

Now this microflow triggers the selected workflow:

{{< figure src="/attachments/studio/workflows/call-workflow-example.jpg" alt="Call Workflow Example" >}}

## 3 Workflow App Template

You can use a workflow-specific **Approval app** template to configure an approval request form for end-users. Based on this form the app is be created that contains preconfigured elements, such as dashboards, admin pages, dashboards, and a workflow that you can afterwards customize even more.

When [creating an app in the Developer Portal](http://new.mendix.com/), choose the **Approval app** in the **Starting Point** section to use the app template. 

## 4 Workflow Context Parameter

A [workflow parameter](/studio/workflow-parameter/) is input data for your workflow. The **WorkflowContext** parameter represents a business-related data that travels through the workflow:

{{< figure src="/attachments/studio/workflows/parameter.jpg" alt="Workflow Parameter Example" >}}

For more information, see [Workflow Context Parameter](/studio/workflow-parameter/). 

## 5 Toolbox Elements

The **Toolbox** tab contains elements that you can drag and drop on a path. Below is a categorized overview of all elements. The following sections are used:

* [General](#general)
* [User actions](#user-actions)
* [System actions](#system)

A microflow action can be exposed in Studio Pro as a custom action in the workflow toolbox in both Studio and Studio Pro. This functionality is particularly useful if you plan to reuse the microflow logic several times. Actions that are exposed appear in the custom category in the **Toolbox**. For more information on exposing a microflow action in the workflow toolbox, see [Adding a Custom Action to the Workflow Toolbox](/refguide/add-action-to-workflow-toolbox/) in *Studio Pro 9 How-tos*.

### 5.1 General {#general}

Elements in the **General** section help you control the workflow path, for example, add parallel paths or end them:

{{< figure src="/attachments/studio/workflows/general.jpg" alt="General Section" >}}

The elements of this section are described in the table below:

| Element                                                      | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Start event                                                  | Start event is the starting point of a workflow. Workflows are triggered either by the [Call workflow](/studio/page-editor-widgets-events-section/#call-workflow) on-click event on pages or by the [Workflow call](/studio/microflows/#microflow-workflow-activities) action in microflows. <br />Click the start event to open [workflow properties](/studio/workflow-properties/). |
| [Annotation](/studio/workflows-general-activities/#annotation) | **Annotation** is used to put comments to a flow.            |
| [Decision](/studio/workflows-general-activities/#decision)   | **Decision** makes a choice based on a condition and follows one and only one of the outgoing paths. |
| [Jump activity](/studio/workflows-general-activities/#jump)  | The **Jump** activity allows you to jump to other activities in the workflow. |
| [Parallel split](/studio/workflows-general-activities/#parallel-split) | **Parallel split** adds two or more parallel paths to your workflow. |
| [End activity](/studio/workflows-general-activities/#end)    | End activity ends the path of the workflow                   |

### 5.2 User Actions {#user-actions}

[User task](/studio/workflows-user-task/) – a central element in a workflow that allows you to assign a task to a certain user or a group of users using filters or microflows. 

{{< figure src="/attachments/studio/workflows/user-actions.jpg" alt="User Actions" >}}

### 5.3 System Actions {#system}

The elements of this section allow you to [call a microflow](/studio/workflow-system-actions/#call-microflow) or [call another workflow](/studio/workflow-system-actions/#call-workflow):

{{< figure src="/attachments/studio/workflows/system-actions.jpg" alt="System Actions" >}}

## 6 Main Documents in This Category

* [Workflow Context Parameter](/studio/workflow-parameter/) – describes the Workflow Context parameter and its properties 
* [Workflow Properties](/studio/workflow-properties/) – describes workflow properties 
* [User Task](/studio/workflows-user-task/) – describes properties of a user task 
