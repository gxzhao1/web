---
title: "Spatial Analysis: Indego Bikeshare Prediction"
excerpt: 
header:
  teaser: /assets/images/portfolio-indego-bikeshare.jpg
layout: single
---
{% capture fig_img %}
![Foo]({{ "/assets/images/portfolio-indego-bikeshare.jpg" | relative_url }})
{% endcapture %}

<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>Bikeshare demand error map illustration</figcaption>
</figure>

Urban bike sharing is a service system that provides bicycles on the public street for individuals to use on a short term basis, usually through purchasing a membership plan. Many bike sharing systems, including Philadelphia’s Indego bike share, allow users to unlock a bike from a dock and return it at another dock. This form of transportation is often seen as a mean to promote health and sustainability while reducing automobile congestion.

Despite the benefits, this kind of system is hard to operate well, as there are limited number of docks at a dock station. A user cannot return a bike when the station is full and cannot get a bike when the station is empty. To prevent users from suffering from such problems and stop using the service, operators need to manually distribute the optimal number of bikes at the stations to ensure that a bike or a dock is available when needed. One way of doing this is to dispatch bikes when problems occur, but this will be very inefficient. By the time the operators arrive with an available bike or make room in the station, the user may be impatiently waiting for a long time or has decided not to use the service again. The operators ought to take a more proactive approach. This is known as the “re-balancing” problem.

The key to re-balancing is predicting the bike share demand for all stations at all times as accurate as possible, and the operators can move the bikes around ahead of time according to past experiences. In this way, user satisfaction will be maximized. As many top mathematicians and computer scientists have been addressing the challenge ^3, this analysis attempts to predict space/time demand for bike share pickups in the city of Philadelphia. It considers the bike share pickup pattern at the station level by time of the pickup and locations of the station. With 5-minute interval data accounting for a 5-week period (July 8 - August 11, 2019), it hopes to inform the usefulness of such algorithms and provide insights for Indego’s re-balancing plan at any given time.

[Code](https://gillianzhaoxz.github.io/508_md/indego_bikeshare_prediction){: .btn .btn--info}

_disclamer: this is a project for a graduate course_