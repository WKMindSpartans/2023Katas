# The Analytics capability will use it's own database
## Status
APPROVED

## Context
The Road Warrior app will need to store analytics data and events generated by candidates using the app. Depending on the number of users and peak usage hours, the app could generate a large volume of analytics data.

## Decision
The Road Warrior app will use a separate database from the persistent storage capability for storing analytics data.

## Consequences
#### Positive
- Since the analytics capability may generate a large volume of database calls, by using a separate database for analytics we are better distributing the load put on our database layer. This should provide better throughput and reliability for all services.
- If the persistent storage capability fails for some reason, analytics data would still be available.
- Decoupling the analytics database schemas from the schemas used for general purposes in the persistent storage capability should allow us to anonymize, aggregate, and delete data where appropriate more easily.

#### Negative
- Additional maintenance overhead and infrastructure costs
#### Risks
- If the analytics database goes down or is corrupted, reports won't be able to be generated and historical usage data would be lost
