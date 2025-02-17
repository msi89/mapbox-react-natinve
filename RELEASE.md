# How to create a release for this repo

## Make sure `main` builds correctly

Are all our [actions](https://github.com/msi89/mapbox-react-native/actions) passing successfully?  
If not, make sure to investigate the issue and fix it prior to a release.

## Bump the version in our package.json

Once you verified, that `main` isn't broken, go on and increase the `version` within our `package.json`.

## Update the CHANGELOG accordingly

Our [`CHANGELOG.md`](https://github.com/msi89/mapbox-react-native/blob/main/CHANGELOG.md) should be updated whenever a PR is merged/ noteworthy changes are committed to `main`.  
Prior to a release, the changes should be documented under the `UNRELEASED` section.  
Once it's clear, that a release is about to be published, move the items under `UNRELEASED` to _this_ releases sections.  
Let your actions be guided by the previous release entries.

## Draft a new release on GitHub

Within the [releases](https://github.com/msi89/mapbox-react-native/releases) section of the repo you can [`Draft a new release`](https://github.com/msi89/mapbox-react-native/releases/new).

`Tag version` & `Release title` should be the same.  
As redundant as it might sound, please add the changes from the `CHANGELOG.md` into the body of the release.

## Monitor the repos issues for updates

Once the release is out the door (on [npm](https://www.npmjs.com/package/@rnmapbox/maps)), make sure to monitor the [issues](https://github.com/msi89/mapbox-react-native/issues) closely for problems the community might encounter
