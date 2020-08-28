### Week 1

- Worked on the initial structure of the repository - discussed with Tarun (mentor) how we'll go about modularizing the repository,
and how the tests must be structured.
- Explored the various features of Ginkgo and Gomega, along with a few existing projects that currently use it.
- Tried out various designs for the project - initial approach was to wrap all tests as separate `Ginkgo.Describe` blocks, 
inside a main parent `Ginkgo.Describe` block
- Wrote tests for control plane lifecycle - this includes linekrd install, uninstall and upgrade commands.
