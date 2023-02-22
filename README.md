# Launch Whitely Challenge

## Overview
We would like our own Feature Flag service that can be called over a REST API.

## Rules/Guide
1. Use your personal GitHub account to work on the code
2. Can use the D55 Testing Account, or your own account (should hopefully be within free tier but ensure this is the case based on what you use)
3. Must use CDK for Infrastructure as Code
4. Must be written in C# (CDK and any Application Code)
5. Needs a public API that adheres to the given API Specification - Success criteria should help here too.
6. Needs to fulfil the given features
   * More features will be added at each phase potentially changing earlier phases, not just extending.

## Features & Success Criteria
### Phase 1
* Have "flags" that can be on or off (boolean) and an ability to create/delete and "flip" the flag
* Will be tested with Postman API checks.
* No auth needed.
* [Swagger File](swagger.yaml)

### Success Criteria
1. Multiple Flags can be created
2. Flags with invalid names (see regex in Swagger) are rejected
3. Duplicate flags are rejected
4. Flags can be retrieved with the variation
5. Requests for Flags that don't exist should fail
6. Flag variations can be updated, and then immediately read with the new value
7. Flags can be deleted
8. A deleted Flag can be re-created
9. The full application should be able to be deployed to a new environment with running a CDK deployment
10. The monthly AWS cost should also be included with the completed phase based on the following load:
    * 250,000 valid reads a month
    * 100,000 reads a month for a missing key
    * 5,000 flag variation updates a month
    * 500 new flags created a month
    * 200 flag deletions a month
