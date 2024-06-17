# Activate Bitrise Build Cache Add-On for Gradle

[![Step changelog](https://shields.io/github/v/release/bitrise-steplib/bitrise-step-activate-gradle-remote-cache?include_prereleases&label=changelog&color=blueviolet)](https://github.com/bitrise-steplib/bitrise-step-activate-gradle-remote-cache/releases)

Activates Bitrise Remote Build Cache add-on for subsequent Gradle builds in the workflow

<details>
<summary>Description</summary>

This steps caches the DerivedData folder and the related metadata required to speed up subsequent builds. The cache is stored in the Bitrise Build Cache infrastructure.

NOTE: you need to have an activate Bitrise Build Cache Trial or Subscription for your workspace to use this step.
</details>

## 🧩 Get started

Add this step directly to your workflow in the [Bitrise Workflow Editor](https://devcenter.bitrise.io/steps-and-workflows/steps-and-workflows-index/).

You can also run this step directly with [Bitrise CLI](https://github.com/bitrise-io/bitrise).

## ⚙️ Configuration

<details>
<summary>Inputs</summary>

| Key | Description | Flags | Default |
| --- | --- | --- | --- |
| `project_root_path` | Path to the root folder of the project to be built | required | `.` |
| `derived_data_path` | Path to the DerivedData folder used by the build. This must be the same folder specified for the -derivedDataPath flag when running xcodebuild. | required | `$HOME/Library/Developer/Xcode/DerivedData` |
| `verbose` | Enable logging additional information for troubleshooting | required | `false` |
</details>

<details>
<summary>Outputs</summary>
There are no outputs defined in this step
</details>

## 🙋 Contributing

We welcome [pull requests](https://github.com/bitrise-steplib/bitrise-step-activate-gradle-remote-cache/pulls) and [issues](https://github.com/bitrise-steplib/bitrise-step-activate-gradle-remote-cache/issues) against this repository.

For pull requests, work on your changes in a forked repository and use the Bitrise CLI to [run step tests locally](https://devcenter.bitrise.io/bitrise-cli/run-your-first-build/).

Learn more about developing steps:

- [Create your own step](https://devcenter.bitrise.io/contributors/create-your-own-step/)
- [Testing your Step](https://devcenter.bitrise.io/contributors/testing-and-versioning-your-steps/)
