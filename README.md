# Catalyst
Nothing here yet

# Goal
This project aims to help in developing domains using CQRS /  Event Sourcing, focusing on what matter (the domain) by providing an accessible (and replaceable) runtime infrastructure for it

# What you have to write (the domain)
1. Commands
2. Events
3. Aggregate roots
4. Read models
5. Functions for Command handling
6. Functions for Aggregate Root projection 
7. Functions for Read Models projections

# Then this project aims to provide (the infrastructure)
1. Polymorphic JSON serialization configuration for commands and events 
2. REST routes with Swagger support for submiting commands
3. Routes to validate submitted commands and once validated, to enqueue then for further processing
4. Routes to listen for arriving commands, process them and enqueue resulting events
5. Routes to listen for published events and submiting them to read model's projections
6. A Journal implementation for storing commands as JSON
7. An EventRepository implementation for events stored as JSON

# Software stack
This will be based on Apache Camel and Postgres. Both are like Swiss Army Knives and enough to have your domain up and running, ready to explore and integrate with your application. And if your solution needs to meet a higher level of non functional requirements, you can leverage the resulting domain in another stack of your choice.

The point is: you can spend your precious time on what's really matter, your domain. 
