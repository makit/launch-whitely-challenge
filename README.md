# Launch Whitely Challenge

## Overview
We would like our own Feature Flag service that can be called over a REST API.

## Rules
1. Use your personal GitHub account to work on the code
2. Can use the D55 Testing Account, or your own account (should be within free tier but ensure this is the case based on what you use)
3. Must use CDK for Infrastructure as Code
4. Must be written in C# (CDK and any Application Code)
5. Needs a public API that adheres to the given API Specification
6. Needs to fulfil the given features
   * More features will be added at each phase potentially changing earlier phases, not just extending.

## Overview and Features
### Phase 1
* Have "flags" that can be on or off (boolean) and an ability to create/delete and "flip" the flag
* Will be tested with Postman API checks.
* No auth needed.
* [Swagger File](swagger.yaml)
