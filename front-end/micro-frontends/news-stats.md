# Architectural decision record (ADR) for Micro-frontend #3 - News and Statistics

## Context and Problem Statement

* Division of QRmeat application into micro-frontends and responsible teams.
* Justify why this particular micro-frontend existence is relevant and how does it achieve the defined decision drivers.

## Decision Drivers

* Define independent and single-responsibility micro-frontends that allow for individual deployment.
* Ensure the ability to develop and maintain micro-frontends without affecting others.
* A micro-frontend should be reusable.
* Ensure the company can create and maintain a large-scale web application with greater flexibility and efficiency.

## Considered Options

* News and Statistics as a micro-frontend.
* News and Statistics as indepdendent micro-frontends.

## Decision Outcome

We decided to consider news and statistics as a unique micro-frontend that can be assigned to a single team without having too much worload on the team. The team is responsible for the presentation and collection of updated news and statistics.

### Consequences

* Good: 
    Allows teams to work on individual micro-frontends in parallel. 
    Single resposibility micro-frontend (News and Statistics).
    Completely independent from other micro-frontends.
    Simple in terms of features and design.
    News´ and statistics data is not shared with other micro-frontends and does not be to stored server-side.

* Bad: 
    Information gathering of updated news and statistics can be complex.
    Dependence of external services (eg: statistics and news provider).
    
