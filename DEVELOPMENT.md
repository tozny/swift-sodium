# Development

## Building

Swift sodium

## Release

To release a new version, make sure that all added files are within the pod defined source folders.

From ToznySodium.podscpec:

```
s.version = '0.10.0' // edit this to match release version
```

Verify that the pod can be compiled with:

```
pod lib lint
```

Tag the release then push to GitHub

```
git tag `0.10.0`
git push --tags
```

More details about the requirements and how to submit to Cocoapods can be found here: https://guides.cocoapods.org/making/making-a-cocoapod.html, https://guides.cocoapods.org/making/getting-setup-with-trunk

In brief, an account needs to be registered to begin a session for publishing on the local device, then running the command:

```
pod trunk push [NAME.podspec]
```

will lint the podspec then publish if the lint is successful.
