[![VRTK logo][VRTK-Image]](#)

> ### VRTK Prefabs `v4-beta`
> A collection of productive prefabs for rapidly building spatial computing solutions in the Unity software.

[![Release][Version-Release]][Releases]
[![License][License-Badge]][License]
[![Backlog][Backlog-Badge]][Backlog]
[![Documentation][Academy-Badge]][Academy]

[![Slack][Slack-Badge]][Slack]
[![Videos][Videos-Badge]][Videos]
[![Twitter][Twitter-Badge]][Twitter]

## Beta Disclaimer

The VRTK Prefabs have not yet been released fully are still in a beta phase meaning there may still be undiscovered bugs, missing features and a lack of usable documentation. All of these things are being worked on but progress is slow as there is only one person actively working on these VRTK Prefabs in their spare time so please be patient and respectful. You are free to use the VRTK Prefabs in any way you wish, but if you feel you will struggle figuring stuff out for yourself without detailed documentation then it may be better off if you wait until the full release of the VRTK Prefabs.

The prefabs contained in this repository will eventually be separated out into their own repositories and packages.

## Introduction

The VRTK Prefabs aim to make building spatial computing solutions in the [Unity] software fast and easy for beginners as well as experienced developers.

> **Requires** the Unity software version `2018.3.10f1` (or above).

## Getting Started

### Setting up the project

* Create a new project in the Unity software version `2018.3.10f1` (or above) using `3D Template` or open an existing project.
* Ensure `Virtual Reality Supported` is checked:
  * In the Unity software select `Main Menu -> Edit -> Project Settings` to open the `Project Settings` window.
  * Select `Player` from the left hand menu in the `Project Settings` window.
  * In the `Player` settings panel expand `XR Settings`.
  * In `XR Settings` ensure the `Virtual Reality Supported` option is checked.
* Ensure the project `Scripting Runtime Version` is set to `.NET 4.x Equivalent`:
  * In the Unity software select `Main Menu -> Edit -> Project Settings` to open the `Project Settings` inspector.
  * Select `Player` from the left hand menu in the `Project Settings` window.
  * In the `Player` settings panel expand `Other Settings`.
  * Ensure the `Scripting Runtime Version` is set to `.NET 4.x Equivalent`.

> Note: Unity `2019.1` (or above) requires additional project setup before importing the VRTK Prefabs.

* Download and install the `XR Legacy Input Helpers` from the Unity Package Manager.
  * In the Unity software select `Main Menu -> Window -> Package Manager` to open the `Package Manager` window.
  * Select `XR Legacy Input Helpers` from the `Packages` tab in the `Package Manager` window.
  * Click the `Install` button located in the bottom right of the `Package Manager` window.
  * The `XR Legacy Input Helpers` package will now download and install into the project.

### Adding the package to the Unity project manifest

* Navigate to the `Packages` directory of your project.
* Adjust the [project manifest file][Project-Manifest] `manifest.json` in a text editor.
  * Ensure `https://registry.npmjs.org/` is part of `scopedRegistries`.
    * Ensure `io.extendreality` is part of `scopes`.
  * Add `io.extendreality.vrtk.prefabs` to `dependencies`, stating the latest version.

  A minimal example ends up looking like this. Please note that the version `X.Y.Z` stated here is to be replaced with [the latest released version][Latest-Release] which is currently [![Release][Version-Release]][Releases].
  ```json
  {
    "scopedRegistries": [
      {
        "name": "npmjs",
        "url": "https://registry.npmjs.org/",
        "scopes": [
          "io.extendreality"
        ]
      }
    ],
    "dependencies": {
      "io.extendreality.vrtk.prefabs": "X.Y.Z",
      ...
    }
  }
  ```
* Switch back to the Unity software and wait for it to finish importing the added package.

### Updating to the latest version

The package will show up in the Unity Package Manager UI once the above steps have been carried out. From then on the package can be updated by selecting the package in the Unity Package Manager and clicking on the `Update` button or using the version selection UI.

## Documentation

Visit the [Academy] for a collection of educational content to help you get the most out of building spatial computing solutions with the VRTK Prefabs.

## Contributing

Please refer to the Extend Reality [Contributing guidelines] and the [Unity project coding conventions].

## Code of Conduct

Please refer to the Extend Reality [Code of Conduct].

## License

Code released under the [MIT License][License].

## Disclaimer

These materials are not sponsored by or affiliated with Unity Technologies or its affiliates. "Unity" is a trademark or registered trademark of Unity Technologies or its affiliates in the U.S. and elsewhere.

[VRTK-Image]: https://user-images.githubusercontent.com/1029673/40060519-bb122e8c-584e-11e8-8402-ca168b327671.png

[Version-Release]: https://img.shields.io/github/release/ExtendRealityLtd/VRTK.Prefabs.svg
[Backlog-Badge]: https://img.shields.io/badge/project-backlog-78bdf2.svg
[License-Badge]: https://img.shields.io/github/license/ExtendRealityLtd/VRTK.Prefabs.svg
[Academy-Badge]: https://img.shields.io/badge/learn-academy-f3aeae.svg

[Slack-Badge]: https://img.shields.io/badge/slack--E24663.svg?style=social&logo=slack
[Videos-Badge]: https://img.shields.io/badge/youtube--e52d27.svg?style=social&logo=youtube
[Twitter-Badge]: https://img.shields.io/badge/twitter--219eeb.svg?style=social&logo=twitter

[Releases]: ../../releases
[License]: LICENSE.md
[Backlog]: http://tracker.vrtk.io
[Academy]: https://academy.vrtk.io

[Slack]: http://invite.vrtk.io
[Videos]: http://videos.vrtk.io
[Twitter]: https://twitter.com/VR_Toolkit

[Unity]: https://unity3d.com/
[Latest-Release]: ../../releases/latest
[Project-Manifest]: https://docs.unity3d.com/Manual/upm-manifestPrj.html

[Contributing guidelines]: https://github.com/ExtendRealityLtd/.github/blob/master/CONTRIBUTING.md
[Unity project coding conventions]: https://github.com/ExtendRealityLtd/.github/blob/master/CONVENTIONS/UNITY3D.md
[Code of Conduct]: https://github.com/ExtendRealityLtd/.github/blob/master/CODE_OF_CONDUCT.md