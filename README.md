## Introduction
A Data Transfer Object (DTO) in Java is a simple object used to encapsulate data and transfer it between different layers or subsystems of an application, particularly over remote interfaces like web services.
A DTO is Java pattern that simplfies data sharing to reduce the number of system calls and network ovverhead by aggregating the data into a single object for transfer.

## Benefits
Key benefits include:
- Reduced Calls: Aggregating data into one object reduces the number of round-trip network calls between client and server, improving performance.
- Decoupling: DTOs act as a boundary, preventing tight coupling between the presentation (UI) layer and the domain or persistence (database entity) layers. This allows each layer to evolve independently.
- Security and Data Privacy: DTOs allow developers to select and expose only the necessary fields, keeping sensitive data (like passwords or financial details) hidden from the client side.
- Data Shaping: DTOs can be tailored to specific use cases (e.g., a UserRequestDTO for input might differ from a UserResponseDTO for output), simplifying data handling and validation.

## Typical example
In this project, we create a web service to record and retrieve products from a database.
A product is represented by this structure:
```Product
id
name
description
price
```

We will use maven to create, build and run this code