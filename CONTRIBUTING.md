![1000143076](https://github.com/user-attachments/assets/6dbf02ea-0e3d-41a9-9fbb-106a39b71cf8)
![1000143075](https://github.com/user-attachments/assets/dae377ea-9641-4b0c-bf60-1a9e40c6a8a5)
![1000143077](https://github.com/user-attachments/assets/ba93c512-be4a-4079-85ea-a9fb38dd5e19)
![1000143078](https://github.com/user-attachments/assets/5cfb6447-71b5-4f77-bf70-be2b353251e4)
![1000143079](https://github.com/user-attachments/assets/1ca7c0a6-7618-4c98-aea6-6158c3b6a733)
![1000143080](https://github.com/user-attachments/assets/6b04be8a-4e7c-4baf-9338-c72651b38bbf)
![1000143081](https://github.com/user-attachments/assets/f32f521a-60e9-4166-a4aa-071e65d71aad)
![1000143083](https://github.com/user-attachments/assets/ea0d71e5-c3e3-4fbe-a151-6a4b94c6376e)
![1000143082](https://github.com/user-attachments/assets/c30bf59f-de9e-4620-ab8e-ed1a572477fe)
## Contributing

[fork]: https://github.com/github/github-mcp-server/fork
[pr]: https://github.com/github/github-mcp-server/compare
[style]: https://github.com/github/github-mcp-server/blob/main/.golangci.yml

Hi there! We're thrilled that you'd like to contribute to this project. Your help is essential for keeping it great.

Contributions to this project are [released](https://help.github.com/articles/github-terms-of-service/#6-contributions-under-repository-license) to the public under the [project's open source license](LICENSE).

Please note that this project is released with a [Contributor Code of Conduct](CODE_OF_CONDUCT.md). By participating in this project you agree to abide by its terms.

## What we're looking for

We can't guarantee that every tool, feature, or pull request will be approved or merged. Our focus is on supporting high-quality, high-impact capabilities that advance agentic workflows and deliver clear value to developers.

To increase the chances your request is accepted:
* Include real use cases or examples that demonstrate practical value
* Please create an issue outlining the scenario and potential impact, so we can triage it promptly and prioritize accordingly.
* If your request stalls, you can open a Discussion post and link to your issue or PR
* We actively revisit requests that gain strong community engagement (👍s, comments, or evidence of real-world use)

Thanks for contributing and for helping us build toolsets that are truly valuable!

## Prerequisites for running and testing code

These are one time installations required to be able to test your changes locally as part of the pull request (PR) submission process.

1. Install Go [through download](https://go.dev/doc/install) | [through Homebrew](https://formulae.brew.sh/formula/go)
2. [Install golangci-lint v2](https://golangci-lint.run/welcome/install/#local-installation)

## Submitting a pull request

1. [Fork][fork] and clone the repository
2. Make sure the tests pass on your machine: `go test -v ./...`
3. Make sure linter passes on your machine: `golangci-lint run`
4. Create a new branch: `git checkout -b my-branch-name`
5. Add your changes and tests, and make sure the Action workflows still pass
    - Run linter: `script/lint`
    - Update snapshots and run tests: `UPDATE_TOOLSNAPS=true go test ./...`
    - Update readme documentation: `script/generate-docs`
    - If renaming a tool, add a deprecation alias (see [Tool Renaming Guide](docs/tool-renaming.md))
    - For toolset and icon configuration, see [Toolsets and Icons Guide](docs/toolsets-and-icons.md)
6. Push to your fork and [submit a pull request][pr] targeting the `main` branch
7. Pat yourself on the back and wait for your pull request to be reviewed and merged.

Here are a few things you can do that will increase the likelihood of your pull request being accepted:

- Follow the [style guide][style].
- Write tests.
- Keep your change as focused as possible. If there are multiple changes you would like to make that are not dependent upon each other, consider submitting them as separate pull requests.
- Write a [good commit message](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html).

## Resources

- [How to Contribute to Open Source](https://opensource.guide/how-to-contribute/)
- [Using Pull Requests](https://help.github.com/articles/about-pull-requests/)
- [GitHub Help](https://help.github.com)
