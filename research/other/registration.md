# Registration   

This page summarises and signposts the key stages of the design process so far, for user registration to Future NHS (FNHS). 

## What is this?  

The registration journey from start to finish, with a focus on the landing page, the registration form and onward journeys until arrival at the homepage of FNHS.  It includes SSO journeys, but excludes the 'About us' page and the email inviting people to join the platform. These elements of the user journey are dealt with separately.

Effective registration is critical because:   
- the platform is secure and lives behind a log-in, therefore everyone has to register to use it  
- it is the users' first touchpoint with FNHS
- the highest proportion of support tickets are for registration, therefore there is a significant need to improve the process

This journey distinguishes between the 'happy' and 'unhappy' paths, which offer significantly different user experience. 
- The happy path is defined as where someone is invited to a group and their email domain is allowed for self-registration (constitutes approx 80% of our users.)
- The unhappy path is defined as where someone is not invited. They might have heard about FutureNHS in a webinar - they don't know the name of the group they want to join and their email domain is not recognised as an allowed email.

## Current status  

**Status:** 🟠  

There were two rounds of research conducted around the topic of registration.
The first round of research took part in May 2021. This was a set of usability tests on initial prototypes on the first Alpha prototype (pre-NHS Design system). This was part of a larger test of several areas such as a dashboard and discoverability of new groups.

The second round of testing in April 2022 consisted of user testing of a new prototype using the NHS design system. The design of this prototype built on learnings from previous research as well as general best practice.

The main research goals from these sessions to test users understanding and ability to navigate 2 main journeys - the happy and unhappy paths. 

Also tested were variations on screen layout:

- single page (one long form with multiple questions) 
- multiple pages (different questions on separate pages) 

Both of these simplified new registration offered considerable user benefits over the Kahootz process. 

Designs for the new platform were equally usable, with a minor preference for the single form, where users could see at a glance what questions they needed to answer. 
The ultimate decision for the design was expected to depend upon technical review. 

No new designs were implemented into the product as the designs for 2.0 needed to be scaled back for the MVP. 

WHAT WAS launched on UAT(?),  
List any known issues (spammy emails, OKTA interface) 
THIS WOULD BE FOR BEN TO FILL OUT
 
Retire from a software (MVC forum) and move to an NHS approved software(ad bec)  

## Recommendations  

### Short term (in Kahootz)  

For the landing page: 

- Users need to understand whether or not they will be able to access the platform before they attempt to register. 
- The landing page needs to present a clear visual hierarchy to lay out the options and explain concisely what FutureNHS offers without making users look any further. 
- Review the user journey and consider splitting registration from account creation 

For the form: 

- Reduce the number of fields in registration form – we should only ask for critical information and users should only be asked once 
- Consider making NHS Mail first option? [is this SSO?] 
- Explain what happens if you need to request access vs registering 
- Remove or deprioritise NHS apps  

### Long term  

- Allow users to add more information to profile over time (Linkedin style) 

## What we did   

### Kahootz Research  

- [12 May 2021](/research/interviews/user-research-20210512.md) - Interviews on user **registration**, **user dashboards** and how users **discover new groups** 

* Analysis of usage data    
* Review of related support desk tickets   

### FNHS 2.0 Research  

- [17 April 2022](/research/interviews/user-research-20220417.md) - Prototype testing for **registration** 

### Designs  

- [Figma prototype designs](https://www.figma.com/file/4ws4CymBPVIpgdNIsTLHcb/FutureNHS_Notifications?node-id=136%3A34204)    


## Insights  

**Insight 1:**   **Awareness** of FNHS

Users need to have both awareness of FNHS and the motivation to register. This information needs to be presented within channels they use or they may not complete registration.  

To support them in their decision making and encourage them to complete the process.


**Insight 2:**   Authority to **access**  

Users need to understand whether they will be able to access the platform or not. 

To save anyone from unnecessarily completing the process and reassure them it is worth their time. 


**Insight 3:**  Intuitive **flow**

Users are sometimes overwhelmed by the number of options on the login page and may not understand where to start. The page should present a simple hierarchy of options which guide the user.  

To enable intuitive login, reduce complexity and improve ease of use.
 

 **Insight 4:**  **Quick** access 

NHS users expect to be able to access the platform quickly using their NHS email. 

To save them from setting up new login details and having to remember multiple different logins 

**Insight 5:**  Registration should be **familiar**

Users expect principles of common good practise to apply to the registration for FNHS. For example, information that users provide to FNHS needs to be seen as vital if they are to enter it in a form.  

To simplify and streamline the process of registration.  

  
 **Evidence for insights:** Survey and interviews, wireframes and design concepts  

  

**User needs**   
> As a person working in Health and Social care, I need to understand what the FutureNHS platform offers, so that I can decide whether to join.

> As a person working in Health and Social care, I need to understand whether the FutureNHS platform is available to me, so that I can decide whether to join.

> As a person working in Health and Social care, I need to access the FutureNHS platform, so that I can share, learn and connect with others in my sector.

> As a person working in Health and Social care, I need the FutureNHS platform to be secure and reliable, so that I can trust the source of the content I find there.

**Areas to explore** 

Review previous design concepts 

**Challenges** 

Limitations as to what can be achieved within Kahootz and speed at which changes can be applied.  
