![Banner depicting screen from 1981 "Clash of the Titans" movie where the Kraken has been released](./banner.webp)
# gh-kraken

A `gh` extension to identify unreleased changes compared to latest release.

```shell
$ gh kraken cli/cli          

cli/cli trunk branch is ahead of v2.36.0 by 7 commits

COMPARE: https://github.com/cli/cli/compare/v2.36.0...trunk

SHA                                       DATE                  AUTHOR         MESSAGE
49ec4842116f67fc672c01d393953cf0af22f279  2023-10-03T14:45:44Z  williammartin  Add homebrew-bump-debug workflow (#8114)
aefecbab6515b1b864e381b6a0210cf4f90a0d0a  2023-10-03T14:54:44Z  andyfeller     Update homebrew-bump.yml...
80e46cabebb378ae9bd70cf341517ba09b195bb1  2023-10-03T15:28:58Z  andyfeller     Update deployment.yml...
3443a752a9949ee4f954a84f7ab94a4b99df1b27  2023-10-03T17:20:02Z  darthwalsh     docs: fix typo in pr create (#8115)...
7a68d19c40eae8e0cb590ea91309948c9beabb97  2023-10-10T12:29:40Z  andyfeller     Merge pull request #8116 from cli/andyfe
885ccd7424acb8db9519dc972bbac2b67c5a9d3f  2023-10-11T08:35:40Z  utouto97       Disable issue with template (#7918)...
363dacbbed8cc9f86026ec1b1e38c6dca0d78c08  2023-10-11T13:41:00Z  kbailey4444    Set default repository for `repo clone`
```

## Quickstart

1. `gh extension install andyfeller/gh-kraken`
1. `gh kraken <owner>/<repo>`
1. Profit! :moneybag: :money_with_wings: :money_mouth_face: :money_with_wings: :moneybag:

## Usage

```shell
Identify unreleased changes compared to latest release.

USAGE
  gh kraken [flags]
  gh kraken [flags] <repo>
  gh kraken [flags] <owner>/<repo>

FLAGS
  -d, --debug                          Enable debug logging
  -h, --help                           Displays help usage
  -H, --hostname <host>                Hostname of the GitHub instance to authenticate with
```

## Setup

Like any other `gh` CLI extension, `gh-kraken` is trivial to install or upgrade and works on most operating systems:

- **Installation**

  ```shell
  gh extension install andyfeller/gh-kraken
  ```

  _For more information: [`gh extension install`](https://cli.github.com/manual/gh_extension_install)_

- **Upgrade**

  ```shell
  gh extension upgrade gh-kraken
  ```

  _For more information: [`gh extension upgrade`](https://cli.github.com/manual/gh_extension_upgrade)_
