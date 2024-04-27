# Architectural decision record (ADR) for Micro-frontend #2 - Products Browsing and Consultation

## Context and Problem Statement

* Division of QRmeat application into micro-frontends and responsible teams.
* Justify why this particular micro-frontend existence is relevant and how does it achieve the defined decision drivers.

## Decision Drivers

* Define independent and single-responsibility micro-frontends that allow for individual deployment.
* Ensure the ability to develop and maintain micro-frontends without affecting others.
* A micro-frontend should be reusable.
* Ensure the company can create and maintain a large-scale web application with greater flexibility and efficiency.

## Considered Options

* Products searching and consultation as a micro-frontend.

## Decision Outcome

We decided to consider product browsing, product highlights and product information consultation as a unique micro-frontend that can be assigned to a single team. The team is responsible for all features related to the presentation and sales of meat products.

### Consequences

* Good: 
    Allows teams to work on individual micro-frontends in parallel. 
    Single resposibility micro-frontend (products showcase).
    Simple in terms of features and design.
    Product´s information is not shared with other micro-frontends and does not be to stored server-side (unless updates to market are necessary).

* Bad: 
    User session information may need to be shared between micro-frontends (eg: storage of user favourite products).
    Information gathering of products can be complex.
    Dependence of external services (eg: supermarkets's products).
