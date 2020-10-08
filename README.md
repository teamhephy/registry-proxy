
[![Slack Status](https://slack.teamhephy.com/badge.svg)](https://slack.teamhephy.com/)

**Hephy Workflow** is the open source fork of Deis Workflow PaaS. Some of the old documentation and README are still preserved so they may reference "Deis Workflow". Hephy Workflow is the community continuation of the Deis Workflow project after it was discontinued by the Deis team which moved on to do bigger projects at Microsoft Azure.

|![](https://upload.wikimedia.org/wikipedia/commons/thumb/1/17/Warning.svg/156px-Warning.svg.png) | Hephy Workflow is the open source fork of Deis Workflow.<br />Please [read the announcement][] for more detail. |
|---:|---|
| 10/02/2020 | Hephy Workflow [v2.22.0][] release |
| 05/26/2020 | Hephy Workflow [v2.21.6][] patch release |
| 04/23/2020 | Hephy Workflow [v2.21.5][] patch release |
| 12/31/2019 | Hephy Workflow [v2.21.4][] patch release |
| 09/11/2019 | Hephy Workflow [v2.21.3][] patch release |
| 08/11/2019 | Hephy Workflow [v2.21.2][] patch release |
| 06/21/2019 | Hephy Workflow [v2.21.1][] patch release |
| 05/05/2019 | Hephy Workflow [v2.21.0][] release |
| 03/08/2019 | Hephy Workflow [v2.20.2][] patch release |
| 02/14/2019 | Hephy Workflow [v2.20.1][] patch release |
| 11/29/2018 | Hephy Workflow [v2.20.0][] new release|
| 08/27/2018 | Team Hephy [blog][] comes online |
| 08/20/2018 | Deis [#community slack][] goes dark |
| 08/10/2018 | Hephy Workflow [v2.19.4][] fourth patch release |
| 08/08/2018 | [Deis website][] goes dark, then redirects to Azure Kubernetes Service |
| 03/16/2018 | [Hephy Workflow website][] comes online |
| 03/01/2018 | End of Deis Workflow maintenance: critical patches no longer merged |
| 12/11/2017 | Team Hephy [slack community][] invites first volunteers |
| 09/07/2017 | Deis Workflow [v2.18][] final release before entering maintenance mode |
| 09/06/2017 | Team Hephy [slack community][] comes online |


# Deis Registry Proxy

Deis (pronounced DAY-iss) Workflow is an open source Platform as a Service (PaaS) that adds a developer-friendly layer to any [Kubernetes](http://kubernetes.io) cluster, making it easy to deploy and manage applications on your own servers.

For more information about the Deis Workflow, please visit the main project page at https://github.com/teamhephy/workflow.

We welcome your input! If you have feedback, please [submit an issue][issues]. If you'd like to participate in development, please read the "Development" section below and [submit a pull request][prs].

# About

registry-proxy is a proxy deployed on every Kubernetes worker node, proxying all requests to the Deis Workflow [registry][registry]. This allows the worker nodes' Docker daemons to communicate to the registry over localhost, bypassing the need for adding the `--insecure-registry` flag to the daemons.

# Development

The Deis project welcomes contributions from all developers. The high level process for development matches many other open source projects. See below for an outline.

* Fork this repository
* Make your changes
* [Submit a pull request][prs] (PR) to this repository with your changes, and unit tests whenever possible.
  * If your PR fixes any [issues][issues], make sure you write `fixes #1234` in your PR description (where #1234 is the number of the issue you're closing)
* The Deis core contributors will review your code. After each of them sign off on your code, they'll label your PR with LGTM1 and LGTM2 (respectively). Once that happens, the contributors will merge it

## Testing Your Code

When you've built your new feature or fixed a bug, make sure you've added appropriate unit tests and run `make test` to ensure your code works properly.


[issues]: https://github.com/teamhephy/registry-proxy/issues
[prs]: https://github.com/teamhephy/registry-proxy/pulls
[registry]: https://github.com/teamhephy/registry
[k8s-home]: http://kubernetes.io
[install-k8s]: http://kubernetes.io/gettingstarted/
[mkdocs]: http://www.mkdocs.org/
[issues]: https://github.com/teamhephy/workflow/issues
[Deis website]: http://deis.com/
[blog]: https://blog.teamhephy.info/blog/
[read the announcement]: https://blog.teamhephy.info/blog/posts/announcements/hephy-workflow-deis-fork.html
[#community slack]: https://slack.deis.io/
[slack community]: https://slack.teamhephy.com/
[v2.18]: https://github.com/teamhephy/workflow/releases/tag/v2.18.0
[Hephy Workflow website]: https://web.teamhephy.com
[v2.19.0]: https://github.com/teamhephy/workflow/blob/master/src/changelogs/v2.19.0.md
[v2.20.0]: https://github.com/teamhephy/workflow/blob/master/src/changelogs/v2.20.0.md
[v2.20.1]: https://github.com/teamhephy/workflow/blob/master/src/changelogs/v2.20.1.md
[v2.20.2]: https://github.com/teamhephy/workflow/blob/master/src/changelogs/v2.20.2.md
[v2.21.0]: https://github.com/teamhephy/workflow/blob/master/src/changelogs/v2.21.0.md
[v2.21.1]: https://github.com/teamhephy/workflow/blob/master/src/changelogs/v2.21.1.md
[v2.21.2]: https://github.com/teamhephy/workflow/blob/master/src/changelogs/v2.21.2.md
[v2.21.3]: https://github.com/teamhephy/workflow/blob/master/src/changelogs/v2.21.3.md
[v2.21.4]: https://github.com/teamhephy/workflow/blob/master/src/changelogs/v2.21.4.md
[v2.21.5]: https://github.com/teamhephy/workflow/blob/master/src/changelogs/v2.21.5.md
[v2.21.6]: https://github.com/teamhephy/workflow/blob/master/src/changelogs/v2.21.6.md
[v2.22.0]: https://github.com/teamhephy/workflow/blob/master/src/changelogs/v2.22.0.md
