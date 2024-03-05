# Architectural decision record (ADR) for Micro-frontend #1 - User Registration, Authentication and Account details 

## Context and Problem Statement

* Division of QRmeat application into micro-frontends and responsible teams.
* Justify why this particular micro-frontend existence is relevant and how does it achieve the defined decision drivers.

## Decision Drivers

* Define independent and single-responsibility micro-frontends that alllow for individual deployment.
* Ensure the ability to develop and maintain micro-frontends without affecting others.
* A micro-frontend should be reusable.
* Ensure the company can create and maintain a large-scale web application with greater flexibility and efficiency.

## Considered Options

1. ???

## Decision Outcome

We decided to consider all user specific actions (Registration, Authentication and Account Settings) a unique micro-frontend that can be assigned to a single team.

### Consequences

* Good: 
    Allows teams to work on individual micro-frontends in parallel. 
    Allows teams to be assigned to specific backend actions' implementation (separation of concerns). 
    Brings the possibility of a reusable authentication and registration page for other systems or applications. 
    This micro-frontend is independent since its only responsibility is the management of user sessions and user account details which also promotes simplicity. 
    Allows the possibility of data storage separation (users´ data can be stored server-side while products and statisitics information data can be obtained in an external way).

* Bad: User session information may need to be shared between micro-frontends (eg: storage of user favourite products).

## More Information

* ???
