# Governance

## Incremental feature changes

We distinguish between a deployment and a release.

- A **deployment** brings a code change into an environment. This code change should not be visible to end users.
- A **release** make a change visible to one or more end users.

### Deployment

Every change is:

- Peer reviewed by at least one other developer
- Tested using automated unit, integration and exploratory tests before it is deployed to production
- Tested using automated browser tests and exploratory tests in production before it is exposed to users

This approach requires that each change is hidden behind a Feature Flag. See our [testing approach](../testing/README.md) for more details. Because these changes are not visible to end users, deployments can be made multiple times a day. This enables quick bug fixes in case an issue has not been found earlier by the different layers of testing.

### Release

Every feature is:

- Hidden behind a Feature Flag
- Enabled by the Product Owner after being tested and discussed with the service team
- Sometimes gradually rolled out to subsets of users for *live* observation and impact assessment

## Significant Platform Changes

Bigger changes to the platform will go through an approval process and involve the oversight of an Architecture Review Board. This ensures we're not duplicating effort for something that already exists elsewhere in the organisation. 