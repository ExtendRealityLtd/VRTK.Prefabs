# Changelog

### [1.0.2](https://github.com/ExtendRealityLtd/VRTK.Prefabs/compare/v1.0.1...v1.0.2) (2019-10-15)

#### Bug Fixes

* **README.md:** provide correct link for package releases ([1027f04](https://github.com/ExtendRealityLtd/VRTK.Prefabs/commit/1027f04f222dd278f9daa5478e7f2ce235e01a57))
  > The package release link was incorrect and pointing to VRTK. This has now been updated and references specific to VRTK have been removed.
  > 
  > The README.md now reads as if it is specific to the VRTK prefabs.

### [1.0.1](https://github.com/ExtendRealityLtd/VRTK.Prefabs/compare/v1.0.0...v1.0.1) (2019-10-15)

#### Bug Fixes

* **CHANGELOG.md:** add meta file for Unity to consume ([c9b51f0](https://github.com/ExtendRealityLtd/VRTK.Prefabs/commit/c9b51f03e7fe60c54e5247ddb7623ff7cb4845cd))
  > Unity would complain if the package was included in another project due to packages being read only and therefore not being able to generate the .meta file for the CHANGELOG.md file.
  > 
  > This fix simply adds a meta file in manually.

## 1.0.0 (2019-10-15)

#### Features

* **ci:** add configuration for ci+cd pipeline ([1a546ea](https://github.com/ExtendRealityLtd/VRTK.Prefabs/commit/1a546ea401c17fad7e87aea2fe7f11c65ff61743))
  > The .devops directory contains the configuration for the azure ci+cd pipeline build process.
* **README.md:** add content to readme ([a3f25f3](https://github.com/ExtendRealityLtd/VRTK.Prefabs/commit/a3f25f312d9b855d6f631bb4c8d24a40b9386ded))
  > The README.md file is now populated with useful content about the repo and how to use it in other projects.
* **structure:** add prefab collection ([cf8198b](https://github.com/ExtendRealityLtd/VRTK.Prefabs/commit/cf8198bb5ee6b88f53463fa304dd212b0ddf6ba5))
  > The prefabs from the VRTK repo have been copied over and Zinnia has been added as a dependency to the package.json file.

#### Documentation

* **support:** add supporting .github files ([24bc9c5](https://github.com/ExtendRealityLtd/VRTK.Prefabs/commit/24bc9c5f7dc590c52b461f1b92d80b23912b875f))
  > The .github files provide a way for GitHub to display useful information when performing certain tasks such as raising issues or pull requests.
  > 
  > This commit also renames the LICENSE file to add the `.md` extension and modifies the default .gitignore to be inline with other projects.
