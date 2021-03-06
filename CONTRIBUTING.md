# How to Contribute

We love Pull Requests! Your contributions help make ChooseALicense.com great.

## Getting Started

So you want to contribute to ChooseALicense. Great! We welcome any help we can
get. But first, please make sure you understand what
[this site is all about](http://choosealicense.com/about). It’s not a comprehensive list of all possible licenses.

## Adding a license

Choosealicense.com is intended to demystify license choices, not present all of them. As such, there are several requirements for a license to be listed on the site:

1. The license must have [an SPDX identifier](https://spdx.org/licenses/). If your license isn't registered with SPDX, please [request that it be added](https://spdx.org/spdx-license-list/request-new-license-or-exception).
2. The license must be listed on one of the following approved lists of licenses:
  * [List of OSI approved licenses](https://opensource.org/licenses/alphabetical)
  * [GNU's list of free licenses](https://www.gnu.org/licenses/license-list.en.html) (*note: the license must be listed in one of the three "free" categories*)
  * [Open Definition's list of conformant licenses](http://opendefinition.org/licenses/) (non-code)
3. A [GitHub code search](https://github.com/search?q=MIT+filename%3ALICENSE&type=Code) must reveal at least *1,000* public repositories using the license

If your proposed license meets the above criteria, here's a few other things to keep in mind as you propose the license's addition:

* Licenses live in the `/_licenses` folder.
* The license files should be in the format of `_licenses/[lowercased-spdx-id].txt` (e.g., `_licenses/mit.txt`)
* Each license has both [required and optional metadata](https://github.com/github/choosealicense.com#license-metadata) that should be included.
* The text of the license should be wrapped to a 78 character width.
* The body of the file should be the text of the license in plain text.
* Almost without exception, new licenses should be added as hidden (`hidden: true` in the YAML front matter), such that they are directly linkable and detectable, but not otherwise listed.

## Making Changes

The easiest way to make a change is to simply edit a file from your browser.
When you click the edit button, it will fork the repository under your account.
Note what issue/issues your patch fixes in the commit message.

For example, to [change this file](/CONTRIBUTING.md),
find it in the GitHub repository. Then click the `Edit` button. Make your
changes, type in a commit message, and click the `Propose File Change` button.
That’s it!

For more advanced changes, check out [the bootstrap instructions](https://github.com/github/choosealicense.com#run-it-on-your-machine) in the [project's readme](/README.md).

## Testing

[HTML::Proofer](https://github.com/gjtorikian/html-proofer) is set up to validate all links within the project.  You can run this locally to ensure that your changes are valid:

```shell
./script/bootstrap
./script/cibuild
```
