# Catalyst
Nothing here yet

# Goal
This project aims to help in developing domains using CQRS /  Event Sourcing, focusing on what matter (the domain) by providing an accessible (and replaceable) runtime infrastructure for it

# What you have to write
1. Commands
2. Events
3. Aggregate roots
4. Read models
5. Functions for command handling and events projections

# Then this project aims to provide thing like:
1. Polymorphic JSON serialization configuration for commands and events 
2. REST endpoints (for each Aggregate Root) with Swagger support for submiting commands
3. Messaging functionality
4. Database persistence

# Stack
This will be based on Apache Camel and Postgres. Both are Swiss Army Knives and are enough to have your domain up and running, ready to explore. The point is: once your domain is validated, you can leverage it in another stack of your choice. 
