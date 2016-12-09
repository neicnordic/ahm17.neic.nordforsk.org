---
organizers: Frederic Haziza and Juha Törnroos
title: "Connecting two secure clouds across countries, and implementation of ELIXIR AAI system"
---

#### Part 1 - Frederic Haziza: Connecting two secure openstack clouds across countries: case Knox - ePouta

When a cluster runs at full capacity, all the newly scheduled jobs have to
wait. In case this happens often, it is necessary to scale up the
infrastructure for more computations and more data transfers. To this end, we
can of course buy more hardware, i.e., more compute nodes, more disks and more
network switches. However, this might be an expensive solution. The Tryggve
project focused therefore on an alternative approach, where we ask other
clusters if they have available resources that we could "borrow for a while".

An immediate issue with such a solution is whether a connection across borders
is even feasible, or if there is a penalizing latency. We can imagine the
scenario where computations happen in one country, while the data is located in
another country. It’s worth mentioning that this work focused on technical
aspects and did not take up legal matters related to the transfer of sensitive
data between countries. That topic is left for further work within the Tryggve
project.

In order to test the connection between countries, we built a temporary cloud
cluster in Sweden, called Knox, and connected it to the resources of ePouta, a
secure cloud cluster in Finland. The desired outcome is that the jobs would not
know whether they are scheduled in Finland or Sweden. This tutorial explains
the details of how the connection was set up and presents the various
performance tests that showed the feasibility of the solution.

The participants should have basic knowledge of OpenStack clouds.


#### Part 2 - Juha Törnroos: Taking into use federated ELIXIR AAI system

This tutorial explains the basics of the European federated authentication and
authorisation infrastructure, ELIXIR AAI. It also presents how the particular
AAI system was implemented in a genomic data access service prototype (Beacon).

The participants should be familiar with basic concepts of AAI systems.
