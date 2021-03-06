**MB-500: Microsoft Dynamics 365: Finance and Operations Apps Developer**

**Lab 1 – Development Environment Configuration**

Change Record
=============
<table>
<tr><th>Version</th><th>Date></th><th>Change</th></tr>
<tr><td>1.0</td><td>10 Jan 2020</td><td>Initial release</td></tr>
<tr><td>1.1</td><td>11 Jun 2020</td><td><ul><li>Changed link in Lab Environment to be more direct</li><li>Removed unclear text from Scenario</li><li>Added clarifying instructions to: <ul><li>Exercise 1 prior to step 1</li><li>Exercise 1 between steps 11 and 1</li><li>Exercise 2 step 2</li></ul></li></ul></td></tr>
</table>



Lab Environment
===============

In order to run this lab, you will need:

-   (Optional) A Lifecycle Services account with an environment created

-   An all-in-one demo data VM with

    -   Visual Studio installed, and a Visual Studio subscription. These are
        available for free at
        <https://visualstudio.microsoft.com/dev-essentials/>.

Lab Overview
============

-   Open the Dynamics 365 Finance and Operations Azure-hosted instance

-   You will configure Visual Studio to do development work for Dynamics 365
    Finance and Operations

-   You will create a new project and model for doing the lab

**Estimated time to complete this lab: 15+ minutes**

Scenario
========

In this lab, we will configure the Visual Studio features to work conveniently
with Dynamics 365 Finance and Operations Apps. We will also create a model and a
project, where we will do most of the development work.

Exercise 1: Open Dynamics 365 for Finance and Operations
--------------------------------------------------------

If you have an LCS project and environment provided by your Learning Partner:

1.  In your browser, please type <https://lcs.dynamics.com>

2.  Sign In using the credentials provided to you

3.  Read and accept Terms & Conditions

4.  You will find a Dynamics 365 for Finance and Operations project is already
    created for you to use for this lab

5.  Once you enter the project and scroll in the right, you will find a Development instance is already hosted under the Environment tab. It may also be found in the menu icon under Cloud-hosted environments

    ![Lifecycle Services blades](Images/Lab1Ex1Step5.png)

6.  Select the Start

    ![Start](Images/Lab1Ex1Step6.png)

    button and wait for the environment to start

7.  After a few minutes, refresh the browser and see if you have these two
    buttons

    ![Deployed and Login](Images/Lab1Ex1Step7.png)

    at the right top corner

8.  Select the **Login** button followed by **Log on to environment** option

    ![Login \> Log on to environment](Images/Lab1Ex1Step8.png)

    to launch Dynamics 365 for Finance and Operations browser-based user
    interface

9.  After the environment is up, if you scroll down, you will find the VM
    details as follows

![VM Name](Images/Lab1Ex1Step9.png)

1.  Select the highlighted icon

    ![Looks like a wifi or an eye](Images/Lab1Ex1Step10.png)

    and view the password; click the copy icon to copy it

2.  Select the VM Name link and launch the Remote Desktop session. It will ask
    for credentials. Please provide the credentials from the last step.

If you have a virtual machine provided by your Authorized Lab Hoster:

1.  Log into the machine using the credentials provided to you

Exercise 2: Configure Visual Studio 
====================================

In this exercise, you will configure Visual Studio in the development VM for
Dynamics 365 for Finance and Operations programming.

1.  Search for Visual Studio, and open it as administrator. The following screen will pop up

    ![Visual Studio sign in ](Images/Lab1Ex2Step1.png)

2.  Select the **Sign in** button, enter your credentials and close the form

3.  Open menu **Dynamics 365 \> Options** in Visual Studio and expand **Text Editor**

    Select **All Languages** node:

    1.  Select the Word wrap check box

    2.  Select the Line numbers check box

        ![Options \> Text editor \> All Languages](Images/Lab1Ex2Step3.png)

4.  In the menu **Dynamics 365 \> Options**, expand the **Dynamics 365** node

![Best practices](Images/Lab1Ex2Step3.png)


Select Best Practices node and make sure the following are checked: (All are
under Model Acceptance Test Library – Application Suite and begin with
Microsoft.Dynamics.AX.Framework.)

1.  BestPracticeFramework.UIRules

2.  CodeStyleRules

3.  DataAccessRules

4.  DataEntityRules

5.  DeprecatedElementsRules

6.  MaintabilityRules

7.  StaticCodeValidationRules

5.  In the menu **Dynamics 365 \> Options**, expand the **Dynamics 365** node

    Click Projects node

    1.  Verify that the **Organize projects by element type** check box is
        selected

    2.  Verify that **Synchronize database on build for newly created project**
        check box is selected

![Dynamics 365; Projects. Both boxes should be selected.](Images/Lab1Ex2Step5.png)


6.  Select **OK** to save selections

Exercise 3: Create new Model and Project
========================================

1.  On the Visual Studio menu, click **Dynamics 365**

2.  Select **Model Management \> Create model**

    1.  Model name: DynamicsDevTraining

    2.  Model publisher: D365F&O developer

    3.  Layer usr

    4.  Version 1.0.0.0

    5.  Model description: Dynamics 365 F&O development training

    6.  Model display name: D365 F&O dev training

3.  Click **Next** and select **Create new package** radio button

    ![Create Model \> Select package: Create new package](Images/Lab1Ex3Step3.png)

4.  Click **Next** and choose these under **Select referenced packages**

    1.  Application Foundation

    2.  Application Platform (default selected)

    3.  Application Suite

    4.  ContactPerson

    5.  Directory

        ![Update model parameters \> Select referenced packages: ApplicationFoundation ApplicationPlatform ApplicationSuite](Images/Lab1Ex3Step4.png)

5.  Click **Next** and in the **Summary** screen, check the given options, and
    select **Finish**

    ![Summary screen: Make sure that "Create new project" and "Make this my default model for new projects" are selected](Images/Lab1Ex3Step5.png)

6.  **New Project** pop-up will appear with **Dynamics 365 \> Unified
    Operations** as the default template selected

7.  Provide Project & Solution name as follows and select **OK** button

    ![New Project \> Installed \> Templates \> Dynamics 365. Name: DynamicsDevProject Solution name: DynamicsDevSolution](Images/Lab1Ex3Step7.png)

8.  Your new project should appear in the Solution Explorer

    ![Solution Explorer \> DynamicsDevProject](Images/Lab1Ex3Step8.png)

9.  Right click the project, select **Properties**, and set the value of
    *Company* to USMF. Select **Apply** and **OK**

Check Output
============

Please ensure you have created the model & project in this lab. Nothing else to
check.
