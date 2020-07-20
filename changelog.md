# Change Log for BaselineManagement module

## v3.0.0

- refactored to remove support for formats other than Group Policy
  - removed parsers
  - removed tests
- Add support for Group Policy Client Side Extension
  - switched from Registry resource in PSDscResources module to RegistryPolicyFile resource in GPRegistryPolicyDsc module
  - added RefreshRegistryPolicy to end of configuration block (in all cases)
- remove external modules available in gallery
- minor changes to comments where appropriate (typo's, etc)
- started change log