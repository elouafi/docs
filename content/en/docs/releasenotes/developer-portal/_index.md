---
title: "Developer Portal"
url: /releasenotes/developer-portal/
description: "Release notes for all project management parts of the Mendix Developer Portal"
tags: ["developer portal", "buzz", "mendix profile"]
weight: 20
#This document is mapped to the landing page, update the link there if renaming or moving the doc file.
---

These release notes cover changes to the app management functionality and other features of the [Mendix Developer Portal](/developerportal/).

{{% alert color="info" %}}
For release notes on Mendix Cloud and deployment options, see [Deployment](/releasenotes/developer-portal/deployment/).
{{% /alert %}}

To see the current status of the Mendix Developer Portal and Control Center, see [Mendix Status](https://status.mendix.com/). Here you can also see planned maintenance and past incidents.

## 2023

### April 4th, 2023

#### Improvements

* We are making the option to migrate your app to Git more prominent. The banner is now displayed on all pages within the **Collaborate** section of the Developer Portal. Read more information on how to migrate and if you are eligible to migrate [here](/developerportal/collaborate/migrate-to-git/).
* Have you tried [Epics](/developerportal/collaborate/epics/) yet? You should! It is awesome if we do say ourselves. We are also working in the background to make it possible to connect your Mendix apps to your Jira boards – stay tuned!

### March 23rd, 2023

#### Improvements

* In preparation for the [merging of Studio and Studio Pro](https://www.mendix.com/blog/coming-in-2023-the-merging-of-studio-and-studio-pro/), we removed the **Edit in Studio** button. You can still open your app in Studio via the ellipsis (**…**) in the [app tile](/developerportal/#my-apps) on the **My Apps** page.
* After the big overhaul we released on [February 13th](#feb-13-23), our logging showed a decrease in the overall performance of [Stories](/developerportal/collaborate/stories/). We took some counter-measures and made performance improvements.
* We made some minor improvements to the flow for [inviting app team members](/developerportal/collaborate/team/#inviting). For example, when you invite someone new to your app, the default role will be **Business Engineer** (as long as this role exists in your app).
* We made some improvements to the layout of the [App Buzz](/developerportal/collaborate/buzz/#app-buzz) page so that it displays better on small screen resolutions.
* The left-hand app sidebar menu is now collapsible, which makes for a far better experience on small screen resolutions.
* You can now create and manage personal access tokens (PATs) in **User Settings** > **Developer Settings**. This location replaces the Warden tool that was previously used. For more information, see the [Personal Access Tokens](/developerportal/community-tools/mendix-profile/#pat) section in *Mendix Profile*.
* We are preparing the Developer Portal for a brand new feedback experience. Please stay tuned!

### March 16th, 2023

#### Improvements

* In Control Center, we increased the limit of apps you can [activate or deactivate](/developerportal/control-center/#active-deactivated) to 100.
* We added the **Contributor** access role in [Portfolio Management](/developerportal/portfolio-management/#access-management), and we renamed the **User** access role to **Viewer**.

#### Deprecations

* We have deprecated **General Settings** > **Webhooks** for stories and Sprints. For more information, see the deprecation note in the [Webhooks](/developerportal/collaborate/general-settings/#webhooks) section of *General Settings*. You can now set webhooks for building and deploying your app. These are described in [Webhooks](/developerportal/deploy/webhooks/).

### March 9th, 2023

#### Improvements

* As of now, only Scrum Masters can [manage the app team](/developerportal/collaborate/team/#managing).
* We simplified the way your [Notification](/developerportal/community-tools/mendix-profile/#notifications) settings are stored.

#### Fixes

* We fixed an issue where the users you administered for your app's [environment](/developerportal/collaborate/general-settings/#manage-users) were not displayed in the correct order.

### February 23rd, 2023

#### New Features

We have released a feature in Control Center where you can add and manage a [Security Contact](/developerportal/control-center/#company-details) for your company. A Security Contact is informed if there are critical security issues with the Mendix Platform and platform-supported Marketplace components.

With this feature, you can do the following:

* Add a new Security Contact to your company
* Remove an existing Security Contact and replace it with a newer one
* Adjust the Security Contact’s name 

For more information on security issues, see [Security Advisories](/releasenotes/security-advisories/).

#### Fixes

* We fixed a performance issue that occurred when opening an [App Buzz](/developerportal/collaborate/buzz/#app-buzz) page for an app with a large team. We now show no more than 25 team members in the team list in the right corner at a time.
* We fixed an issue where the country of residence you selected during sign-up was not properly stored in your [Mendix Profile](/developerportal/community-tools/mendix-profile/#profile).

### February 16th, 2023

#### Improvements

* We enabled more options for search in [Epics](/developerportal/collaborate/epics/). On the [Board](/developerportal/collaborate/epics/#board) page, you can now search stories based on tags, epic name, assignee (and unassigned stories), story title, and story ID. On the [Planning](/developerportal/collaborate/epics/#planning) page, you can search stories based on tags, epic name, assignee (and unassigned stories), status name (only in the Scrum workflow), story title, and story ID.
* The Epics listed on the [Epics](/developerportal/collaborate/epics/#epics) overview page now have visible tags.

#### Fixes

* We fixed an issue in **Epics** where the unsaved changes pop-up window did not take you to the correct story after clicking **Leave**.
* We updated the text in the [notifications](/developerportal/#notifications) when a story is assigned to you in **Epics**.

### February 13th, 2023 {#feb-13-23}

#### Improvements

* We overhauled the entire [Project Management](/developerportal/collaborate/general-settings/#project-management) to a completely new design. This design brings the benefit of using the full body width of your screen, scales much better across several devices and screen resolutions, and is dark-mode ready.
* Have you lost track of where your apps live? We now display the cloud plan on the app tile in [My Apps](/developerportal/#my-apps).
* We moved the notification settings you set for your app management to **Account Settings** > [Notifications](/developerportal/community-tools/mendix-profile/#notifications) (which you can access via the menu beneath your avatar in the top bar). This page includes a list of the apps you are watching.
* We simplified the [team member invitation](/developerportal/collaborate/team/#inviting) flow from a multi-step wizard to a single page.
* We moved the **Pending Invites** to a tab on the [My Apps](/developerportal/#my-apps) page. You will find both the pending invitations to apps that you have received (which you can **Accept** or **Decline**) in addition to the invitations you have sent. 
* In addition, personal **API Keys** are available via **Account Settings** > [Developer Settings](/developerportal/community-tools/mendix-profile/#dev-settings).

#### Fixes

* We fixed a performance issue on the [Team](/developerportal/collaborate/team/) page.

### January 26th, 2023

#### Improvements

* We fixed an issue where the story description did not appear in Studio Pro.
* [Epics](/developerportal/collaborate/epics/) now have different colors so that you can distinguish between them more easily. The color is currently assigned randomly (as is done with story labels), but we may add management functionality at a later point.
* If you practice Scrum, you can now see the status of the stories in your active Sprint on the [Planning](/developerportal/collaborate/epics/#planning) page.
* Sprint details are now editable, so you can change the date, name, and goal of your Sprint after you start it. Use this power wisely, as committing to a Sprint goal is important, so only change the goal if there really is no other option.
* We have implemented the new [Mendix Feedback](/appstore/modules/mendix-feedback/) module, so now you have much better screenshot functionality. Do send us feedback, we love hearing what you think. And also try out the new Mendix Feedback module in your own apps, it's awesome!

## 2022

### December 21st, 2022

#### Fixes

* We fixed an issue where some users were not able to open the [Sprint Status](/developerportal/collaborate/stories/) page.

### December 13th, 2022

#### New Features

We have released the Beta version of [Product Insights](/developerportal/collaborate/product-insights/), which is a new way for you to proactively get feedback from your users. The functionality consists of a tool for setting up mini surveys in addition to the [Product Insights - Mini Surveys](/appstore/modules/product-insights/) Marketplace module, which you can add to your app to set up the exact targeting criteria for a survey.

A survey can have a maximum of three questions that appear in your app based on the implemented criteria. You can choose between four different question types (rating scale, multiple choice, open question, and NPS question), and you can place the survey toaster in any of corner of the page. You can also preview exactly what the survey will look like.

This feature is in Beta, so we would very much appreciate your feedback. If you have any questions or suggestions for improvement, just reach out via the **Feedback** widget on the **Product Insights** page in the Developer Portal.

### December 1st, 2022

#### Improvements

We released a new version of [Epics](/developerportal/collaborate/epics/), our brand new Agile planning tool, for General Availability!

We made the following improvements:

* It is possible to migrate all your data from Stories into Epics. For details, see the [Data Migration](/developerportal/collaborate/epics/#data-migration) section of *Epics*.
* You can link a feedback item to a story in Epics. If you accept feedback, the story with the feedback ID and the link to the original issue will show up in your backlog.
* If you type *#* and then start typing a story name, you can link a story in the description of another story. This is handy for showing dependencies or other relationships between stories.
* Mentioning app team members with *@* is available in story and epic descriptions as well as in comments. If someone *@* mentions you, it triggers a notification on the Mendix Platform and/or an email, depending on your notification settings.
* We have added emoji reactions to comments, for those times when there is no need to bother typing a message because a simple thumbs-up says it all.

From this point on, Epics is the default project management tool for all new apps.

### November 30th, 2022

#### New Features

The new [Portfolio Management](/developerportal/portfolio-management/) tool allows portfolio managers, business stakeholders, and developers to stay informed about projects and manage them in the different development stages. By providing everything you need to collaborate effectively in one place, it is now easier than ever to bring project ideas to the Mendix Platform.

In Portfolio Management, you can do the following

* Control and manage digital project initiatives in one overview (via Kanban and list views)
* Prioritize project initiatives by industry standard prioritization methods:
    * Weighted shortest jobs first (WSJF)
    * Reach, impact, confidence, and effort (RICE)
* Sort, filter, and search project initiatives on fields such as **Tags**, **Owners**, **Departments**, and **Dates**
* Add attachments, link Mendix apps, and assign owners to a project initiative
* Archive and restore project initiatives
* Invite users to dedicated portfolio boards (both internal to your organization and external)
* Easily manage portfolio users via **Access Management**
* Get notified when you get assigned to a project initiative or someone commented on a project initiative you own

### November 21st, 2022

#### New Features

* We introduced a self-service option for Team Server SVN that allows Scrum Masters to permanently migrate eligible apps to Git. For more information on what apps are eligible for migration and on the migration process, see [Migrate to Git](/developerportal/collaborate/migrate-to-git/). For more information on steps after the migration and process differences between Git and SVN, see [Migrating from SVN to Git: Steps After Migration and Process Differences](/refguide/svn-git-differences/).

### November 10th, 2022

#### Improvements

* We improved the way [Company Brand](/developerportal/control-center/#company-brand) is stored and distributed. The company logo that is uploaded in Company Brand will be updated throughout the platform where it is used.
* We removed the Brand Colors feature for Company Brand.

### October 20th, 2022

#### Fixes

* We fixed an issue where the story name in the revision history was not visible when you link a commit to a story in Epics or Jira (Beta).

### October 6th, 2022

#### Improvements

* You can now see your app history under the [General Settings](/developerportal/collaborate/general-settings/#history) page. Previously this was located under the **Stories** page.

#### Fixes

* We fixed an issue which could occur when you try to accept feedback items with a long description.
* We fixed an issue where the feedback description was not always scrollable.

#### Deprecations

* All [Mendix Feedback](/appstore/modules/mendix-feedback/) widgets with versions lower than 8.4.0 are disabled. The feedback provided via a widget version lower than 8.4.0 is no longer sent to the [Feedback](/developerportal/collaborate/feedback/) section of the Developer Portal, but your app will keep working as usual. Please download and replace your current Mendix Feedback widget with version 8.4.0 or higher. If you are using the [Native Mobile Resources](/appstore/modules/native-mobile-resources/) module (which also includes a version of the Mendix Feedback widget), please upgrade to version 3.5.1 or higher of that module. 

### September 28th, 2022

#### New Features

* We replaced the widget used in story description in [Epics](/developerportal/collaborate/epics/) with a new one, which fixes the bug you might have been experiencing. This replacement also comes with the following changes:
    * You can use @ to mention someone in the text of story description or epic objective. The mentioned person will get a notification once the text is saved.
    * You can copy the link to a story or an epic on the upper-right corner of the [story details](/developerportal/collaborate/epics/#story-details) dialog box or the [epic details](/developerportal/collaborate/epics/#epic-details) dialog box.
    * Story and epic details now appear in a dialog box instead of a side pane.
    * The widget styling is now slightly different.
* We added a **Project Buzz** button on the [Board](/developerportal/collaborate/epics/#board) page. Clicking the button brings you to the [Buzz](/developerportal/collaborate/buzz/#app-buzz) page of the specific app in the Developer Portal.
* We added an error page in case you access Epics with no apps enabled.
* We made it possible for you to link commits from Studio Pro to stories in Epics.

#### Improvements

* We improved some empty states in the story details dialog box, epics details dialog box, archived Sprint details dialog box, and archived story details dialog box in Epics.

### September 15th, 2022

#### New Features

* We added the option to watch and unwatch an app. You can find this option on the [General Settings](/developerportal/collaborate/general-settings/) page for an app as well as when you click the ellipsis (**...**) in an app tile on the [My Apps](/developerportal/#my-apps) page. Watching an app means that you will receive feedback notifications for this app, while unwatching an app turns off the notifications.
* We introduced the [Billing Accounts](/developerportal/control-center/#billing-accounts) page in Control Center where Mendix Admin can update the payment card information for their company at any time.

#### Fixes

* We fixed an issue where users were not able to delete an app, if other users were still members of this app.
* We fixed a navigation issue that would occur when users click **Go to Environments** in [Cloud Settings](/developerportal/collaborate/general-settings/#cloud-settings).

### August 25th, 2022

#### Fixes

* We fixed an issue where Mendix Admins were not able to invite users to their company's apps.
* We fixed a pagination issue on the [user management overview](/developerportal/collaborate/general-settings/#manage-users) in your **Access Management** settings.

### August 22nd, 2022

#### New Features

* We have changed the password reset flow:
    * You can no longer update your password from your Mendix Profile.
    * All password resets and changes are now done via the [New Password Request page](https://login.mendix.com/mxid3/request-password-reset), which you can reach using the **Forgot password?** link on the login screen. This will send a password reset link to your registered email address.
* We introduced a separate session duration of one hour for users logging into the platform using SSO with their companies BYOIDP, so session management can be better controlled by their IDP.

### August 11th, 2022

#### New Features

* We have introduced the [Marketplace Content](/developerportal/control-center/#marketplace-content) page in Control Center, where Mendix Admins can manage the visibility of Marketplace Content in Studio.
* We simplified the process of [inviting other users](/developerportal/collaborate/team/#inviting) to your projects. Now you do not need to add a personal message to the invitation anymore and the whole process can be completed on a single page.
* We added a banner about [Epics](/developerportal/collaborate/epics/), our new tool for Agile planning, on the [Stories](/developerportal/collaborate/stories/) page. This banner provides more information about Epics and makes it easier for Scrum Masters to enable it for their projects.  

### August 9th, 2022

#### New Features

* We released [Notifications](/developerportal/#notifications) for Beta usage, which allows you to receive updates from Academy, Data Hub, Developer Portal, Epics, and Forum. Additionally, you can manage what kind of updates you will receive in the [Notification Settings](https://user-settings.mendix.com/link/notifications) page.

### July 21st, 2022

#### Improvements

* We removed **My Activity Overview** from the **Account Settings** page.
* We redesigned the **Pending App Invites** section and added it as a new menu item to the **Account Settings** page.
* We improved the warning messages when you leave or delete an app.

#### Fixes

* We fixed an issue where apps on the **Company Apps** page would not be displayed properly.
* We fixed an issue that would cause an error when you edit a very long app name or description on the **General Settings** page.

### July 14th, 2022

#### Improvements

* We removed the profile buzz page.
* We made some small improvements to the **General Settings** page.

### July 7th, 2022

#### New Features

* We released [Epics](/developerportal/collaborate/epics/), our brand new tool for Agile planning, for Beta usage. Epics has many features. For example, you can:

    * Map your exact development process with fully customizable swimlanes
    * Use Scrum or Kanban – we support both!
    * Set Sprint goals and see all the basic Sprint information on the board – if you are using Scrum
    * Drag and drop stories on our brand new project board
    * Format stories in any way you want – for example, adding headers, links, and code blocks, linking specific stories, and using @ to mention people (notifications for this coming soon!)
    * Clone stories
    * Create and track the progress of epics
    * Archive single stories or whole swimlanes
    * Easily search through your completed stories and get an overview of completed Sprints in the archive

    You can try it out for any Mendix app. Your Scrum Master just needs to enable Epics in the [General Settings](/developerportal/collaborate/general-settings/#project-management). Please note it is not yet possible to migrate the data from Stories into Epics, so we recommend using it for new projects or iterations first – in this way you do not have to worry about the stories in your current backlog.

### June 30th, 2022

#### Fixes

* We introduced improvements in the performance of the [Feedback API](/apidocs-mxsdk/apidocs/feedback-api/).

#### New Features

* We redesigned the [General](/developerportal/collaborate/general-settings/) settings section to make it more intuitive and user-friendly.
* We prepared the integration of Studio Pro with our new project management tool, Epics (coming soon!).

### June 16th, 2022

#### Fixes

* We fixed an issue where users with an invalid Twitter URL in the **Social** section of their Mendix Profile Settings could not change their password.
* We fixed an issue where users could have a duplicated project membership, resulting in two identical projects in the Developer Portal.

### June 9th, 2022

#### New Features

* The free Mendix Cloud environment of an app can now be deleted from the [app details](/developerportal/control-center/#app-details) page in Control Center.

#### Improvements

* The free and licensed Mendix Cloud environments of an app are now visualized on the [app details](/developerportal/control-center/#app-details) page in Control Center.
* From now on, the free Mendix Cloud environment of an app will be deleted whenever the app is deactivated or deleted.

### May 19th, 2022

#### Fixes

* We fixed an issue where replies on [Feedback](/developerportal/collaborate/feedback/) emails were not correctly processed into comments.

#### Improvements

* We added a download button for Feedback images, so that you can see them in full size more easily.

### May 5th, 2022 {#may-fifth}

#### Fixes

* We fixed a known issue where not all app images were displayed correctly on the [My Apps](/developerportal/#my-apps) page. (Ticket 148379)

### April 21st, 2022

#### Improvements

* We removed the old [Stories](/developerportal/collaborate/stories/) UI in preparation for a brand new Mendix tool for Agile project management that will eventually replace **Stories** completely – stay tuned!
* We expanded the export-to-Excel functionality in [Control Center](/developerportal/control-center/) for both the [Apps](/developerportal/control-center/#apps) tab (which includes the **App ID**) and the [Cloud](/developerportal/control-center/#cloud) tab (which includes the **App ID**, **Environment ID**, and **Environment URL**).

#### Known Issues

* Under certain circumstances, the app image is not displayed properly on the [My Apps](/developerportal/#my-apps) page.
    * Fixed on [May 5th, 2022](#may-fifth).

### April 7th, 2022

#### Improvements

* We introduced a new layout of the [Mendix Forum](/developerportal/community-tools/mendix-forum/) that features the following changes:
    * The main navigation has been moved to the left sidebar
    * There is a dedicated for page for your bookmarks
    * Breadcrumb navigation
    * Dedicated pages for Forum content you have interacted with (asked, answered, and commented for questions, and submitted and commented for ideas)

### March 24th, 2022

#### Improvements

* As of today, we send all app invites, [Buzz](/developerportal/collaborate/buzz/) notifications, and the Daily Digest from a no-reply email address. You can still reply to Buzz notifications, by the way.
* We have started sending the Daily Digest in a slightly different markup.

#### Fixes

* We fixed an issue where the submitter of a [feedback item](/developerportal/collaborate/feedback/) was no longer able to comment on that issue after they left the app.

### March 10th, 2022

#### Fixes

* We fixed a bug where screenshots posted through the [Mendix Feedback](/appstore/modules/mendix-feedback/) widget could be viewed in thumbnail size only. It ain't much, but it's honest work. (Tickets 143368, 143399, 143435, 143505, 143526, 143602, 143657, 143681, 143782, 143818, 143838, 143919, 143924, 143965)

#### Improvements

* The apps displayed on the **My Apps** tab that appears when starting Studio Pro are pulled from the [My Apps](/developerportal/#my-apps) page in Developer Portal. In Studio Pro versions below [9.6.0](/releasenotes/studio-pro/9.6/), the **My Apps** tab will no longer display [Git for version control](/refguide/branch-line-manager-dialog/#byo-server-app) apps, as Git integration is not supported. In Studio Pro versions 9.6.0 and above, both Git-enabled and SVN-enabled apps are displayed.

### February 10th, 2022

#### New Features

* We changed the button from favorite to bookmark in the [Mendix Forum](/developerportal/community-tools/mendix-forum/). You can now more easily bookmark posts for future reference.

#### Improvements

* In our continuous effort to change the Developer Portal from a monolith into microservices, we have taken a big step in giving company data its own service. This paves the way for an updated password maintenance experience, which we will release soon.

#### Fixes

* We fixed a bug where editing a new task while [creating a story](/developerportal/collaborate/stories/#new-story) threw an error.

### January 18th, 2022

#### Improvements

* We improved the platform navigation. The [Switch to](/developerportal/#navigation) menu on the left side of the top bar now also provides access to your recently used apps.  

## 2021

### December 23rd, 2021

#### Improvements

* We recently changed the password length requirement from 8 to 12 characters. We noticed this caused some confusion, because not all pages where the password can be reset or changed listed the password requirements. We made sure that all pages now list those requirements.
* During the last release, we introduced an issue where the Developer Portal exposed apps without a repository to Studio Pro. We patched this issue on Friday December 17th, 2021 with a band-aid. This release sees a more permanent solution.

### December 15th, 2021

#### Improvements

* We changed the minimum length of passwords from 8 to 12 characters.

### December 2nd, 2021

#### Fixes

* We fixed an error where it was not possible to edit a comment under a [Feedback](/developerportal/collaborate/feedback/) item. (Tickets 134179, 136172)

### November 18th, 2021

#### Improvements

* The arrival of [Git support](/refguide/branch-line-manager-dialog/#byo-server-app) means that a new version of the [Platform SDK](/apidocs-mxsdk/mxsdk/) is in order. We made some changes to the Developer Portal to accommodate this new version, which is currently being tested and will be published soon.
* We introduced a new version of the [Feedback API](/apidocs-mxsdk/apidocs/feedback-api/) that will be used by a new generation of [Feedback widgets](/appstore/modules/mendix-feedback/) coming to the Marketplace soon.
* Until now, you were not able to delete or deactivate an app if it was still deployed to an environment, regardless of whether it was a licensed environment or a sandbox for a Free App. We changed this behavior so that the only check is on whether the environment is licensed. A consequence of this change is that the cloud icon on the app tiles on the [My Apps](/developerportal/#my-apps) page is only displayed if your app is deployed to a licensed node.

### November 4th, 2021

#### Improvements

* We redesigned the [Stories](/developerportal/collaborate/stories/) archive page to allow you to more easily search through completed stories by ID, name, description, or Sprint.

### November 1st, 2021

#### Update of *.mendixcloud.com SSL/TLS certificate

* We have renewed the SSL/TLS certificate for `\*.mendixcloud.com`. Browsers like Mozilla Firefox, Microsoft Edge, Google Chrome, and Internet Explorer automatically trust the new certificate. In that case, there is nothing you have to do. If you run services that connect to a `\*.mendixcloud.com` endpoint and use a static or outdated trust store, we advise you to update their certificates. The new SSL/TLS certificate can be downloaded [here](/attachments/releasenotes/developer-portal/mendixcloud.com-2021-10-29.crt.txt). This can be done from today, you do not have to wait for the old certificate to expire.
    * Current certificate details:
        * Subject: `*.mendixcloud.com`
        * Issuer: C = US, O = DigiCert Inc, OU = www.digicert.com, CN = RapidSSL TLS RSA CA G1
        * Validity: Sep 12 00:00:00 2019 GMT - Nov 10 12:00:00 2021 GMT
        * SHA-256 Fingerprint: `AE:55:1D:88:32:E1:7E:BF:AB:0D:F3:2F:57:57:C8:98:8D:87:3F:E8:F6:5F:A6:09:82:EA:37:F7:12:25:A5:D3`
        * SHA-1 Fingerprint: `5E:4D:05:9B:FE:54:3F:B6:D8:A4:D7:86:7F:3B:50:9A:EE:09:35:8F`
    * New certificate details:
        * Subject: `*.mendixcloud.com`
        * Issuer: C = GB, ST = Greater Manchester, L = Salford, O = Sectigo Limited, CN = Sectigo RSA Domain Validation Secure Server CA
        * Validity: Oct 29 00:00:00 2021 GMT - Oct 29 23:59:59 2022 GMT
        * SHA-256 Fingerprint: `BF:AE:01:9F:93:5A:D9:92:35:B5:BA:9F:E4:AE:56:99:21:17:44:51:56:17:A2:11:A1:FE:3B:42:9C:B4:B6:70`
                * SHA-1 Fingerprint: `0F:3B:31:9F:86:6E:65:2D:5F:7A:EF:35:64:04:45:67:58:E4:ED:11`

### October 21st, 2021

#### Improvements

* The app [Team](/developerportal/collaborate/team/#managing) overview now shows deactivated users. These users can no longer sign in to the Mendix Platform or contribute to the app, and they were until now hidden from view. By showing deactivated users, app administrators have the opportunity to remove them from the app team.
* During our continuous monitoring, we noticed that creating an app during peak hours caused performance issues and sometimes resulted in timeouts. We mitigated these problems by restructuring the app creation process.

#### Fixes

* We fixed an issue accidentally introduced in the [October 14th](#oct-fourteen) release where you were no longer able to post comments on a [feedback item's details page](/developerportal/collaborate/feedback/#feedback-details). (Tickets 132892, 132959, 132983, 133075)

### October 14th, 2021 {#oct-fourteen}

#### Improvements

* We noticed our **API Keys** overview was not telling the exact truth and made some changes accordingly. Because API keys are cached by our user-provisioning system, when you revoke an API key, it takes a certain amount of time before this is reflected across the platform. A new confirmation message warns you of this.
* We added a [Team Server revision history](/developerportal/collaborate/team-server/#revision-history) overview page for your Git-enabled apps. This allows you to have an overview of the last 40 commits made in your app. You can filter the overview per branch. When a revision is linked to a user story, the Team Server page can bring you to the [story details](/developerportal/collaborate/stories/#story-details) page.

#### Fixes

* We fixed an issue where you could not see the story details if one of the tasks had a title that was longer than 200 characters.

### October 1st, 2021 {#oct1}

#### New Features

* We have released the company [Onboarding](/developerportal/control-center/#onboarding) functionality in Control Center that enables setting up Mendix onboarding specifically for all new members of your company. You can set up an onboarding email that new users get as soon as they create their Mendix accounts and a company onboarding page that new users land on.

### September 23rd, 2021

#### Improvements

* We simplified the drag-and-drop behavior on the [Stories Overview](/developerportal/collaborate/stories/#overview) page (for both the new and old UI) to make it more stable.
* We added support for adding labels to stories on the **Stories Overview** page.
* It is now possible to add labels and tasks as well as assign a team member when you [create a story](/developerportal/collaborate/stories/#new-story).
* Thanks to a lot of feedback from the community, we have improved the new stories functionality to the point where we feel comfortable removing the old UI. Because of this, we will be deprecating the old UI on December 31st, 2021.
* We improved the look and feel of the [story details](/developerportal/collaborate/stories/#story-details) page, and we removed support for the old version of this page.
* We made further preparations for the support of Git-enabled apps.
* We finished a year-long project where we modernized the way the Developer Portal communicates internally. This meant we removed a long-running internal platform app, which had a great run, but now it is time to say goodbye. This app has been replaced with business events based on Kafka.

#### Fixes

* We fixed an issue where an error was shown when a Sprint was created from the [Stories](/developerportal/collaborate/stories/#new-sprint) page.

### September 13th, 2021

#### Improvements

* Your [Mendix Profile](/developerportal/community-tools/mendix-profile/) got a visual update.
* We removed the possibility to add a GitHub account to your profile.

### September 6th, 2021

#### New Feature

* Mendix Admins can now configure their own [single sign-on](/developerportal/control-center/set-up-sso-byoidp/) configuration from the [Security](/developerportal/control-center/#security) tab of Control Center. 

### September 2nd, 2021

#### Improvements

* We removed the **Burndown Chart** and the **Release Plan** from **Stories**. We are working on reintroducing solutions for project analytics and release planning in the future.
* We implemented [context deep links](/developerportal/collaborate/manage-deeplinks/) to all main app pages on the Developer Portal so you can easily share references.
* We increased the performance of opening the [My Apps page](/developerportal/#my-apps)

#### Fixes

* We fixed a bug where the pop-up window with pending invitations was shown twice.
* We also fixed a layout bug on the invitation pop-up window that we accidentally introduced during the last release.

### August 26th, 2021

#### Improvements

* We added a new menu item for Mendix Admins to access [Data Hub](/developerportal/control-center/#data-hub) tasks in Control Center. For details, see [Data Hub Administration](/developerportal/control-center/data-hub-admin/).

### August 19th, 2021

#### Improvements

* We implemented the first batch of endpoints for mobile, in preparation for something cool coming your way.
* We improved the way the Developer Portal shares data across its several components.
* We made small improvements to the look and feel of the Developer Portal.

#### Fixes

* We fixed an issue with the app's [Team](/developerportal/collaborate/team/) page where [Mendix Admins](/developerportal/control-center/#company) could not add or remove team members.

### July 27th, 2021

#### Improvements

* We improved the **External Members** overview on the Control Center [Dashboard](/developerportal/control-center/#dashboard) so that a list of external members from a specific company appears when you click a part of the pie chart.

### July 14th, 2021

#### Improvements

* We updated the look and feel of the [Documents](/developerportal/collaborate/documents/) page.

### June 30th, 2021

#### Improvements

* You can now assign team members to a [user story](/developerportal/collaborate/stories/#story-details).
* We moved the old version of the Stories UI. You can now access it via the [More](/developerportal/collaborate/stories/#more) button on the **Stories** page.
* We removed the **Team** read-only overview page and send you straight to the [Manage Team](/developerportal/collaborate/team/#managing) page.
* We moved the **API Keys** page to the [General Settings](/developerportal/collaborate/general-settings/#general-settings-api-keys) page.
* We implemented a new responsive search panel.
* We will remove the **Burndown Chart** and **Release Plan** tabs from the Developer Portal on August 31st, 2021.

### June 15th, 2021

#### Improvements

* Git is coming: we have prepared the Developer Portal for the handling of Git-supported apps.
* We added a button to the [Stories](/developerportal/collaborate/stories/) overview that allows you to [create a new label](/developerportal/collaborate/stories/#new-label).
* We made some minor changes to the look and feel across the Developer Portal.

#### Fixes

* We fixed a broken link to the documentation on the [Team Server](/developerportal/collaborate/team-server/) page.

### June 1st, 2021

#### Improvements

* We added a tab on the [Cloud](/developerportal/control-center/#cloud) page in Control Center that displays details on **Free Environments**.
* We are deprecating part of the options to create an app based on an app template. As of June 20th, 2021, you can no longer create apps through the [Projects API](/apidocs-mxsdk/apidocs/projects-api/) or the [Developer Portal](/developerportal/#navigation) using app templates created in Desktop Modeler version [7.23.14](/releasenotes/studio-pro/7.23/#72314) or below. Please update your templates to [7.23.15](/releasenotes/studio-pro/7.23/#72315) or above before creating apps based on those templates.

### May 17th, 2021

#### Improvements

* We made some minor changes to the look and feel over several pages, buttons, and UI components in line with the recent redeisgn of Mendix Developer Portal.

#### Fixes

* We fixed an issue where you could not always see the avatars of other users in the same app.
* We fixed an issue where there were styling glitches visible when adding a description to a newly created [story](/developerportal/collaborate/stories/).
* We fixed an issue where Mendix Support was not always able to adjust app permissions on behalf of customers.

### May 7th, 2021

#### New Features

* It is now possible to create a new app with the [workflows](/refguide/workflows/) functionality more deeply integrated in the creation flow.

#### Fixes

* We fixed an issue where some graphs in the Contral Center [Dashboard](/developerportal/control-center/#dashboard) were loading indefinitely. 
* We fixed the page title of the [Mendix Studio](/studio/) landing page.
* Page links now open in the correct tab.

### April 26th, 2021

#### New Features

* We released the Control Center [Dashboard](/developerportal/control-center/#dashboard), which provides an overview of various activities for your company on the Mendix Platform. This feature is currently in [Beta](/releasenotes/beta-features/), and you can provide feedback via the feedback button on the right of the page.

### March 30th, 2021

#### Improvements

* We have released our new [platform navigation](/developerportal/) solution with these main features:
    * The **Switch to** menu on the left side of the top bar provides access to different parts of the Mendix Platform.
    * The top bar contains sub-navigation items (for example, **Company Buzz**).
    * Clicking the **+** button on the right side of the top bar will create a new app from anywhere in the platform.
    * Under your avatar on the right side of the top bar, there is an option to switch off the new navigation, which will be available for a limited amount of time.
* We improved the search experience and added a full page of search results that can be accessed by clicking **View Search Results Page** at the bottom of the search drop-down menu or by pressing <kbd>Enter</kbd> after typing a search query
* We changed the [My Apps](/developerportal/#my-apps) page and moved your favorite apps to the **Pinned** tab. This will become the default tab on this page, making it easy to quickly access the apps you care about the most.
* You asked and we listened: We added new label colors for labels in [Stories](/developerportal/collaborate/stories/). There are now 15 different colors to choose from, specifically selected with accessibility in mind.
* We made some big changes to the look and feel of our Developer Portal:
    * We reshuffled the navigation items in the [App Buzz](/developerportal/collaborate/buzz/#app-buzz) to a more logical order, based on our research insights. Now, there are two main sections: **Collaborate** and **Deploy**.
    * We updated the look of various navigation items (**Feedback**, **Planning**, **Team Server**, **General**) to our new design.
    * We removed the grey background with white card content in all pages.
    * We replaced the breadcrumbs in the top left corner of the project navigation with the app name and icon.

#### Fixes

* We fixed an issue where sending feedback from Studio Pro resulted in an error. (Tickets 113634, 115031)

### March 26th, 2021

#### Improvements

* We made some small improvements to the **App Templates** page.

### March 15th, 2021

#### Fixes

* We fixed a bug where it was not possible to open a version 6 Desktop Modeler from the Developer Portal.

### March 10th, 2021

#### Fixes

* We fixed a bug where selecting an IBM or SAP template in the **Create App** flow did not direct you to the right page. 

### March 9th, 2021

#### Improvements

* In Control Center, Mendix Admins can now edit the name and description of an [App Access Group](/developerportal/control-center/#groups) once it has been created.
* Mendix Admins can now [deactivate](/developerportal/control-center/#members) Technical Contacts and the last Scrum Master in a team.

### March 4th, 2021

#### Improvements

* We made some minor changes to the look and feel over several pages, most notably the [General Settings](/developerportal/collaborate/general-settings/) page.
* We removed the old Company Admin pages. But you are already using the [Mendix Control Center](/developerportal/control-center/) as a Mendix Admin, right?
* We made some preparations for Git support.
* We improved the sharing of data across the Developer Portal so that it is more stable and secure.

#### Fixes

* We fixed an issue where the **Add image** icon was missing when posting a comment on the [Buzz](/developerportal/collaborate/buzz/). (Ticket 109481)
* We fixed an issue where creating API keys appeared in the audit trail. (Ticket 116182)

### February 25th, 2021

#### Improvements

* We optimized the **App Templates** page for a better experience. We also improved the search function on this page.
* There is now better performance for building your app after you select a template.

### February 23rd, 2021

#### Improvements

* We have updated the [App Projects](/developerportal/control-center/#apps) tab of Control Center, where you can now do the following:
    * Open the [Team](/developerportal/collaborate/team/#managing) page from the project details page in order to manage team members and add yourself to a team (if you are a Mendix Admin)
    * Deactivate or delete an app or a team member

### February 9th, 2021

#### Improvements

* We improved the speed of the **App Templates** page. After you click **Create App**, the templates appear instantly now.

### February 5th, 2021

#### Improvements

* It is now possible to add or remove labels in the [Story Details](/developerportal/collaborate/stories/#story-details) page.
* We added a link to your app's [environments](/developerportal/deploy/environments/) in the app tile on [My Apps](/developerportal/#my-apps).

#### Fixes

* We fixed an issue where new Mendix Admins did not get access to environment nodes. (Ticket 114913)

### February 4th, 2021

#### New Features

* We released the Mendix [Control Center](/developerportal/control-center/), which provides governance and control features for Mendix Admins (formerly known as Company Admins).

#### Improvements

* We moved the existing Company Admin features in the Developer Portal to Control Center.

### January 24th, 2021

#### Improvements

* We removed support for the **Country** and **Skype** attributes in your [Mendix Profile](/developerportal/community-tools/mendix-profile/).
* You can no longer create new polls on the company or app [Buzz](/developerportal/collaborate/buzz/) page. Existing polls can still be answered.

#### Fixes

* We fixed several minor issues with the [My Apps](/developerportal/#my-apps) page.

### January 15th, 2021

#### Improvements

* We redesigned the [My Apps](/developerportal/#my-apps) page.
* You will now see labels when you are editing a [story](/developerportal/collaborate/stories/#story-actions) using the new **Stories** UI. We will enable the editing of story labels and label colors in a future release.

#### Fixes

* We fixed an issue where newly-added Company Admins did not get access to edit [user groups](/appstore/general/app-store-overview/#user-groups) in the Marketplace.

## 2020

### December 23rd, 2020

#### Improvements

* We tweaked the styling of the **Stories** > **Project History** page.
* We made [moving a story](/developerportal/collaborate/stories/#move-stories) to another app more intuitive.
* We removed the Model page, which contained tips on how to get started creating your apps.

#### Fixes

* We fixed an issue where replies to Buzz notifications were not properly processed into comments on your [app Buzz](/developerportal/collaborate/buzz/#app-buzz) page. (Ticket 111076)

### December 2nd, 2020

#### Improvements

* We changed the home page of the Developer Portal to [My Apps](/developerportal/#my-apps).

### November 4th, 2020

#### Fixes

* We fixed a bug where a change of company name was not properly distributed along the platform.
* We fixed a bug where drop-down menus were cut off on the [story details](/developerportal/collaborate/stories/#story-details) page.

### October 9th, 2020

#### Fixes

* We fixed an issue where team members were not displayed in the [Team](/developerportal/collaborate/team/) overview.

### October 4th, 2020

#### Improvements

* We redesigned the [story details](/developerportal/collaborate/stories/#story-details) page and made it available for Beta usage. You can use the new design when the new story UI is enabled. Please note that it is currently not possible to add or manage [labels](/developerportal/collaborate/stories/#managing-labels) with the new UI; this functionality will be released in the future.
* When you add a [task](/developerportal/collaborate/stories/#adding-task) to a commit of your app model, we now show the revision in the revision overview of the story details. Clicking the task will bring you to the story details page to which the task belongs.
* We simplified the **Company Settings** tab of the **Company** page by removing some barely used attributes.

#### Fixes

* We fixed an issue where the default avatar of a team member who committed a revision was not properly displayed in the revision overview of the story details.
* We fixed an issue where a Company Admin was no longer able to open the [General Settings](/developerportal/collaborate/general-settings/) of an app they for a team in which they were not a member.
* We repaired a dead link to the documentation on the [App User Management](/developerportal/collaborate/general-settings/#managing-app-users) page.

### August 25th, 2020

#### Improvements

* We reintroduced the read-only authorization for the [user story](/developerportal/collaborate/stories/) overview.

#### Fixes

* We fixed an issue where, under certain circumstances, email notifications were not sent on [story comment](/developerportal/collaborate/stories/#story-details) updates.

### August 11th, 2020

#### Improvements

* We made some small performance improvements.

#### Fixes

* We placed a deprecation warning in a file hosted by the Developer Portal that is used in old versions of the [Mendix Feedback](/appstore/modules/mendix-feedback/) widget. As of October 1st, 2020, we will end support for Mendix Feedback widget version 5 or below. Please always keep your Feedback widget up-to-date to ensure the best experience for your users.
* We fixed an issue where you could move a user story to a different Sprint without specifying the target Sprint.

### July 28th, 2020

#### Fixes

* We fixed an issue where email notifications on [feedback](/developerportal/collaborate/feedback/) items were not sent under certain circumstances.

### July 13th, 2020

#### Improvements

* We increased the performance on opening the buzz page.
* We changed the default avatar of a user profile from the Mendix logo to an industry standard user-icon.

#### Fixes

* We fixed a bug where, under certain circumstances, the "View App" was disabled even though it should have been enabled.

### June 28th, 2020

#### Improvements

* We implemented the second increment in renaming the default **End-user** team role to [Guest](/developerportal/collaborate/app-roles/#team-roles).

#### Fixes

* We fixed an issue where it was possible to change the end date of a closed Sprint.

### June 15th, 2020

#### Improvements

* The [new Stories UI](/developerportal/collaborate/stories/) has been improved with various sections. The old Stories UI will be made unavailable soon. We encourage you to turn your tasks that are still available in the old Stories UI into new stories before the old UI is inaccessible.
* We improved performance on story-related actions such as drag-and-drop and status changes on large apps with many deleted items.
* We renamed the default **End-User** team role to [Guest](/developerportal/collaborate/app-roles/#team-roles) to better distinguish team roles from app user roles.
* We removed the list appearance of the [My Company's Apps](/developerportal/#my-company-apps) page.

#### Fixes 

* We fixed a bug where the background did not display properly on mobile browsers.
* We fixed a bug where changes to a story title or description were saved when clicking **Cancel**.

### May 27th, 2020

#### Improvements

* When you delete a story or task on the [Stories](/developerportal/collaborate/stories/) page, it is now irreversibly removed from the system.
* We removed the ability to revert story-related changes in an app's history.
* We removed the ability to delete several stories at once on the **Stories** page.
* We simplified story maintenance by preventing nested tasks.
* We removed the read-only permission on the stories board to bring the Developer Portal in line with industry standards.
* We made small improvements in the look and feel of the Developer Portal.

#### Fixes

* We fixed a bug where the calendar icon on date/time input fields was not displayed properly.
* We fixed a bug where the star icon on your [favorite apps](/developerportal/#my-apps) was not displayed properly.

### May 22nd, 2020

#### Improvements

* The [Stories](/developerportal/collaborate/stories/) template functionality has been replaced with the **Clone** functionality in the [new UI option (Beta)](/developerportal/collaborate/stories/#story-actions).

### May 7th, 2020

#### Improvements

* We added a new story action called **Clone** to the new Beta UI. For more information, see the [New UI Option (Beta)](/developerportal/collaborate/stories/#story-actions) section of *Stories*.

### February 21st, 2020

#### Improvements

* We fixed an issue where [favorited apps](/developerportal/#my-apps) still showed up in the favorites view on the [My Apps](/developerportal/#my-apps) page after being deleted.
* We made performance improvements to the **My Apps** page.
* We fixed an issue where the description field did not expand properly when creating a new [story](/developerportal/collaborate/stories/).

### February 6th, 2020

#### Improvements

* We implemented a new design for the [Create App](/developerportal/) flow.
* When creating a new app, you can now search through templates for feature demos, academy training apps, and ready-made apps.
* After selecting an app template, you can now choose a nice icon for your app.

## 2019

### December 23rd, 2019

#### Improvements

* We made minor improvements to the process of creating a new app.

#### Fixes

* We fixed an issue where you were redirected to the **Comments** page from the **Stories** page.

### December 18th, 2019

#### Improvements

* We made some minor improvements to the style of the [Stories](/developerportal/collaborate/stories/#story-actions) Beta version. This release fixes issues regarding batch actions.

### December 13th, 2019 

#### Improvements

* We redesigned the [Stories](/developerportal/collaborate/stories/#story-actions) page with a brand new UI and improved stability. The new UI can be accessed by clicking **Enable new UI**. This is a [Beta version](/releasenotes/beta-features/).

### December 5th, 2019

#### Improvements

* We made some minor styling improvements on [Buzz](/developerportal/collaborate/buzz/).

### November 21st, 2019

#### Fixes

* We fixed an issue that prevented the **Edit in Studio Pro** functionality in the Developer Portal from opening Studio Pro.

### November 1st, 2019

#### Improvements

* We introduced the ability to [favorite](/developerportal/#my-apps) apps from the **My Apps** page and to filter on favorite apps. This is helpful when you have a large number of Mendix apps.

### September 24th, 2019

#### Improvements

* We fixed an issue that would prevent users from inviting email addresses that contain capital letters.
* We fixed an issue that occasionally triggered an error message during signup.
* We made various small performance improvements on the Developer Portal.

### September 19th, 2019

#### Launchpad Removal and App User Management Update

* We removed the old launchpad page, as we have moved to a new SSO architecture. The old URL `launchpad.mendix.com` now links to your [My Apps](/developerportal/#my-apps) page.
* We moved the App User management functionality of the launchpad to the **General** app settings in the Developer Portal. For more information, see the [Managing App Users](/developerportal/collaborate/general-settings/#managing-app-users) section of *How to Manage General App Settings*.

### August 9th, 2019

#### App User Management Improvements 

* We redesigned the UI for managing app users and improved the performance of loading manageable app environments and users.

### July 25th, 2019

#### Fixes

* We fixed an issue where updates to decimal constants in the Developer Portal were limited to 2 decimal places. This has been increased to 8 decimal places. (Ticket 85507)

### May 10th, 2019

#### Support Improvements

* We have changed the way you request a license for a new app. You can now request a license using the [Request New App Node](https://newnode.mendix.com/) app. Other requests should continue to be made through the [Support Portal](https://support.mendix.com).

### May 2nd, 2019

#### UI Improvements

* With the Beta release of Mendix Studio and Mendix Studio Pro (Mendix version 8), we have updated all mentions of *Web Modeler* to *Mendix Studio* and *Desktop Modeler* to *Mendix Studio Pro* across the Developer Portal.

### April 8th, 2019

#### Webhooks Available

* We have added the ability to create webhooks for stories and Sprints for your apps. These webhooks can be configured to send information when Sprints change and/or stories change.

### April 5th, 2019

#### Fixes

* We fixed an issue with the Developer Portal where the memory utilization was not optimized and could cause system instability. This change does not affect memory utilization by customer apps.

### March 15th, 2019

#### Fixes

* We fixed an found issue where you were not able to change your password on the **Password Has Expired** page. (Tickets 80828, 80882, 80884, 80888, 80997, 81005)
* We fixed an issue with retrieving stories in the Desktop Modeler. (Tickets 80618, 80623, 80636, 80665, 80685, 80705, 80726, 80738, 80780, 80833, 80834, 80854, 80866, 80935, 81008)
* We fixed an error that occurred when importing stories from Excel in certain situations.
* We fixed an issue where you unable to invite referrals to the Mendix Platform.

### March 14th, 2019

#### Fixes

* We fixed an issue that sometimes caused the Technical Contact information to be hidden on the app's *General* page in the Developer Portal. (Tickets 70285, 77387, 80269, 80929)

### March 7th, 2019

#### Fix

* When building a mobile application package for a new project, the default for permissions is now *disabled*. These are the set of permissions that a mobile (Phonegap) app requires and, previously, all permissions were enabled for new projects by default. This caused Push Notifications to fail if no further configuration was provided.

### March 6th, 2019

#### Feedback and Support

* We removed the [Mendix Feedback](/appstore/modules/mendix-feedback/) widget from the Developer Portal. If you want to report an issue or ask a question, please submit a ticket at [Mendix Support](https://support.mendix.com).

### January 3rd, 2019

#### Fixes

* We have updated the links to the tutorials in Mendix welcome email, so that new users of our platform can be guided better. (Ticket 77158)
* We have fixed integration issues that affected some Developer Portal users while managing application members. (Ticket 77386)

## 2018

### December 12th, 2018

#### Improvements

* We improved the performance of the **My Apps** page for users who are a member of a large number of teams.
* We updated the look and feel of the **My Company's Apps** page to be more in line with the **My Apps** page.
* We improved the look and feel of the emails that are being sent by the Developer Portal.

#### Fixes

* We fixed the broken deep link to the **Stories** page of your apps.

### December 1st, 2018

#### Fixes

* We fixed an issue that sometimes caused the team member with the Technical Contact role to be hidden on the **Node Permissions** tab of the **Security** pages. (Tickets 69085, 69150, 69419, 69440, 69458, 69585, 69592, 69783, 69884,70131,70228, 70285, 76152)

### November 14th, 2018

#### Mendix Shop

* The [Mendix Shop](https://mendixshop.mendixcloud.com) is open for business! This is a web shop where you can spend the credits you have gained by completing various [challenges](/developerportal/community-tools/mendix-profile/#challenges). The shop has cool products like Mendix t-shirts, socks, and sweatbands, so be sure to check it out.

    {{< figure src="/attachments/releasenotes/developer-portal/shop.png"   width="300"  >}}

### November 1st, 2018

#### Improvements

* We made improvements in the communication between the Web Modeler and the Developer Portal.

### October 17th, 2018

#### Fixes

* We fixed a memory leak problem that caused Developer Portal to have longer response times.
* We addressed and fixed an issue that caused some Developer Portal users to see empty dialog boxes instead of error message content. (Tickets 67626, 69363)

### October 16th, 2018

#### Fixes

* It is now possible to go to a Mendix community member's new [Mendix Profile](/developerportal/community-tools/mendix-profile/) directly from the [Buzz](/developerportal/collaborate/buzz/) and [People](https://developer.mendixcloud.com/link/people) pages. (Ticket 69702)

### October 11th, 2018

#### Improvements

* The Mendix Profile in the Developer Portal has been merged with the Community Profile. For more information, see [Mendix Profile](/developerportal/community-tools/mendix-profile/).
* Several UX updates were made to Developer Portal pages:
    * The [My Apps](https://sprintr.home.mendix.com/link/myapps) page has been redesigned, and you can now toggle your app list views.
    * The **App** > **General** page has been redesigned.
    * The [People](https://developer.mendixcloud.com/link/people) overview has been redesigned. The same view on Mendix community members is available in the [Connections tab](/developerportal/community-tools/mendix-profile/#connections) of your Mendix Profile.

### October 1st, 2018

#### Web Modeler Improvements

The Web Modeler can now be enabled for all types of apps. You can do this on the **Settings** > **General** page of your app. If you have a licensed app, you will also need to choose your [deployment](/developerportal/deploy/) environment.

#### Fixes

* For a while, the **Show activity for** filter buttons on the company **Buzz** page were broken and displayed nothing. They now work again.

### September 10th, 2018

#### Improvements

* An application created through our APIs now has the Web Modeler enabled if the template on which the app is based is suitable for use in the Web Modeler.

#### Fixes

* We have loosened an unnecessarily strict constraint on email domains during signup. You can now sign up with email domains with single-character sub-domains. (Tickets 68210 , 68386)

### June 26th, 2018

#### Improvement

* We implemented the new Mendix header.

### May 23rd, 2018

#### Improvements

* Company Admins can now export three reports to Excel: active users, app permissions of active users, and apps. This enables managing users and their permissions at scale.

#### Fixes

* The **Revisions** tab on the **Story Details** page now shows the avatar of the committer instead of the app's avatar.

### May 8th, 2018

#### Improvements

* You can now assign colors to your labels on the **Stories** page: Mendix Blue, Firetruck Red, Goldfish Orange, and Tulip Green.
* The **Story Details** page now has a new tab that shows the revisions related to the story.

#### Fixes

* On the **Feedback Details** page, the **Move to app** drop-down menu is visible again.
* Special characters like `&` are now displayed correctly in the subject of **Buzz** notification emails.
* The green call-to-action button in Buzz notification emails will now also work in Outlook for Windows. (Ticket 63452)
* If there is a lot of activity in a Buzz thread, each notification email now displays the correct thread history, instead of each email containing the same comments.
* We fixed two documentation links.

### April 9th, 2018

#### Fixes

* It is now possible to assign an empty value for application constants that have string as the data type.
* The loading pop-up window text shown while retrieving branches is now fixed.
* The bug that prevented some users from viewing the list of running requests of their applications is now fixed.
* The bug that prevented users from deactivating their projects is now fixed.

### March 16th, 2018

#### Improvements

* We changed the browser title from "Mendix App Platform" to **Mendix Platform** to be consistent with our messaging and documentation.
* Hybrid mobile improvements: you can now generate icons and splash screens, add custom loader and error images, and add custom HTML and CSS. We also added a new theming section for minor color tweaks.

#### Fixes

* The **Deploy** and **Operate** deep links were not available in the **Security** menu for user groups without monitoring access. This has been fixed.

### February 15th, 2018

#### Improvements

* We introduced a beautiful new design for the notification emails you receive when someone replies to your **Buzz** posts.

#### Fixes

* We addressed an issue that prevented the **Daily Digest** email from being sent.

### January 25th, 2018

#### Improvement

* It is now possible for you to change the Technical Contact of your applications by yourself.
