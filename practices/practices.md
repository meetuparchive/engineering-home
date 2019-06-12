## Meetup Engineering Practices
#### *Our goal: Empower Meetup engineers to build coherent, lasting engineering solutions that bring value to our customers.*

### How do we use these?
These practices are intended to help you understand what is expected of engineers at Meetup. They should answer the question: *"How should we be building software at Meetup?"*

### *As Meetup engineers, we:*

### [Build for Change](/principles/principles.md) 

1. ***Build iteratively***, using [evolutionary architecture](https://www.thoughtworks.com/insights/blog/microservices-evolutionary-architecture), because it encourages incremental change in [vertical slices](https://agileforall.com/vertical-slices-and-scale/) to help us learn about our software and deliver value to our customers as quickly as possible. We prefer to [defer decisions](https://martinfowler.com/bliki/Yagni.html) as long as is responsible, so that we learn as much about the problem as possible before committing to a solution.
2. [Generate](https://docs.google.com/document/d/1Wuuc7B1AexwT2UV3N-8BpNxxNB0z_hFhHM0tC2Dx-K8/edit?ts=5cfff9bf#), seek out, and ***use data from many different sources*** to be able to frequently [take risks](https://youtu.be/rA3K0nwBIH4?t=1200) and make increasingly better product and engineering [decisions](https://blog.usejournal.com/the-surprising-link-between-a-companys-growth-and-its-data-analytics-strategy-8e5be31bbca5).
3. ***Do [Continuous Integration](https://martinfowler.com/bliki/ContinuousDelivery.html), Delivery, and Deployment*** in every repository because continuously committing and automatically deploying small change sets to master is safer and gets working software in front of customers early and often. 
4. ***Test [in Production](https://martinfowler.com/articles/qa-in-production.html)*** and use [canary releases](https://martinfowler.com/bliki/CanaryRelease.html) to roll out changes to production in an operationally efficient, data-driven, and safe way that uses feature flags and fast rollbacks. 

### [Build for Understanding](/principles/principles.md)

5. ***Believe that higher quality software is made together***, through collaboration within and outside our teams, including [code](https://medium.com/making-meetup/effective-code-review-through-principled-pragmatism-c9ef59228bdb) and [architecture](https://meetup.atlassian.net/wiki/spaces/MUP/pages/679642233/About+the+Architecture+Toolkit) reviews, and [pair](https://meetup.atlassian.net/wiki/spaces/coresvc/pages/523075747/How+To+Pair+Better), and [mob](https://meetup.atlassian.net/wiki/spaces/coresvc/pages/829947918/Mobbing) programming. When we show up for each other, we hold each other to higher standards, unblock and learn from each other, and really [get shit done](http://www.sarahmei.com/blog/2010/04/14/thoughts-on-two-months-of-pairing/).
6. ***Write [small things](https://www.youtube.com/watch?v=8bZh5LMaSmE)*** that are easy to understand, maintain, and change, because our business is quickly changing. When the structure of our code makes changing its behavior difficult, or hard to understand, we [refactor](https://martinfowler.com/books/refactoring.html) by [changing the structure first and then changing the behavior](https://www.youtube.com/watch?v=8bZh5LMaSmE).
7. ***Ship all code with the right set of tests*** through [the pyramid](https://martinfowler.com/articles/practical-test-pyramid.html) to make our software more understandable and safe to change. We optimize for fast feedback loops (most achieved via unit tests) and a great customer experience (most achieved via end-to-end tests).
8. ***Build [infrastructure as code](https://www.hashicorp.com/resources/what-is-infrastructure-as-code)*** so we can bring the benefits of automation, versioning, and continuous delivery to operating our [cloud infrastructure](https://aws.amazon.com/).

### [Build Meetup](/principles/principles.md)

9. ***Measure our [customers' success](https://landing.google.com/sre/sre-book/chapters/monitoring-distributed-systems/)***, not just our system health. We monitor both symptoms and causes. Our alerts and pages reflect an actual impact on customers, are actionable, and minimize false positives.
10. Believe in ***growing engineers into [T-shaped engineers](https://medium.com/making-meetup/t-shaped-engineering-on-meetup-pro-1e0a38df7f5b)*** because it is good for individual career growth, breaks down silos, and empowers teams to deliver faster and be more productive. 
11. ***Measure [UX speed](https://meetup.atlassian.net/wiki/spaces/WEG/pages/818316451/UX+Speed+Definitions)*** so we understand how our customers are [viewing our product](https://meetup.atlassian.net/wiki/spaces/WEG/pages/818316451/UX+Speed+Definitions) and ***[build performant software](https://meetup.atlassian.net/wiki/spaces/WEG/pages/669614663/Web%2BPerformance%2BUX%2BSpeed)*** based on that data.
12. ***[Own and operate our own systems](https://www.thoughtworks.com/insights/blog/there-no-such-thing-devops-team)*** because a higher quality product results when engineers are in direct contact with their customers through [operating their software](https://queue.acm.org/detail.cfm?id=1142065). We’re oncall for the code we write and own. We practice postmortems to identify and fix issues with our software and people systems.
