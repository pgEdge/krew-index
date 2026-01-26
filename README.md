# pgEdge Krew Plugin Index

This repository serves as a custom plugin index for [Krew](https://krew.sigs.k8s.io/), the Kubernetes plugin manager. It contains a curated set of plugins and is designed to be expanded with additional plugins over time.

## Purpose
- Provide a centralized location for custom or community plugins for Krew.
- Enable easy discovery, installation, and management of Kubernetes plugins via Krew.
- Facilitate collaboration and contribution to the plugin ecosystem.

## Structure
- `plugins/`: Contains YAML manifests for each plugin.

## Using this Index

To use this custom index with Krew, add it as a new index source:

```sh
krew index add pgedge https://github.com/pgEdge/krew-index.git
```

You can then install plugins from this index using:

```sh
krew install pgedge/<plugin-name>
```

For example, to install the `cnpg` plugin:

```sh
krew install pgedge/cnpg
```