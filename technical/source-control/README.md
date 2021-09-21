# Source Control

https://github.com/nhsengland/sharing-platform-docs

We currently employ a small number of open-source respositories that cover the various tracts of work being undertaken to deliver our programme.   They can all be found on GitHub and are of course open to contributions from the wider community.

## nhsengland/sharing-platform-docs

This is the repository you are currently viewing.   It is primarily a learning resource for those developing the platform, but we also track our own continual evolution as we learn more about our users, our product and discover better ways of working.  

## nhsengland/futurenhs

https://github.com/nhsengland/futurenhs

This is the repository that currently houses code artefacts for the first part of our platform.  Our initial approach has been to build on-top of existing open-source products where possible and to adopt a monolithic scale-up architecture for the software to keep things as simple as possible and minimise the 'time to market'.   We hope the product will prove successful, and should this be the case, will look to rearchitect the initial solution such that is can scale-out and be more resilient as we start to increase the size of the user base and the features offered.

We have yet to conclude whether we will be adopting a single mono-repository or multiple as we continue forwards and start to break up the monolith.

## nhsengland/futurenhs-infra

https://github.com/nhsengland/futurenhs-infra

This repository contains all the infrastructure as code artefacts; primarily environment specific Terraform scripts.

## nhsengland/futurenhs-file-server

https://github.com/nhsengland/futurenhs-file-server

This repository contains all the code artefacts for the custom file server implementation.  The file server implements open protocols such as WOPI, that are the mechanism through which we can communicate with some 3rd party platform extensions such as Collabora.  As you might imagine, this service is primarily tasked with 'file' specific operations, including collaborative editing and in borwser viewing.

At the time of writing, this service is a Proof-of-Concept extension point that relies on our Application Gateway configuration to handle request routing between the core site, blob storage and this service.   It is anticipated that this service will harden as we move towards a production quality release.