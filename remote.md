---
layout: default
title: Remote Practices
nav_order: 3
---
# Introduction

- Why remote?
- What are the benefits?
- Why would we go down this path?
- But doesn't Agile require co-located teams? How to address this paradox.

## Remote First

Successful implementation of remote working within an organisation or team is not as simple as just allowing people to work remotely, it is important to make some fairly fundamental changes to how you work and especially collaborate to ensure that remote workers are not disadvantaged or hindered from contributing to the team environment and completing their work. To facilitate this we have adopted a **Remote First** approach with a number of practices and principles to elevate remote working and workers to the same level as those in the office.

This is not about discouraging face to face, and in-person collaboration, as whenever possible this is absolutely  most effective. The intent adopt practices that address the challenges of major timezone difference across the business and teams and to level-up remote communication and collaboration to feel as cohesive as sitting in the same room.

Many of the ideas and approaches here have been tried and tested from other globally remote organisations, some of which even do not have any central offices, i.e. remote only. Some reference material can be found here:

- [**Remote Only**](https://remoteonly.org/) - a useful resource of ideas, principles and examples of remote working
- [**GitLab Remote Manifesto**](https://about.gitlab.com/blog/2015/04/08/the-remote-manifesto/) - GitLab's manifesto for remote working.

### Communicate Asynchronously
It's certainly okay to have a face to face conversation with a colleague or team member either by video conferencing (VC) or even in-person if you're lucky enough to be together in the same place at the same time, and we don't want to discourage this and the bonding that it helps to foster. However, the reality is that this becomes the exeption rather than the norm as the teams grow and the level of remote working increases.

The only scalable solution for communication amongst remote/distributed teams is to communicate asynchronously where ever possible.

What does this mean at Adepto?

The primary mechanism for asynchronous communication as Adepto is slack, and there are some basic guidelines that it is important to understand:

- Asynchronous communication is **asynchronous!** Remember the person or people that you are comminicating with may be otherwise busy, or sound asleep. Sometimes you are able to chat back and forth in essentially real time, but don't expect that someone must or will respond to your slack message immediately.
- There’s a general expectation to **respond within 24 hours**, but beyond that each person can decide when to check and respond to their messages.
- If you require a prompt response to your message, be really specific about the urgency. If it is really urgent then follow the escalation process.
- Keep conversations in public or shared channels. In most cases, there is more than one person who will be able to help you or is interested in the conversation.
- If you have a request use the @person functionality to bring it to the attention of that person. Provide clear guidelines as to the urgency and timeframes, i.e. "I'm working to a deadline can I please have this by 5pm tomorrow (GMT)", or "Can we have this complete by the end of the week?" Don't forget to specify timezones.


### Collaborate Asynchronously
Collaboration is an extension of communication, and many of the same principles apply to facilitate effective and efficient remote/asynchronous collaboration.

Many of us will argue that one of the most effective collaboration mechanisms is sitting around a good old fashioned whiteboard. This is still great when you have the opportunity, but it is not a viable option if any of the meeting participants are remote, as the ability to follow and participate in the conversation is very constrained. In this situation the synchronous collaboration should be achieved using a digital platform. (At this point we have not settled on a standard set of tools for this, but have been experimenting with various things).

As in communication, the ability to collaborate in such a synchronous manner quickly breaks down with significant timezone differences. Therefore we recommend the following approaches:
- The **Pull Request (PR)** process is a critical channel for collaboration within the engineering team. This forces a level of socialisation and approval of each persons work. This is a critical part of the overall engineering process and an opportunity for each engineer to observe and contribute to other engineers work. There is a separate section of the handbook dedicated to the PR process, and it is important to understand the roll of the PR process and collaboration it facilitates. Try to keep the PR collaboration focused on the change at hand, if you find the discussion diverting to a broader problem, then best to extract the collaboration into a more public slack channel.
- An **open slack channel** such as #eng, or #eng-backend-chat provides an ideal platform for a broader while fairly short discussion and team collaboration.
- However, if the conversation is going beyound a dozen or so messages, and is starting to spawn multiple threads then it is probably time to move it to the next level.
- **Temporary slack channels** - the most effective combination for remote and asynchronous collaboration is a dedicated (temporary) slack channel along with an accompaning collaboration document such as a confluence page, Google Doc or Google sheet. Create the temporary slack channel, invite the people that should be involved in the conversation, and set up the conversation by setting the context, and desired outcomes of the collaboration. The "owner" of the conversation is responsible for creating the slack channel and facilitating the ongoing conversation. They should create the corresponding collaboration document, and summarise the outcomes as they happen, to assist in getting a positive set of actions rather than just an ongoing meandering conversation. Be sure to set ground rules, goals of the exercise, and timeframes for the collaboration session.
- **Face to Face** - sometimes an asynchronous collaboration may conclude with a face-to-face session to wrap it up. This can be for a few different reasons, but the most common are, 1) Two or more parties can not come to an agreement via the asynchronous channel, and a face-to-face conversation is required to resolve, or 2) For an in depth collaboration, it can be worth getting the parties together to review and agree the solution and action plan.
- If you receive a response but it doesn't sound right, assume you've misunderstood what the person has said and ask for clarification.

### Slack Channels for Collaboration and Communication
There are a number of "formal" slack channels that align to each of the main group functions within Adepto and are the ideal starting point for a conversation relating to that area. By default you may or may not be a member of some of these channels depending on your role, but they are all open for you to join so if you want to join a particular conversation just reach out to someone from that group and they will be able to invite you.

Last but not least is the **saythanks** channel. Use this to recognise work of your team mates, and thank them when they have helped out. We have a bit of fun with this, using the hey-taco plugin to slack to dispense virtual tacos as a show of gratitude. Just mention the person you want to thank using @person and give them a **:taco:**

### Side benefits (effects) of Remote First
There are some not insignificant benefits or side effects that result from the asynchronous communication and collaboration approach that is necessitated by a remote and distributed workforce.

- **Writing things down**. The default behaviour is to right down conversations, and self document the collaboration and discussions.
- **Public Sharing of information**. It is much easier to share information that is written down, compared with relying on verbal communication. This is particular important during growth phases of a company as a large number of new starters are brought onboard. Information and knowledge is also less likely to end up in "need to know" silos once documented and shared publicly across the company or team.
- **The liberation of documentation**, this Handbook is case in point. Visible and documented collaboration is open and transparent, coupled with a robust change control process such as a pull request process allows documents to be changed by anyone, and hence further foster full team collaboration. A product code base is just another example of this documentation and collaboration, the principles, guidelines and processes that help us to work as teams and do our jobs should be treated no differently.

### Daily Standups
Daily standup meetings have always been about collaboration and removing blockers, not a status update for management. If your team uses synchronous standup meetings, make sure you use them as an opportunity to bond with your team, and identify and formulate plans to remove any blockers so that you can get on with your work. They are also a great way to understand what other team members are working on and determining if you have any dependencies.

Standups can also be run asynchronously, and different teams are trialing different tools to run their standups asynchronously over slack.

### Face to Face when you can
It's still important to get face to face meetings where ever possible, if you are able to do this in-person then great, otherwise utilise zoom or slack for a VC chat. This might be a regular structured one-on-one, or just an adhoc chat to resolve something.

### Bond in Real Life
We spend a big proportion of our time at work, and working with our colleagues and team mates. Whenever you get the opportunity it is great to spend real face-to-face time, not to work, but just to get to know you work colleagues.

Trust is crucial to good team work and collaboration, and is generally earn't through repeated actions and or familiarity. The quickest way to build trust is to get to know your team, and the best way to do this is through shared experiences and getting to know your team mates beyond the work that you're doing.

### Set and Manage your boundaries
One of the potential risks of remote working and in fact just working within a company where you have to deal with major timezone differences is the ability to switch off.

Asynchronous communication will continue to flow well after normal working hours for pretty much everybody, so it is important that everyone manages this in a way that allows them to effectively perform their job, but also to be able to find a balance between work and life. For some of us, this is one of the key benefits of the remote environment, where we can work when it suits, and balance that with other commitments, such as family.

However, it doesn't come without dangers and hence here are some suggestions of ways to set and manage your boundaries, the most important thing is to decide what boundaries work for you and set them:

- Decide what hours you want to be alerted to communications and turn things off outside these hours. For example use the Snooze setting on slack to turn off notifications between certain hours and over the weekend.
- If you have regular outside or family commitments then put something in your calendar so that people know that you are not available.
- It is particularly helpful to indicate unavailability during acceptable business hours and during the overlap time periods between the UK and Australia as this makes it much easier for the meeting organiser to book a meeting at late notice with confidence.
- If you are blocking out time in your calendar to complete some tasks then please be explicit in the calendar event about your availability for meetings during this time.
- Calendar systems have been designed with functionality to accept, decline or suggest a different time. If you have a clash use these features to let the organiser know.

### Respect Peoples Boundaries and Time
When communicating and setting meeting invites, especially across timezones, please consider the following.

- Don't expect that someone will read or respond to your email or slack message out of hours or over the weekend. They may do, but this should not be considered as an expectation.
- Given our timezone challenges, 7am to 7pm are considered reasonable hours. If you are trying to communicate with someone or book a meeting time outside these hours then by default please respect that the person may **NOT** be available.
- As a general rule, try to prioritise the UK/AUS overlap time for cross region meetings and calls, i.e. 7-10am (GMT) and 4-7pm (AEST). For the UK team this means, where possible avoid booking UK only meetings first thing in the morning, and for the Australian team minimise bookings in late afternoon/early evening that are Australia specific.
- When booking meetings you should **ALWAYS** check the persons availability, and respect this.
- If someone has a meeting, appointment, family commitment booked in their calendar then **DO NOT** book over this. If this is the only time available then contact the person first to check if there is a possibility that they can move or reschedule. Don't assume that your meeting is more important.
- Respecting peoples time in this way can make it difficult to book last minute meetings, so try and avoid that situation. Is it really so urgent that it can't wait for 1 day? We are asking a lot of people to make pretty considerable sacrifices with their personal time, for this to be sustainable we must respect that time.
- If you do not check, or choose to book over top of a prior commitment in someones calendar. They may well decline your invitation, so best to check in advance. In a lot of cases if you ask the person in advance they will do their best to reorganise, but if you disrespect the boundaries they have set then they are much more likely just to decline.

### Escalation of communication
It is important that non real-time communication is **NOT** in real time, which means an immediate response is not required and people can and should turn off notifications on these primary asynchronous channels, both to put aside blocks of time to focus on a task at hand, and also to maintain personal balance.

However, our primary focus as a company is to build and support the Adepto platform. For a number of reasons, including a major outage, it is sometimes critical that the team, particularly the Engineering and DevOps team, can be contacted when required and act swiftly. For this reason it is important that an alternative communication mechanism is in place as an escalation channel and also in the case of emergencies.

**SMS** and **Mobile phone** are the escalation mechanism in this situation.

This document will provide details of who to contact in an emergency, and contact details.

Please remember that these are personal mobile phone numbers of our staff, treat them with due privacy and do not abuse this escalation channel.
