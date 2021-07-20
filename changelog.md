# Change Log for BaselineManagement module

## v3.1.4

- ConvertFrom-GPO: Fix configname string evaluation for space characters

## v3.1.3

- ConvertFrom-GPO: Fix bug where parameters are evaluated in "Begin" block using default value instead of pipeline input

## v3.1.2

- ConvertFrom-GPO: Fix "valuefrompipeline" not implemented for ConfigName (by alias, to support piping from backup-gpo)

## v3.1.1

- Minor fix across modules so messages are written to verbose stream rather than warning stream, unless they are warnings
- Add parameter aliases to align with BackUp-GPO cmdlet
- Fix bug in ConvertFrom-GPO where "return" included output from "mkdir" command if output path did not already exist

## v3.1.0

- ConvertFrom-GPO: Update to return object with properties organizing information about what has been output
- ConvertFrom-GPO: Add 'PassThru' parameter to to retain previous outputbehavior if desired
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