---
title: The myth of the single production environment
layout: post
---

Recently, I was expressing my opinion that automated testing code is
too often assigned a second class status, a practice that results in
this type of code becoming unmanageable over time. The person with
whom I was having this conversation, a ThoughtWorks quality analyst by
the name of Tim Camper, agreed that many developers do not treat the
test code with the same respect as production code, whereas for him
he believed that the test code was his production code.

This comment from Tim really got me thinking about "production" in
general. Often when we talk about "production" it is the environment
in which we deploy applications for our end-users. However, Tim's
comments made me realize that all of the environments that we use in
the development process (development, continuous integration, QA, UAT,
staging and production) are all production environments to at least
one set of stakeholders. Environment issues such as server or
application downtime, incorrect configuration and out of date software
each have a direct impact on the productivity of the stakeholders associated
with the affected environment.

Taking the position that all environments used in the development
process are in fact production environments suggests that there is
value in managing each environment as if they were production
environments themselves. Unfortunately, many software projects tend to
leave the responsibility of managing the "non-production" environments
to the development team. While this may give the perception that the
developers have more control over their environments, enabling the
environments to be configured in whatever way that makes the
developers the most productive, there are other implications that are
often overlooked. One such implication is the isolation of the IS team
from the development process, i.e. the team most likely to be
responsible for configuring, maintaining and monitoring the final
production environment. The result of not having IS involved in the
development process is that their expertize is underutilized.  At the
same time IS gains no insight into the deployment requirements for a
new software application until the production release request passes
their desks. Once this happens, IS becomes unable to fully support the
production application as much of the requisite knowledge remains the
property of the development organization.

It should be pointed out that involving IS in the management of
environments and acting as real stakeholders in their own right (as
they are commonly the owners of the operating requirements) may be
disruptive to existing development practices, while introducing
greater bureaucracy to environment configuration.

Embracing IS as a part of the development process is not without its
problems.  One fear is that developers loose control of what tools
they install to enhance their development activities. This fear becomes
a reality all too often as the benefits of allowing developers to tune
their development environent are not clearly communicated to the IS
deceision makers. IS then locks down develoer machines just as they
would any other desktop user. The result is that the developer's
(production) environment is no longer supporting the needs of its
target stakeholder. For this reason, the IS team (or a part of it)
needs to become part of the development team rather than being an
isolated participant in the process. Their role is then directed
toward the productivity of the delivery team by providing a stable and
adaptable environment targetted at their end user's specific needs.


