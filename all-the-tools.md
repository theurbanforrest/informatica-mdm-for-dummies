# all-the-tools
There are a handful of tools you get with Informatica MDM Multidomain on-prem.  They do not have a single easy portal to run them all from.  Here is the cheatsheet for the full set

## Hub Console
A .jar file you run locally.  This is where you set up your initial schemas (BO_ tables) & its supporting elements:

- Lookups for columns that are limited to a set of values (BT_ tables)
- Relationships to other entities (BR_ tables)
> Side note: when creating custom schemas, the XO_ XT_ XR_ convention is good to use

- Match rules to flag potential duplicate records
- Merge settings to either merge automatically vs. kick out to a queue (Task Manager) for an analyst to review


You can also run a handful of jobs manually:

- Run match rules against all the newly loaded data (CONSOLIDATION_IND == 4)
- Load data from Landing tables into your schemas
- Perform manual reviews of matches like you would in C360

## Provisioning Tool
With your initial schemas set up, you now need to wire them up so they can appear in the C360 UI

## Customer 360 (C360)
Formerly known as Data Director, this is where your end users will be interacting with MDM

## ActiveVOS
Acquired by Informatica to power its Task Manager feature, the workflows & jobs configured here are what enable C360 users to use the Task Manager to work through queues of work

## Swagger UI
There is also a built-in API on the OpenAPI 2.0 Swagger specification
