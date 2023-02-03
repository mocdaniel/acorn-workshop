# Acorn Workshop

This repository contains the material for attendees of my workshop '*From Dev to Prod with Acorn - Simplifying Kubernetes Deployments*', where we will take the application defined in `compose.yml` within this branch and transform it into a so-called *Acorn* to be deployed to virtually any Kubernetes cluster.

> This workshop was held for the first time on Feb 07 2023 at [CIVO Navigate](https://civo.com/navigate).

## Prerequisites

For participating in the workshop, you will need a few things on your local machine:

* `git`
* `Docker` and `docker compose`
* `acorn`, which you can install from [the project's release page](https://github.com/acorn-io/acorn/releases)
* a working Kubernetes cluster, either running locally or in the cloud; The workshop has been tested on **Docker Desktop** and **Rancher Desktop** clusters on **Windows 10**, **(Arch) Linux**, and **MacOS Ventura 13.2**

## Setup

Clone this repository, install acorn to your cluster, and check out branch `section-01` to get started!

```console
git clone https://github.com/mocdaniel/acorn-workshop.git
cd acorn-workshop
kubectl config use-context <CONTEXT>
acorn install
git checkout section-01
```

## Working with the material

This workshop is meant to be worked on while having the   [slides of my talk]() handy for reference.

> The source code of the slides is hosted in [my slides repository]().

After each section of the workshop you are supposed to check out the next branch, which will provide a clean slate to continue with.

This allows you to experiment at each stage of the workshop without having to worry that you're breaking your workshop repository.

At the moment, there are five sections to this workshop:

- `section-01` - creating a primitive `Acornfile`
- `section-02` - adding dependencies and probes
- `section-03` - adding (secret) data management
- `section-04` - adding user-provided data
- `section-05` - building, pushing, and deploying the Acorn

## License

This workshop is licensed under MIT license. For more information, please see [LICENSE](LICENSE).