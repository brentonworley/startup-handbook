---
layout: default
title: Engineering Principles
nav_order: 4
---
# Engineering Principles

The Adepto Engineering team have agreed the following set of Principles to guide us in the continual jourey of building a great product and a quality code base.

## Architecture Principles

- **Engineer Sufficiently.** - Understand the problem you are trying to solve, and tackle this, this includes the scale and volume of users expected.It is important that the solution works and is performant for this expected user base, but not useful to design something for 10 million users if we have 10,000. Don't be scared of having to comeback and refactor something, our **Test Coverage** principle should minimise the risk and impact of this.
- **Avoid Premature Optimisation.** Raise a ticket or Tech Debt entry to cover those edge cases.
- **Strict Interface Control** - Access to data and/or logic from a microservice must only be allowed through a defined and documented API, or through the consumption of agreed events.
- **Address Architecture Early.** Discuss any proposed architecture changes early and with an appropriately wide audience. This can be done through team slack channels, and if necessary Chapter meetings. Do **not** leave architecture discussions to the PR Process.
- **Squad/Team Independence.** Independence allows teams to scale and move faster. Consistency across the platform is important from a UX perspective, but from a code perspective it is not as important as independence.
- **Owners and Maintainers.** Independence of teams and services is facilitated by the Owners and Maintainers
- **Leverage the Open Source model.** To share components and consistent ways of solving problems across the platform leverage the open source model to reduce dependencies on individuals and different teams.
- **A Million Flies.** Look to the community for a solution before building our own, and don't be afraid to reassess our custom solutions as the community and industry move forward.
- **Consistency is important but not at the expense of improvement.** Work toward eventual consistency in the platform to avoid delays and dependencies. If one team finds a better way of doing something, DO IT. Don't wait until that change can be rolled out across the whole platform, prove the value, and then drive consistency after this.


## Business and Customer Principles

- **Focus on Customer Value.** Every feature we deliver and every change we make to the code base should be viewed from a lens of the value that it delivers to our Customers and Users. We are a funded startup/scaleup and it is critical that our limited resources are being used in the most efficient way.
- **Solve the problem at hand.** Don't be distracted from the problem you're solving by trying to re-factor or re-architect large pieces of the code base. However, this principle is subject to the Boy Scout Rule caveat. If there is something small that you can do to improve the code base, then do it, otherwise make sure that they limitation is documented in one of our Tech Debt registers.
- **Do not compromise on Quality.** In delivery of any software solution there are three levers that can be moved independently, Time (=cost), Scope and Quality. We will only ever move Time and Scope, Quality is sacrosanct as cutting corners in quality will always result in significant cost in the medium to long term. If timeframes are fixed, then we must look to manage scope and expectations. Our whole Product Development process should be founded on the delivery of quality software.
- **POCs and spikes** are the one exception where quality and clean code principles may be compromised. In these situations it is important to start again, or completely rework the code.
- **Customer Value User Stories.** Features should be designed, implemented and delivered as end-to-end slices of functionality. User Stories were created to focus attention on the user outcome, use these to define your features and work in teams to deliver each story as an independent, working piece of software. This is why we work in cross-functional teams.

## Communication Principles

- **Keep Discussions in the open.** Where ever possible have discussions in open or team slack channels, rather than private chats. Record meetings and publish were appropriate.

## Coding Principles

> Writing clean code is what you must do in order to call yourself a professional. There is no reasonable excuse for doing anything less than your best.
>
> *Robert C. Martin*

- **Clean Code.** We aspire to software craftsmanship, everyone should read and be familiar with Clean Code by Robert C. Martin. The ratio of time spent reading vs writing code is more than 10:1, making it easier to read code actually makes it easier (and quicker) to write. Writing clean code is faster than not writing clean code!
- **KISS** "All code is technical debt" is often mentioned regarding solutions that are far larger than they need to be. Consider if single use values declared in a separate namespace is premature optimisation. Consider the readability of code that is written by reducing nested blocks. Consider building many smaller functions over one larger function to avoid "god functions" occurring.
- **Simplicity equals flexibility.** Direct quote from GitLab handbook:
> Please remember that the only way to make code flexible is to make it as simple as possible.
>
> https://twitter.com/BaseCase
- **Boy Scout Rule.** *Leave the campground cleaner than you found it.* It’s not enough to write the code well. The code has to be kept clean over time.
- **The Code should tell the story**. Comments do not make up for Bad Code. Rather than spend your time writing comments to explain code, spend the time cleaning the code so that it is self explanatory.
- **Respect the Linter.** Do push code that has Linter errors. The Linter will eventually be added to the pre-commit hook, but in the meantime take the responsibility to check this yourself.
- **Keep an eye on the browser console.** Keep an eye on the browser console to ensure you're not introducing new errors.

## Quality and Testing Principles
- **Follow the Testing Pyramid**

![Automation Test Pyramid](../assets/testPyramid.png)
- **Test every possible case.** Make sure that every possible case and outcome is being tested. High code coverage reduces the cost of ownership over the long term.
- **Implementation Agnostic Tests.** Your code should be able to be tested without understanding or touching the inner workings of a class or component.
- **Everyones responsibility.** Quality and testing is not just the responsibility of the QA team. Everything you merge to master should be production ready.
- **Keep the Error Logs clean.** It is vital for our application to keep our logs healthy. There shall be no new unintended or unchecked errors introduced in any logs we rely on.

## <a name="pr-principles">Pull Request Principles</a>

- **Aim for Continuous / Iterative improvement.** There is no such thing as *perfect* code - there is *only better code*. Reviewers should not require the author to polish every tiny piece of a PR before granting approval. Rather, the reviewer should balance out the need to make forward progress compared to the importance of the changes they are suggesting. Instead of seeking perfection, what a reviewer should seek is continuous improvement. (from https://google.github.io/eng-practices/review/reviewer/standard.html)
- **Everyones Day Job.** The Peer Review process is critical part of mainatianing the quality of the code base. Every Engineer must consider this a part of their *normal* or *day* job. Don't leave this work to the few.
- **Reference the JIRA ticket in your commit.** Every PR should relate to a JIRA ticket, either User Story or Bug, and the link should be added to the commit, e.g. XXXX: message or XXXX - message.
- **Avoid subjectivity and don't sweat the small stuff.** Need to minimise subjectivity in PR’s. One way to identify subjectivity is does the work you’re about to comment on really affect readability/performance/coding standards that greatly? If not, make it clear it’s an optional comment. Don't feel you need to complete each comment. It's fine to respond and say the work will be done in another ticket (and ensure the actual ticket exists) as at times some comments will hold up a PR that might be required for deployed unnecessarily. If in doubt, ask another team member as it will take some time to get used to.
- **PR Approvals.** All PR's only require 1 approval before the code is merged to Master. It's quite ok to require more approvers if it gives you that peace of mind, or there is a breaking change which you believe needs team attention.
- **Prefix your PR titles (if appropriate)** Add one of the following prefixes to your PR title. This makes it easier for the team to understand the priority of a PR as well as help the reviewer view the PR in the right context. Some titles may be used together if appropriate eg *[RC/Bugfix] -  This is some PR title*

| Prefix | Reason |
| ---      |  ---------|
| **WIP**   | Already used and widely accepted from all knowing that the code is ongoing work. |
| **Expedite**   | PR is top priority work and are the tickets that appear in the expedite row. |
| **NSR** (next scheduled release)  | PR is part of the current tagged release. |
| **Bugfix**   | PR is a bugfix. |
| **Feature**   | PR is a brand new feature. |
| [No Prefix]   | PR is part of the normal backlog. |



## References

- https://about.gitlab.com/handbook/engineering/
- https://google.github.io/eng-practices/review/reviewer/standard.html
- https://martinfowler.com/articles/practical-test-pyramid.html
- https://blog.cleancoder.com/
- https://martinfowler.com/articles/microservices.html
