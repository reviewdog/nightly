# reviewdog nightly releases
[![release](https://github.com/reviewdog/nightly/workflows/release/badge.svg)](https://github.com/reviewdog/nightly/actions?query=workflow%3Arelease)
[![release page](https://img.shields.io/github/release/reviewdog/nightly.svg?logo=github)](https://github.com/reviewdog/nightly/releases)
<!--
[![release stat](https://img.shields.io/github/downloads/reviewdog/nightly/total.svg?logo=github)](https://somsubhra.com/github-release-stats/?username=reviewdog&repository=nightly)
-->

It provides nightly [reviewdog](https://github.com/reviewdog/reviewdog) releases.
You'll get to try the latest reviwedog improvements every day.

Your feedback will support reviewdog maintainance, so I hope you'll consider
trying the reviewdog nightly and give us any feedback!
Please [file an issue](https://github.com/reviewdog/reviewdog/issues) if you come across any bugs.

## Install nightly reviewdog

```shell
# Install the latest version. (Install it into ./bin/ by default).
$ curl -sfL https://raw.githubusercontent.com/reviewdog/nightly/master/install.sh| sh -s

# Specify installation directory ($(go env GOPATH)/bin/)
$ curl -sfL https://raw.githubusercontent.com/reviewdog/nightly/master/install.sh| sh -s -- -b $(go env GOPATH)/bin

# In alpine linux (as it does not come with curl by default)
$ wget -O - -q https://raw.githubusercontent.com/reviewdog/nightly/master/install.sh| sh -s [vX.Y.Z]
```

You can check installed version and +build commit short hash with `reviewdog -version`.

```shell
$ ./bin/reviewdog --version
0.9.17-nightly20200506+f536e33
```

