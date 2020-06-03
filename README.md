docs-pcf-install
==========

Installation docs for Ops Manager and VMware Tanzu Application Service for VMs.

**Note:** If you see PRs made against the `backup-restore` directory, move the corresponding Tracker story
to the PCF Docs Services tracker and notify the Services Docs PM.

## Which book repos publish this repo?

Currently only the [docs-book-pivotalcf](https://github.com/pivotal-cf/docs-partials) repo publishes this repo. 

## Which branch to use?

**Note**: Provide instructions in your PRs to indicate which branches you want Docs to apply your commits to.

| Branch name | Use for… |
|-------------| -------|
| master      | "edge" branch for Ops Manager and TAS for VMs v2.10, publishes to https://docs-pcf-staging.cfapps.io/platform/2-10/customizing/
| 2.9		  | v2.9.x |
| 2.8         | v2.8.x |
| 2.7         | v2.7.x |
| 2.6         | EOGS v2.6.x. |
| 2.5         | EOGS v2.5.x. |
| 2.4         | EOGS v2.4.x. |
| 2.3         | EOGS v2.3.x.|
| 2.2         | v2.2.x — PDFed: https://resources.docs.pivotal.io/pdfs/pcf-docs-2.2.pdf |
| 2.1         | v2.1.x — PDFed: https://resources.docs.pivotal.io/pdfs/pcf-docs-2.1.pdf |
| 2.0         | v2.0.x — PDFed: https://resources.docs.pivotal.io/pdfs/pcf-docs-2.0.pdf |
| 1.12        | v2.0.x — PDFed: https://resources.docs.pivotal.io/pdfs/pcf-docs-2.0.pdf |
| 1.11         | v2.0.x — PDFed: https://resources.docs.pivotal.io/pdfs/pcf-docs-2.0.pdf |
| 1.10         | v2.0.x — PDFed: https://resources.docs.pivotal.io/pdfs/pcf-docs-2.0.pdf |
| 1.9         | v2.0.x — PDFed: https://resources.docs.pivotal.io/pdfs/pcf-docs-2.0.pdf |

## Partials

Cross-product and repo partials are single sourced from the [docs-partials](https://github.com/pivotal-cf/docs-partials) repo.

## Style Guide

See [Word and Phrase List](https://docs.google.com/spreadsheets/d/1hkadtxR1hY57kK7h5HN4ITHLJleZixCDH_RJPUpNq_A/edit#gid=0).

## Steps for local development
```
$ git clone git@github.com:pivotal-cf/docs-layout-repo
$ git clone git@github.com:pivotal-cf/docs-pcf-install
$ cd docs-pcf-install && git checkout <branch> && cd -
$ git clone git@github.com:pivotal-cf/docs-book-pivotalcf
$ cd docs-book-pivotalcf && git checkout <branch>
$ bundle install
$ bundle exec bookbinder watch
$ open http://127.0.0.1:XXXX/platform/<version, such as `2-10`>/customizing
```

