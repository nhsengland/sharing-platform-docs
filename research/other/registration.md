# Registration   

This page summarises and signposts the key stages of the design process so far, for user registration to Future NHS (FNHS). 

## What is this?  

The registration journey from start to finish, with a focus on the landing page, the registration form and onward journeys until arrival at the homepage of FNHS.  It includes single sign on (SSO) journeys, but excludes the 'About us' page and the email inviting people to join the platform. These elements of the user journey are dealt with separately.

Effective registration is critical because:   
- the platform is secure and lives behind a log-in, therefore everyone has to register to use it  
- it is the users' first touchpoint with FNHS
- the highest proportion of support tickets are for registration, therefore there is a significant business need to improve the process

This journey distinguishes between the **'happy'** and **'unhappy'** paths, which offer significantly different user experience. 
- The happy path is defined as where someone is invited to a group and their email domain is allowed for self-registration (constitutes approx 80% of  users.)
- The unhappy path is defined as where someone is not invited, but requests to register. For example, they may have heard about FutureNHS in a webinar - they don't know the name of the group they want to join and their email domain is not recognised as an allowed email.

## Current status  

**Status:** 🟠  

There were two rounds of research conducted around the topic of registration.
The first round of research took part in May 2021. This was a set of usability tasks tested on the first Alpha prototype (pre-NHS Design system). This was part of a larger usability test of several areas including dashboard and the discoverability of new groups.

The second round of user testing in April 2022 was conducted using a new prototype, which applied the NHS design system. The design of this prototype built on learnings from previous research as well as general best practice.

The main research goals from these sessions were to test users' understanding and ability to navigate through 2 main journeys - the happy and unhappy paths. 

Also tested were variations on screen layout:

- single page (one long form with multiple questions) 
- multiple pages (different questions on separate pages) 

Both of these simplified new registration flows offered considerable user benefits over the existing Kahootz flow. 

Both designs for the new platform were equally usable, with a minor preference for the single form, where users could see at a glance what questions they needed to answer overall. 
The ultimate decision for the design to be implemented for FNHS version 2.0 was expected to depend upon technical review. 

Having reached this stage, MVP for FNHS 2.0 was unexpectedly scaled back and unfortunately neither of the designs were implemented.  

With the decision to halt work on 2.0, the focus reverted back to improving the existing Kahootz registration process. Wireframes based on this process have been defined and are currently in technical review. It is expected this process will generate a flow that resembles those already tested with users and will not require additional user testing at this stage. However this assumption has not yet been verified.


## Recommendations  

### Short term (in Kahootz)  

For the landing page: 

- Users need to understand whether or not they will be able to access the platform before they attempt to register 
- The landing page needs to present a clear visual hierarchy to lay out the options and explain concisely what FutureNHS offers without making users look any further afield
- The user journeys for registration and account creation will be reviewed and redesigned as necessary 

For the form: 

- Reduce the number of fields on the registration form – we should only ask for critical information and users should only be asked once 
- Consider the flow for users choosing to use their NHS Mail login (SSO)
- Explain the different flows for users on the happy and unhappy paths  
- Consider removing or deprioritising NHS apps  

### Long term  

- Consider the allowing users to add more information to their profiles over time in order to benefit from elements of personalisation (Linkedin style) 

## What we did   

### Kahootz Research  

- [12 May 2021](/research/interviews/user-research-20210512.md) - Interviews on user **registration**, user dashboards and how users discover new groups 

* Analysis of usage data    
* Review of related support desk tickets   

### FNHS 2.0 Research  

- [17 April 2022](/research/interviews/user-research-20220417.md) - Prototype testing for **registration** 

### Designs  

- [Figma prototype designs](https://www.figma.com/file/3wAo33GAoL8j9MN5HE7yrd/Registration---BETA?node-id=903%3A22944&t=BK7gM775Yan4aKcy-1)


## Insights  

**Insight 1:**   **Awareness** of FNHS

Users need to have both awareness of FNHS and the motivation to register. This information needs to be presented within channels they currently use or they may not complete registration.  

To support them in their decision making and encourage them to complete the registration process.


**Insight 2:**   Authority to **access**  

Users need to understand whether they will be able to access the platform or not. 

To save anyone from unnecessarily completing the process and reassure them it is worth investing their time. 


**Insight 3:**  Intuitive **flow**

Users are sometimes overwhelmed by the number of options on the login page and may not understand where to start. The page should present a simple hierarchy of options which guide the user.  

To enable intuitive login, reduce complexity and improved ease of use.
 

 **Insight 4:**  **Quick** access 

NHS users expect to be able to access the platform quickly using their NHS email. 

To save them from setting up new login details and having to remember multiple different logins. 

**Insight 5:**  Registration should be **familiar**

Users expect principles of common good practise to apply to the registration for FNHS. For example, information that users provide to FNHS needs to be seen as vital if they are to enter it in a form.  

To simplify and streamline the process of registration.  

  
 **Evidence for insights:** Survey and interviews, wireframes and design concepts  

  

**User needs**   
> As a person working in Health and Social care, I need to understand what the FutureNHS platform offers, so that I can decide whether to join.

> As a person working in Health and Social care, I need to understand whether the FutureNHS platform is available to me, so that I can decide whether to join.

> As a person working in Health and Social care, I need to access the FutureNHS platform, so that I can share, learn and connect with others within and across my sector.

> As a person working in Health and Social care, I need the FutureNHS platform to be secure and reliable, so that I can trust the source of the content I find there.
  
> As a person working in Health and Social care, I need the FutureNHS platform to be secure and reliable, so that I feel confident the content I post will be kept and accessed securely.

**Areas to explore** 

Review previous design concepts and apply findings from user research when developing new designs and flows. 

**Challenges** 

Limitations as to what can be achieved within Kahootz and the speed at which changes can be applied.  
