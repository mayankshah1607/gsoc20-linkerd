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

Total issues opened: 13

#### Repository: [linkerd/linkerd2-conformance](https://github.com/linkerd/linkerd2-conformance)

- [linkerd/linkerd2-conformance#2](https://github.com/linkerd/linkerd2-conformance/issues/2) - Add spec for control plane installation and its lifecycle
- [linkerd/linkerd2-conformance#3](https://github.com/linkerd/linkerd2-conformance/issues/3) - Add support to read and parse test configuration from a YAML file
- [linkerd/linkerd2-conformance#5](https://github.com/linkerd/linkerd2-conformance/issues/5) - Add tests for proxy injection
- [linkerd/linkerd2-conformance#6](https://github.com/linkerd/linkerd2-conformance/issues/6) - Add support for using add-ons for control plane installation tests
- [linkerd/linkerd2-conformance#7](https://github.com/linkerd/linkerd2-conformance/issues/7) - Add new spec for ingress tests
- [linkerd/linkerd2-conformance#8](https://github.com/linkerd/linkerd2-conformance/issues/8) - Consider using `gotestsum`
- [linkerd/linkerd2-conformance#13](https://github.com/linkerd/linkerd2-conformance/issues/13) - Release plan for linkerd2-conformance
- [linkerd/linkerd2-conformance#14](https://github.com/linkerd/linkerd2-conformance/issues/14) - Restructuring docs
- [linkerd/linkerd2-conformance#15](https://github.com/linkerd/linkerd2-conformance/issues/15) - Clean-up and refactor Gomega assertions
- [linkerd/linkerd2-conformance#24](https://github.com/linkerd/linkerd2-conformance/issues/24) - Add new spec for testing retries and timeouts

#### Repository: [linkerd/linkerd2](https://github.com/linkerd/linkerd2)

- [linkerd/linkerd2#4497](https://github.com/linkerd/linkerd2/issues/4497) - `pkg.go.dev` discovers an older version of `linkerd2` module
- [linkerd/linkerd2#4530](https://github.com/linkerd/linkerd2/issues/4530) - Add new helper method in `testutil` package
- [linkerd/linkerd2#4643](https://github.com/linkerd/linkerd2/issues/4643) - Refactor existing helpers from `inject` integration tests

## Pull Requests

Total PRs made: 17

> Note: A lot of the PRs hold really big changes (some of which took weeks to review), hence the relatively low number of PRs.

#### Repository: [linkerd/linkerd2](https://github.com/linkerd/linkerd2)

- [linkerd/linkerd2#4532](https://github.com/linkerd/linkerd2/pull/4532) - Add new helper to package `testutil`
- [linkerd/linkerd2#4591](https://github.com/linkerd/linkerd2/pull/4591) - Update function signature of `testutil.NewGenericTestHelper`
- [linkerd/linkerd2#4644](https://github.com/linkerd/linkerd2/pull/4644) - Refactor helper functions from `inject` integration tests
- [linkerd/linkerd2#4681](https://github.com/linkerd/linkerd2/pull/4681) - Refactor helper functions from `install` integration tests
- [linkerd/linkerd2#4800](https://github.com/linkerd/linkerd2/pull/4800) - Refactor helper functions from `tap` integration tests
- [linkerd/linkerd2#4752](https://github.com/linkerd/linkerd2/pull/4752) - Refactor and make `checkOutput` public

#### Repository: [linkerd/linkerd2-conformance](https://github.com/linkerd/linkerd2-conformance)
- [linkerd/linkerd2-conformance#1](https://github.com/linkerd/linkerd2-conformance/pull/1) - First pass on conformance validation
- [linkerd/linkerd2-conformance#11](https://github.com/linkerd/linkerd2-conformance/pull/11) - Add CI features for linkerd2-conformance repo
- [linkerd/linkerd2-conformance#12](https://github.com/linkerd/linkerd2-conformance/pull/12) - Add tests for ingress
- [linkerd/linkerd2-conformance#16](https://github.com/linkerd/linkerd2-conformance/pull/16) - Add tests for `linkerd tap` command
- [linkerd/linkerd2-conformance#17](https://github.com/linkerd/linkerd2-conformance/pull/17) - Add tests for `linkerd stat` command
- [linkerd/linkerd2-conformance#18](https://github.com/linkerd/linkerd2-conformance/pull/18) - Refactor all Gomega assertions and clean up logging
- [linkerd/linkerd2-conformance#19](https://github.com/linkerd/linkerd2-conformance/pull/19) - Simplify and clean up ingress tests logic
- [linkerd/linkerd2-conformance#20](https://github.com/linkerd/linkerd2-conformance/pull/20) - Add tests for `linkerd routes` command
- [linkerd/linkerd2-conformance#21](https://github.com/linkerd/linkerd2-conformance/pull/21) - Change CI linter timeout to `30m`
- [linkerd/linkerd2-conformance#22](https://github.com/linkerd/linkerd2-conformance/pull/22) - Add tests for `linkerd edges` command
- [linkerd/linkerd2-conformance#23](https://github.com/linkerd/linkerd2-conformance/pull/23) - Omit flaky output validation for `linkerd inject --manual` tests

## Weekly Updates

[WIP]