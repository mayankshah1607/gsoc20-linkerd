# Google Summer of Code '20 with Linkerd

Hi, there! This repository has all the details of the work I did as a part of Google Summer of Code '20 with [Linkerd](https://github.com/linkerd)

## General Information

- Name: Mayank M Shah
- Github: [@mayankshah1607](https://github.com/mayankshah1607)
- Email: hello@mayankshah.dev
- Mentors: [@Pothulapati](https://github.com/Pothulapati), [@ihcsim](https://github.com/ihcsim)
- Project Title: Conformance Validation
- Project Repository: [linkerd/linkerd2-conformance](https://github.com/linkerd/linkerd2-conformance)
- Design Proposal: [View Proposal](https://github.com/linkerd/rfc/blob/c75ee3f76692c5eb22457d3d91a29d0a8b1cbea3/design/0003-conformance-validation.md)

## Project Abstract

Linkerd has an extensive check suite that validates a cluster is ready to install Linkerd and that the installation was successful. These checks are, unfortunately, static checks. Because of the wide number of ways a Kubernetes cluster can be configured, users want a way to validate their specific install for conformance over time. The proposed project tackles this problem by allowing users to deploy sample workloads to their cluster and carry out extensive E2E tests for conformance.

This project proposes a new test suite that shall be used for conformance validation. The new test suite shall be used to validate non-trivial network communication (HTTP, gRPC, websocket) among stateless and stateful workloads in the Linkerd data plane. This shall be done by carrying out extensive e2e tests of Linkerd features using a sample distributed application (data plane).

## Issues

## Pull Requests

## Weekly Updates

