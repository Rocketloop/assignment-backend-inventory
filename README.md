# Rocketloop Coding Assignment - Inventory Management API

Hi there 👋

Whether you have been sent this assignment in response to an interview with us or you have stumbled upon it by chance, we are excited you are here. Rocketloop is always looking for smart, passionate people that want to use their skills and talents to create awesome things, so if you are interested in taking on a new challenge, working with a world-class team of passionate and technology-loving people, we would love for you to take on this assignment.

## Objective

In this assignment, you will be building a small back-end application that provides an API to manage and organize inventory for a small grocery store. The store has multiple spaces where items can be located and items of different types that can be stored in different spaces. Some items also have an expiration date, after which the item cannot be sold anymore and needs to be removed from the store.

## Requirements

The API you are going to build should be able to fulfill the following functionality and requirements:

### Storage Spaces

- A **storage space** has a name and a maximum capacity (e.g. 100 items)
- A storage space can be refrigerated
- New storage spaces can be created
- Existing storage spaces can be renamed
- Existing storage spaces can be removed, if they are empty, i.e. there are no items assigned to them
- A storage space can never be assigned more items than its maximum capacity
- It should be possible to retrieve a list of all items assigned to a given storage space

### Item Types

- Each **item type** has a name that describes what item it is (e.g. "Ice Cream Sandwich") and whether it needs refrigeration
- Multiple items can share one item type, i.e. there can be multiple items of type "Ice Cream Sandwich"
- New item types can be created
- Existing item types can be renamed
- Existing item types can be removed, if there are no items of the given type

### Items

- Each **item** has an item type and an expiration date
- Each item must be assigned to a single storage space
- An item that has an item type that requires refrigeration cannot be assigned to a storage space that is not refrigerated
- New items can be created. The item's expiration date must be in the future.
- Items can be moved to another storage space if the constraints allow it
- Existing items cannot be changed, i.e. neither the type nor the expiration date can be changed
- Existing items can be removed
- It should be possible to retrieve a list of all items, optionally sorted by expiration date. This list should support pagination.

## Implementation Details

### Languages and Frameworks

We are currently accepting submissions for both Python and Node.js/TypeScript. If you are planning on using Python to solve the assignment, please make sure to make use of a modern, asynchronous Python framework, such as FastAPI or Sanic. If you are planning on using Node.js to solve the assignment, please make sure to use a modern Node.js framework that supports TypeScript. In any case, please make sure to use the latest stable version of all languages and frameworks used.

### Database

For this assignment, please make use of a relational database, such as PostgreSQL or SQLite. Also, make sure to use an ORM for all database interactions where it is possible.

### External Libraries and Sources

You are free to use any external library to complete this assignment, as long as the library's license is not restrictive or incompatible with the MIT license. You are also free to use external sources such as StackOverflow if necessary, as long as you clearly mark and attribute any and all code not written by yourself.

## Deliverable

Please clone or fork this repository and use it as a starting point for your submission. The repository and version history of your code should be part of your submission. Your submission should be self-contained and runnable using a single command. It is highly preferred to use Docker and docker-compose to package your submission. Please make sure to include instructions on how to run your solution and an overall description of what you have built with your submission as part of a README. 
