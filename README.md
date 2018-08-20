
# OpenShift Service Mesh

Click here to read the [OpenShift Service Mesh MVP documentation](https://github.com/openshift-istio/istio-docs/blob/master/content/install-mvp.adoc) that was previously displayed at this location.  The linked document also includes information about associated sample applications (boosters) and tutorial scenarios(missions) released with the MVP.

This repository contains documentation for the MVP (developer preview) release of OpenShift Service Mesh, based on the upstream Istio project.  This README provides information about this documentation repository.

## Getting Started

The OpenShift Service mesh documentation is written in [Asciidoc](http://asciidoctor.org/docs/asciidoc-syntax-quick-reference/).  


### To Build the Docs

The downstream docs use `ccutil` to generate the docs as part of the Docs-to-Drupal toolchain.

To build all of the books, open a terminal, navigate to the root directory of this repository, and type the following command (you may need to run it as `sudo`):
```
$ scripts/buildGuides.sh   
```
The script provides links to both asciidoctor and ccutil builds for each of the example books.

You can also build a single guide. Navigate to the folder of the manual you want to build and type the following command (you may need to run it as `sudo`):
```
$ ./buildGuide.sh
```

To view the generated output, nagivate to the following directory for a particular manual:`<title>/build/tmp/en-US/html-single/index.html`


## Submitting a Pull Request

You can close a GitHub issue from a Pull Request.  All you have to do is include the [special keyword syntax] (https://help.github.com/articles/closing-issues-using-keywords/) (for example, “fixes #5) in the body of your Pull Request.  When the pull request is merged into your repository's default branch, the corresponding issue is automatically closed.

Commit messages against Jira should start with the project name associated with the PR. If the PR is to address MAISTRA-123 then the commit message for the PR must start with "MAISTRA-123 " and then followed by the detailed commit message (no semi-column or dash between the Jira ID and text, no brackets... just a space).

