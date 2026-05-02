# Nukemichi

Nukemichi is a private network management ecosystem focused on making self-managed connectivity simpler, more structured, and more maintainable.

The core idea is straightforward: instead of treating private networking as a pile of terminal commands, scattered configs, and manual server work, Nukemichi turns it into a product with a clear workflow, modular components, and room for both regular users and engineers.

The ecosystem is built around the sing-box unified proxy platform and combines client-side operation, server-side orchestration, and deployment tooling into one direction.

## What I am building

I am building a system where a person can:

- deploy their own private network stack
- manage it from an Android app
- inspect and operate the remote server through a dedicated backend agent
- work with both simplified and advanced flows depending on their level of expertise

The goal is to reduce friction for people who want a private, self-controlled network setup, while still keeping the system extensible for developers and operators.

## Ecosystem components

### `nukemichi-android`
The Android application and the main user-facing product.

It combines two roles in one app:

- a client for connecting to and monitoring a configured profile
- a wizard for guided deployment and management of a remote server setup

This repository is also where the public modular APIs and the main application architecture are exposed.

Repository:
- [nukemichi-android](https://github.com/Nukemichi/android)

### `agent-michi`
A dedicated backend orchestration agent written in Go.

It is responsible for structured remote operations such as:

- host inspection
- deployment
- service lifecycle management
- server-side operational tasks needed by the Android app

It exists so the ecosystem does not have to depend on fragile terminal parsing or ad-hoc server automation.

Repository:
- [agent-michi](https://github.com/Nukemichi/agent)

## Direction

Nukemichi is being developed as an ecosystem, not just a single app.

Current and planned directions include:

- split user flows for regular users and engineers
- guided infrastructure deployment
- integrated educational and FAQ content
- modular deployment strategies for different operational needs
- stronger privacy, safety, and environment hardening
- tighter integration between the Android app and backend orchestration services

## Philosophy

Nukemichi is built around a few principles:

- private networking should be manageable without chaos
- advanced tooling should not require a broken UX
- self-hosted infrastructure should be accessible without hiding how it works
- public APIs and modular architecture matter if the ecosystem is going to grow

## Status

> Intense development is in progress.

The ecosystem is under active construction, and both architecture and functionality are evolving quickly.
