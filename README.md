# Knowledge

This repo contains the contents and source code for [FGACYC's Knowledge Base](https://knowledge.fgacyc.com). We used 
[Quartz](https://github.com/jackyzha0/quartz) and markdown (managed by [Obsidian](https://obsidian.md/) and [Obsidian Git](https://github.com/denolehov/obsidian-git)) to build this knowledge base.

## How to run locally

All the available commands can be found in the [Makefile](/Makefile). However you need to install the following to make 
it work locally.

- [go](https://go.dev/doc/install)
- [hugo-obsidian](https://github.com/jackyzha0/hugo-obsidian)
- [hugo](https://github.com/gohugoio/hugo)

Then you can run the following command to start the server locally.

```sh
make serve
```

or if you prefer to serve locally through docker

```sh
make docker
```

## How to publish

We use GitHub Actions for CI/CD, the deployment workflow definition can be found at [deploy.yaml](/.github/workflows/deploy.yaml). In short, 
to deploy a change, just commit and push to the `main` branch and GitHub Actions will take care of deploying it to GitHub Pages.