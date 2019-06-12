## Meetup Engineering Principles
#### Empower Meetup engineers to build coherent, lasting engineering solutions that bring value to our customers.*

### How do we use these?
These principles are intended to help you evaluate engineering solutions to problems. Therefore, before you can apply them to your project, you have to be able to answer the question *"What problem am I trying to solve?"*   
Once you know that, ask yourself questions like:

- Have I evaluated each of these principles in choosing this solution?
- What aspects of these principles am I actively prioritizing? Why?
- Why are the other aspects of these principles not a priority in this context?

### Build for Change
Meetup's engineering team and platform will scale. The demands of our users will change, and our understanding of the needs of our users will evolve. The systems we build will need to either adapt to change or be replaced. 

Systems built for change:

- … are easily replaced or extended
- … gracefully handle changes in the systems they interact with ([robustness principle](https://wikipedia.org/wiki/Robustness_principle))
- … scale without an increase to operational overhead (people or processes)
- … are observable, so that we're aware of when they're not meeting our needs and the needs of our users, and need to be changed

What *doesn't* this principle mean?

- It doesn't mean it's fine to make abrupt changes without consideration of consumer effects
- It doesn't mean *don't think ahead*, but neither should you build the most general, flexible, scalable system that will solve the problem; part of building for change means accepting that you don't know on what axis change will be required.

### Build for Understanding
Building a compelling product means integrating with other systems, and doing so effectively means understanding those systems. Do you understand the systems that you're integrating with? Will engineers who need to integrate with or maintain your new system in the future (including you!) be able to understand how it works, and what the limits of this system are? 
Seek to compose systems out of small, easy-to-understand components. Make their presence, intent, and how they fit together, discoverable. 

This likely means a combination of:

- Reusing common toolsets and patterns
- Well-structured code
- Builds, deployments, resource provisioning (e.g. databases, server instances, etc.) specified as artifacts in the code repository (infrastructure-as-code)
- Tests
- Documentation
- Code comments
- Instrumentation

What *doesn't* this principle mean?

- This doesn't mean *"Make it as small as possible."* Instead, adequately separate the concerns.
- This doesn't mean every code module of every component of every system needs exhaustive documentation before it can be released (or after)
- This doesn't mean you need to ensure 100% test coverage

### Build Meetup
The decisions we make in designing our systems should reflect the problem being solved. Some teams solve problems for our users, while others solve problems for other engineers, but all of us should be focused on solving problems pertinent to making Meetup.

What *doesn't* this principle mean?

- This doesn't mean *challenge the validity of the problem being solved*.
- This doesn't mean *we only solve Meetup-specific problems*. We tackle problems where the lack of a solution, or a solution more suited to our needs, is significantly slowing us down.
