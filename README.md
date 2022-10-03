# EnigmatiKreations.Framework

[![Develop Build](https://github.com/Juansero29/EnigmatiKreations.Framework/actions/workflows/build.yml/badge.svg?branch=develop)](https://github.com/Juansero29/EnigmatiKreations.Framework/actions/workflows/build.yml)
[![Build, Pack & Push NuGets](https://github.com/Juansero29/EnigmatiKreations.Framework/actions/workflows/build-pack-and-push.yml/badge.svg?branch=main)](https://github.com/Juansero29/EnigmatiKreations.Framework/actions/workflows/build-pack-and-push.yml)

A base-framework for all my apps across the .NET environment

## References

Created with the help of:

- https://www.wearecogworks.com/blog/nuget-with-github-packages-tutorial/ 
- https://docs.microsoft.com/en-us/nuget/create-packages/supporting-multiple-target-frameworks
- https://nicksnettravels.builttoroam.com/multitargeting/

## How To Update Nuget Source Password (PAT) When Expired

### On github
- Go to https://github.com/settings/tokens and check your PATs
- If needed, create a new one and delete the old ones
- Update secrets as needed in https://github.com/Juansero29/EnigmatiKreations.Framework/settings/secrets/actions
- Verify that the workflows use the correct secret name in the different commands https://github.com/Juansero29/EnigmatiKreations.Framework/tree/main/.github/workflows

### On local machine using the custom nuget feed
- Run command `nuget sources`
- Verify which source name you should update
- Run command `nuget sources update -Name "SOURCE_NAME" -username "NEW_USERNAME" -password "NEW_PAT"`

## Porting To MAUI
https://devblogs.microsoft.com/xamarin/tips-for-porting-your-xamarin-library-to-dotnet-maui/
