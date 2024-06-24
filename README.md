# Save xcodebuild Bitrise Build Cache

[![Step changelog](https://shields.io/github.com/bitrise-steplib/bitrise-step-save-xcodebuild-cache?include_prereleases&label=changelog&color=blueviolet)](https://github.com/bitrise-steplib/bitrise-step-save-xcodebuild-cache/releases)

Saves the DerivedData folder and the related metadata into Bitrise Build Cache to speed up subsequent builds.

<details>
<summary>Description</summary>

This steps caches the DerivedData folder and the related metadata required to speed up subsequent builds. The cache is stored in the Bitrise Build Cache infrastructure.

If not specified otherwise, the complete system DerivedData folder (`$HOME/Library/Developer/Xcode/DerivedData`) is cached. As xcodebuild only reuses DerivedData if the input files'
modification time is the same, the step also collects and saves the modification time of the input files (project files including source code files) into a metadata file.

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
| `project_root_path` | Path to the root folder of the project to be built |  |  |
| `cache_key` | The key used to store the cache archive | required | `.` |
| `verbose` | Enable logging additional information for troubleshooting | required | `false` |
</details>

<details>
<summary>Outputs</summary>
There are no outputs defined in this step
</details>

## 🙋 Contributing

We welcome [pull requests](https://github.com/bitrise-steplib/bitrise-step-save-xcodebuild-cache/pulls) and [issues](https://github.com/bitrise-steplib/bitrise-step-save-xcodebuild-cache/issues) against this repository.

For pull requests, work on your changes in a forked repository and use the Bitrise CLI to [run step tests locally](https://devcenter.bitrise.io/bitrise-cli/run-your-first-build/).

Learn more about developing steps:

- [Create your own step](https://devcenter.bitrise.io/contributors/create-your-own-step/)
- [Testing your Step](https://devcenter.bitrise.io/contributors/testing-and-versioning-your-steps/)
