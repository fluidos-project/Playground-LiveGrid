# FLUIDOS LiveGrid

**Tagline:** Operational Testbed of Interconnected FLUIDOS Nodes with Live Dashboard

## Overview

FLUIDOS LiveGrid is a real-world, geographically distributed testbed composed of interconnected FLUIDOS nodes and a live monitoring dashboard.

It demonstrates an energy-aware orchestration mechanism that enables:

- Local edge nodes to extend their execution capabilities by leveraging remote cloud clusters.
- A central orchestrator to optimize and coordinate service deployments across edge devices.

This environment showcases real hybrid orchestration in an end-to-end, demonstrable setup.

## Description

This software relies on a set of scripts that setup an edge-to-cloud infrastructure, which is made by:

- a variable number of edge nodes, equipped with a lightweight flavor of Kubernetes (K3s)
- a 'cloud' Kubernetes cluster (e.g., running on a public cloud or on premises)

The installed software includes Liqo, which enables the creation of 'virtual Kubernetes clusters' spanning across edge devices and cloud. This allows (a) edge users to transparently offload local applications on the cloud cluster, and (b) the cloud manager to offload (i.e., push) applications on edge node, achieving a transparent cloud continuum.

This testbed has been described in the following paper:

> Davide Miola, Stefano Galantino, Ivano Cerrato, Francesco Lucrezia, Fulvio Risso, Giacomo Verticale, "Offloading Resources to the Cloud or to the Edge? A Liqo-Powered Testbed," in proceedings of the IEEE Conference on Standards for Communications and Networking (CSCN), Bologna (Italy), September 2025.

For more information and the sull scripts to automate the setup, please refer to the following link: [https://github.com/netgroup-polito/edge-infrastructure-ansible](https://github.com/netgroup-polito/edge-infrastructure-ansible).
