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

