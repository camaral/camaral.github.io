---
---
# Database Migration Pattern for SecDevOps

Continuous delivery is great, most software engineers agree.
Let's analise how to implement Database migration in a safe and controlled manner.

## Context
In our company, we decided to separate the database migration from the application release.
The data is very valuable for us, so we need more control over this process.
We need to recovery under 10 minutes from any new release. 
It goes without says, that the database migration scripts are always backward compatible.
As SQL scripts can become fairly complicate, a failure has to be mitigated by having 
a rollback scripts in place and tested by the time of the release.

## Testing scripts
*Migration Success*
*Migration Backward compatibility*
*Rollback*

## Tools
- Liquibase
- Flyway

## Pipeline
- AWS ECS
- Kubernetes