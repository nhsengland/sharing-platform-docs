# 2. Feature flags

Date: 2021-04-27

## Status

Accepted

## Context

Feature Flags are essentially on/off switches that allow you to toggle code availability within an application. This means we would have the ability to deploy code to Production without a user seeing it because it has been disabled for them by a feature flag. Code deployed behind a feature flag is essentially inactive until a user is given permission to see it and won't have any effect on their use of the platform until this decision is made.

## Decision

We intend to use Feature Flags as a tool to manage deploying to and testing in Production - switches that allow you to toggle isolated code or features in Production. This allows us to deploy code directly from the *main* branch to Production behind a feature flag that prevents users from seeing the new code until it has been thoroughly verified that it is safe to make available.

## Consequences

### Feature flagging

User roles can be assigned to Feature Flags so developers/QA can test newly-deployed code in Production whilst the wider user base are unable to see it. This will allow us to test with real data and infrastructure, giving us a high degree of confidence that enabling the feature is unlikely to introduce any bugs.
Many well known brands utilise feature flagging, such as Google, Facebook, Netflix, Amazon, etc.

### Benefits

There are many benefits to using Feature Flags beyond allowing testing in Production.

#### Beta testing

With a beta feature flag it will be incredibly easy to make new features available to a select group of beta testers on the platform, without exposing them to the wider user base. There will be no need for a separate beta platform or logins for the beta users.

#### Code rollback

It is extremely quick to rollback a feature flagged release - simply toggle it off. It is inevitable that some bugs will make it into Production and should a serious bug go live, having feature flags in place will allow a rapid response. The breaking code can be temporarily toggled off while a fix is deployed, minimising any downtime for Production as a whole.
Without feature flags it would be necessary to redeploy Production with the offending code rolled-back, which can be a time consuming process.

#### A/B testing

Having feature flagging in place also provides the ability to perform A/B testing. This allows for splitting the user base and testing different prototypes of a feature. The results can be compared and provide insight for the future development of said feature. Assumptions made in the design process can be validated and modified accordingly with real-time feedback from users actually interacting with the feature. If it is not being engaged with you can make an informed decision on whether to cease working on it and prioritise other features for development.

#### Canary deployments

Similar to A/B testing, a canary deployment is where you expose a new feature to a small number of users, say 5%, to get some initial feedback on the feature’s stability, uptake and efficacy. Combined with effective monitoring and analytics, this is a powerful tool for verifying prototypes and feature design, ensuring that by the time the feature goes fully live it has been tested thoroughly.

A canary deployment can be performed either with a feature flag or by creating a second Production environment and diverting users to the new environment. If an issue should arise in the new deployment, it is easy to stop the diversion and continue sending users to the original environment.

#### Workspace segmentation & user engagement

Feature flags can be assigned to specific Groups/Workspaces. This opens up the possibility of identifying workspaces where there is high user engagement or where new features/widgets are taken up quickly by users and targeting them for testing.