# Oracle Linux and Virtualization Training

The OLTrain project provides a place to explore Oracle Linux and Virtualization products using videos and walkthrough tutorials and hands-on labs.

## Getting Started

1. Clone this repository. Use the `--recurse-submodules` to clone the blowfish theme from the original authors GitHub project.

   If you have already cloned the project without using `--recurse-submodules`, then run `git submodule init` followed by `git submodule update` to pull in the theme.

1. Review content locally by running `hugo server` and then view in the provided url in the browser.

<!-- 1. Generate the static site content by running `hugo -t blowfish` where blowfish is the theme to apply to the statically generated content. -->

1. Remove files from destination not found in static directories with `hugo --cleanDestinationDir`.

1. Create a PR.

1. Merging the PR triggers the GitHub action to rebuild the site.


## Deploy Site to GitHub

This site deploys using GitHub Actions configured in `Settings` > `Pages`.

## Support or Contact

- Project Owner: Craig McBride ([@craigmcb](https://github.com/craigmcb))
- Project Admin: Martin Littlecott ([@mlittlec](https://github.com/mlittlec))
- Project Admin: Bill Graef ([@bgraef](https://github.com/bgraef))


## Contributing

This project is not accepting external contributions at this time. For bugs or enhancement requests, please file a GitHub issue unless it’s security related. When filing a bug remember that the better written the bug is, the more likely it is to be fixed. If you think you’ve found a security vulnerability, do not raise a GitHub issue and follow the instructions in our [security policy](./SECURITY.md).

## Security

Please consult the [security guide](./SECURITY.md) for our responsible security vulnerability disclosure process

## License

Copyright &copy; 2022,2023 Oracle and/or its associates.

All content in this repository is distributed under the [Universal Permissive
License 1.0](https://oss.oracle.com/licenses/upl/).

[Blowfish](https://github.com/nunocoracao/blowfish) is distributed under the
[MIT License](https://github.com/nunocoracao/blowfish/blob/main/LICENSE).

[Vagrant by HashiCorp](https://www.vagrantup.com/) is distributed under the
[MIT License](https://github.com/hashicorp/vagrant/blob/master/LICENSE).

[Ruby](https://www.ruby-lang.org/en/) is distributed under the terms of the
[2-clause BSD License](https://opensource.org/licenses/BSD-2-Clause) or the
conditions listed in the [Ruby `license.txt` file](https://www.ruby-lang.org/en/about/license.txt).
