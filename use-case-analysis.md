# Use Case Analysis — News Channel Program

## 1. Purpose

This document defines the actors, use cases, and associations for a prime-time television news program. The purpose is to clarify the system's scope and show how editorial, technical, audience, and commercial participants interact with the program.

## 2. System boundary

**System:** News Channel Program

The system covers preparation and delivery of news content, the live broadcast, audience interaction, broadcast equipment support, and the placement of advertisements.

The model focuses on high-level interactions. It does not specify internal workflows, technical architecture, or detailed business rules.

## 3. Identify the actors

| Actor | Type | Role and interaction |
| --- | --- | --- |
| **News producer** | Primary | Plans segments, selects topics, assigns reporters, and coordinates live coverage. |
| **Reporter** | Primary | Gathers information, conducts interviews, contributes stories to segments, and reports live. |
| **Viewer** | Secondary | Watches the broadcast and shares comments or feedback through social media. |
| **Technical team** | Supporting | Sets up, maintains, and troubleshoots the equipment used for the broadcast. |
| **Advertiser** | External | Submits advertisements and coordinates their placement with the channel. |

*Actor classification is based on each participant's role in the modeled interactions; it is not a statement about organizational hierarchy.*

## 4. Define the use cases

| Use case | Description |
| --- | --- |
| **Create news segment** | Select a topic, gather material, and assign a reporter to prepare a segment for broadcast. |
| **Report news live** | Deliver news, interviews, and updates on air as events unfold. |
| **View program** | Watch the live news broadcast. |
| **Interact via social media** | Comment on stories, share feedback, or participate in a discussion about the broadcast. |
| **Manage broadcast equipment** | Prepare and check cameras, microphones, and broadcast software, and resolve faults during production. |
| **Provide advertisement** | Submit an advertisement and coordinate when it will air during a commercial break. |

## 5. Define the relationships

The diagram contains eight actor-to-use-case associations:

| Actor | Use case | Participation |
| --- | --- | --- |
| News producer | Create news segment | Plans and develops the segment. |
| News producer | Report news live | Supports the broadcast by coordinating with reporters. |
| Reporter | Report news live | Delivers the story on air. |
| Reporter | Create news segment | Contributes interviews and information for the segment. |
| Viewer | View program | Watches the live broadcast. |
| Viewer | Interact via social media | Comments on the program and gives feedback. |
| Technical team | Manage broadcast equipment | Checks equipment and resolves technical problems. |
| Advertiser | Provide advertisement | Submits an advertisement and coordinates placement. |

These are associations between actors and use cases. The model does not introduce `include` or `extend` relationships because the exercise does not define use cases that require those relationships.

## 6. Model interpretation

The news producer and reporter are the primary actors in the editorial and live-reporting activities. The viewer interacts with the program through viewing and social feedback. The technical team supports continuity of the broadcast by managing equipment, while the advertiser participates in the commercial component.

Separating actors from use cases makes the system boundary easier to understand and provides a starting point for more detailed requirements gathering.

## 7. Scope and assumptions

- The model represents a high-level prime-time news program.
- Social media interaction is treated as an interaction associated with the program; the external social platform is not modeled as a separate actor.
- Advertisement submission and placement are represented as one high-level use case.
- Equipment management is represented as one supporting use case.
- Detailed schedules, approval rules, user permissions, integrations, and non-functional requirements are outside this exercise's scope.

## 8. Deliverable

See the [UML use case diagram](diagrams/news-channel-use-case-original.png) for the visual representation of the five actors, six use cases, and eight associations.
