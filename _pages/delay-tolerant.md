---
layout: archive
permalink: /delay-tolerant/
title: "Delay Tolerant Network"
author_profile: true
header:
  image: "/images/photo5.jpg"
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
---

## Introduction

Two villages 2 kilometres apart communicate through a Delay Tolerant Network (DTN). Village 1, which has the transceiver Node 0, sends packets to transceiver Node 1. Node 1 is in a bus that travels to the vicinity of Village 2, and back to Village 1 at a constant speed of 25 m/s. Node 1 transfers the packets to transceiver Node 2. The initial position of all nodes is depicted in the figure below.
The main task is to complete the simulation of this DTN for the transmission of 50 packets from Village 1 to Village 2 using NS-3.

<div style="width:image width px; font-size:80%; text-align:center;"><img src="{{ site.url }}{{ site.baseurl }}/images/nodes.png" alt="Initial position of the Nodes" width="width" height="height" style="padding-bottom:0.5em;" />Initial position of the Nodes</div>





You can check out the project on [GitHub](https://github.com/nbolar/Delay-Tolerant-Network).

## Node Operation
Packets generated in Village 1 are sent to the bus. The bus acknowledges the reception of each packet. As soon as a packet is acknowledged, Village 1 sends a new packet to the bus. If a packet is not acknowledged by the bus, Village 1 keeps transmitting the current packet until received successfully by the bus.

After receiving a packet from Village 1, the bus starts transmitting that the bus stops transmitting the current packet upon receiving an acknowledgement from packet to Village 2. Village 2. Note that it is possible for the bus to receive several packets from Village 1 before successfully sending the current packet to Village 2.

Upon receiving a data packet from the bus, Village 2 sends an acknowledgement.

### Several different methods were implemented so as to ensure the accurate delivery of all the 50 packets such as constant mobility model, Gauss-Markov Model, etc. This can be seen in the code.

## Conclusion

A delay-tolerant network is a network designed to operate effectively over large distances. In such an environment, long latency, sometimes measured in hours or days is inevitable. It can be used to connect places that do not have access to internet by using a node to transfer data packets from the a area of no internet connectivity to another area that has access to internet and vice-versa. In this particular project we implemented that very same idea. In such environments, popular ad hoc routing protocols such as AODV fail to establish routes. Based on the experiments carried out in this project it was observed that the time delay in receiving all the packets is a function of the speed on the mobile node. The mobility model that is used in the real world will also largely affect the successful arrival of packets.

<!-- <ul>
  {% for post in site.categories.delay %}
    <li>
      <a href="{{ post.url }}">{{ post.title }} {{ post.date | date_to_string }}</a>
    </li>
  {% endfor %}
</ul> -->
