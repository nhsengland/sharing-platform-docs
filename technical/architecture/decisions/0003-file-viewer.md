# 0003. In-Browser File Viewer

Date: 2021-04-27

## Status

Accepted

## Context

File management is a primary function of the platform and as such an in-browser file management (upload, download, view, edit etc) experience is preferable, albeit acknowleged to be a [progressive enhancement](https://en.wikipedia.org/wiki/Progressive_enhancement) (at least in part).

The following products have been research and considered:-

1. Aspose
2. Collabora Online
3. OnlyOffice
4. Office Web Apps

## Decision

Licensing of the products for use in our platform has been a difficult challenge to overcome given our desire to produce a platform that can be used freely by any third party (within the confines of our own licensing terms and conditions).  

After much consideration it has been determined to move forward with Collabora Online for FutureNHS (due to our non-functional requirements) and leave the door open for future extensions to accommodate any other products that may become suitable in the future. 

## Consequences

### Benefits

The main reason to choose Collabora Online is because it supports the [Web Application Open Platform Interface (WOPI)](https://wopi.readthedocs.io/) file sharing protocol out of the box.  This gives us the freedom to add support for Office Web Apps in the future (should access terms change) with minimal effort, while also opening the door for others to choose to use a different file server to the one we have built for the FutureNHS project (e.g. [NextCloud](https://github.com/nextcloud)).

Retaining the freedom to extend the platform with other out of the box open source applications is considered valuable.

### Disadvantages

At the time of writing, Collabora Online requires a license for each environment in which you need to view/edit more than 10 documents at the same time.  The FutureNHS non-functional requirements greatly exceed this figure so there is an extra cost involved in standing up this solution and growing the platforma cross multiple agencies.  

Collabora have kindly engaged with us and discussions are ongoing so we're hopeful a compromise can be found that assures the developers are compensated for their time and efforts and thus the project continues to add further value into the future for our platform too.
