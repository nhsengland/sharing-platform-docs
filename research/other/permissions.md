# Permissions   

This page summarises and signposts the key stages of the design process to date, for permissions related to workspaces, content areas and forums within the Future NHS (FNHS) service.   

## What is this?  

Permissions are a critical feature of the FNHS service as they provide workspace managers with the opportunity to control which members can view and collaborate within their workspaces. When creating a new workspace, managers can opt for an ‘open’ status, whereby anyone can view, share and contribute to the associated content. These workspaces will be visible to all registered users and will appear within related search results. Alternatively they may opt for ‘restricted’ status, where workspaces are visible, but in order to view and interact with them, members must request permission. The third possible status is ‘private’, which can only be found and viewed by members if they are directly invited by the workspace manager.

This distinction means workspace managers are able to control access to sensitive content and can create highly focused workspaces.  Workspace managers are the predominant users of permissions.

Similar levels of access are applied to content and discussions within forums, sometimes independently of the workspace, meaning that managers can control access at different levels and maintain control of their content. For example 'restricted' content can be put into an 'open' workspace.   

There are multiple user journeys that require the set up and management of permissions in order to complete tasks in an appropriate and secure manner. These include:
  
- the set up of permissions when creating a workspace
- the sharing of content within workspaces
- discussions within workspaces
- the centralised management of permissions within a dashboard or admin area


## Current status  

**Status:** AMBER 🟠  

Permissions are a critical and enabling feature of the FNHS platform and were the subject of three rounds of user interviews during June, August and November 2021. Overall, despite some minor usability issues during setup (which has been described as clunky) and around restricting content assignment (which has been described as complex), managers considered permissions extremely valuable to help them restrict access in their desired way - and in some cases, permissions set Kahootz apart from other tools (for example Sharepoint.) 

Kahootz updated the platform in August 2022 to address some known issues with permissions, but no user research has been conducted since this time, therefore it is recommended that an expert review is conducted at the earliest opportunity. It is anticipated that the navigational support provided around the key user journeys will need to be reviewed and assessed to identify and prioritise improvements.

Several design concepts were also tested with users to inform designs for FNHS 2.0, particularly in respect to the central admin area or dashboard. These concepts should be reviewed again in terms of the learnings they contribute to the Kahootz platform.

No new designs were implemented into the product FNHS 2.0 as the designs were scaled back for MVP. 
 

## Recommendations  

### Short term (in Kahootz)  

Review the user journeys for set up and management of permissions with a primary focus on updating content to improve clarity around the processes. In parallel, review the navigation for these user journeys to improve consistency and remove confusing duplication.

Similarly review the design concepts for the central management of permissions with a focus on updating the content and navigation.  

Submit findings and change requests to Kahootz were necessary.

### Long term  

Review who else might need control over permissions. Check needs across the broader user base to assess for an extension in user roles. Identify the subset of users who don't need full workspace management, but who would benefit from being able to upload and share content with a subset of users. 

## What we did   

### Kahootz Research  

- [24 Nov 2021](/research/interviews/user-research-20211124.md) - Interviews on **permissions**
- [3 Aug 2021](/research/interviews/user-research-20210803.md) - Interviews on use of **kahootz workspace homepage** and **Managers Wireframes**
- [9 June 2021](/research/interviews/user-research-20210609.md) - Interviews on use of **permissions** and **notifications**

* Analysis of usage data   
- [11 November 2021](/research/quantitative/stats-research-20211111.md) - Analysis of how workspaces use **permissions** on **files** and **folders**. Data from 01 Jan 2020 to 30 June 2021
- [29 October 2021](/research/quantitative/stats-research-20211029.md) - Analysis of how workspaces use **permissions** with regards to **forums**. Data up to 29 October 2021
- [26 October 2021](/research/quantitative/stats-research-20211026.md) - How **Teams permissions** functions are used on the platform. Data up to 26 October 2021
* Review of related support desk tickets   

### FNHS 2.0 Research  

- Design concepts were devised and tested

### Designs  

- [Figma prototype designs](https://www.figma.com/file/4ws4CymBPVIpgdNIsTLHcb/FutureNHS_Notifications?node-id=136%3A34204)    


## Insights  

**Insight 1:**   **Set up process** for workspaces on FNHS

Users sometimes find the workspace definitions of ‘open’, ‘restricted’ and ‘private’ ambiguous. They need clarity when creating new workspaces in order to make an appropriate choice. Equivalent clarity needs to be provided when reviewing and editing this status during the lifetime of the workspace. It is important to address both these journeys in tandem in order to maintain consistency and clarity.

**Insight 2:**   Setting up and editing access to **Content**  

The process for adding permissions to content is considered laborious and overly complex, especially when managers are uploading information in bulk. Whether creating ‘Teams’ or ‘Subgroups’, the user journeys need to be reviewed and simplified in terms of naming, navigation and flow. The flow of adding content and then creating a 'Team' before allocating the team to the content is long and can create confusion. The navigation that supports this flow is problematic, with issues including the duplication of some elements, different systems of navigation (list of links vs cog icon) and confusion between the purpose of the 'View' and 'Modify' teams links. All these usability issues could benefit from a redesign that reconsiders the logical stages in the process and reviews the content to ensure clarity. 

**Insight 3:**  **Central area** to manage permissions

Managers find permission management somewhat fragmented and would benefit from a dashboard view where they can centrally manage the permissions of all their workspaces. This area needs to be easy to find and access, plus it needs to enable time and effort savings when editing multiple workspaces, teams and sub-spaces.

 **Insight 4:**  Ability to copy settings across **folders and subfolders**  

There are existing functions available to copy permissions and teams across folders and subfolders. These flows needs to be evaluated and potentially enhanced to ensure the function can be used effectively and consistently across across different user journeys.


**Insight 5:**  Expansion of roles to give permissions to **regional managers** and other non-workspace managers  

Some users requiring acess to permissions are not formal workspace managers. The status of the user group of regional managers - and probably other user groups - should be reviewed and checked for additional user needs. 


**Insight 6:**  Use of private workspaces to **preview** content   

Some users create workspaces with a 'private' status to hide them from view while they are being constructed. Then when they are complete and ready to share, workspace managers switch the status to 'restricted' or 'open.' This suggests a need to review the process for creating a workspace and options for previewing the space until it is ready to share.  

 **Evidence for insights:** Survey and interviews, wireframes and design concepts  

### User needs 

> As a workspace manager, I need the ability to create secure workspaces, so that I can collaborate with the right colleagues.
 
> As a workspace manager, I need to be able to invite everyone to read and contribute to the content I create, so that I give all my colleagues the opportunity to learn, share and connect.

> As a workspace manager, I need to remain aware of what I am sharing and with whom, so that I am in control of sensitive information.

> As a workspace manager, I need an easy way to control who can see all the content I share, so that I don’t waste time searching to make changes. 



### Areas to explore 

Review previous design concepts 

**Challenges** 

Limitations as to what can be achieved within Kahootz and speed at which changes can be applied.  
