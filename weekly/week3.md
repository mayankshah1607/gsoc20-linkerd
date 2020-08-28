### Week 3

- This week I continued working on the existing test suite and extended support for testing out
linkerd's proxy injection features.
- After discussing with mentors, tried a different approach in designing the test suite - I tried
to make the tests runnable as an individial Ginkgot test suite, rather than wrapping them all under a 
single parent test. The problem with this approach was that it introduced complexity in understanding how
the tests may be runnable. The advantage of this approach was that Sonobuoy's test reports were much 
better organized. Because this advantage could not outweigh the obstacles it sets from contributor and maintainence
perspective.
- Worked on revamping some code and moved redundant and reusable code to a separate `utils` package.
- Started some initial ground work on discussing how we'll go about writing tests for ingress.
