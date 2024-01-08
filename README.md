![Banner depicting screen from 1981 "Clash of the Titans" movie where the Kraken has been released](./banner.webp)
# gh-kraken

A `gh` extension to identify unreleased changes compared to latest release.

```shell
$ gh kraken cli/cli          

cli/cli trunk branch is ahead of v2.36.0 by 7 commits

COMPARE: https://github.com/cli/cli/compare/v2.36.0...trunk

SHA       DATE                  AUTHOR            MESSAGE
49ec4842  2023-10-03T14:45:44Z  williammartin     Add homebrew-bump-debug workflow (#8114)
aefecbab  2023-10-03T14:54:44Z  andyfeller        Update homebrew-bump.yml...
80e46cab  2023-10-03T15:28:58Z  andyfeller        Update deployment.yml...
3443a752  2023-10-03T17:20:02Z  darthwalsh        docs: fix typo in pr create (#8115)...
7a68d19c  2023-10-10T12:29:40Z  andyfeller        Merge pull request #8116 from cli/andyfeller/7718-homebrew-bump...
885ccd74  2023-10-11T08:35:40Z  utouto97          Disable issue with template (#7918)...
363dacbb  2023-10-11T13:41:00Z  kbailey4444       Set default repository for `repo clone` and `repo fork` (#7768)
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
  -H, --hostname=<host>                Hostname of the GitHub instance to authenticate with
  -m, --message-width=<int>            Width of commit message; default '80'
  -r, --release-tag=<string>           Release tags to calculate from; default latest
  -s, --sha-width=<int>                Width of commit SHA; default '8'
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
