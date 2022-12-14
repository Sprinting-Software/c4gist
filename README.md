# C4 Gist

The gist of software architecture.

## About this document

This open-source document sets out to create a gist of the ideas on software architecture diagramming that was first published by the C4-model: https://c4model.com/

## Core concepts

- **System**: A **system** is the highest level of abstraction and describes something that delivers value to its users, whether they are human or not. Systems provides a strong organising factor in enterprises. Often teams structure, access control and servicer-ownership follows the system boudaries.

- **Component**: A system is constituted by one or more distinct and non-overlapping **components** which are tangible parts of the code-base with clear boundaries. Each components can be separately deployed into a running state and when all components are deployed they will interact in ways that realize the use-cases of the system.

- **Sub-component**: A component is constituted by code which may have a logical structure which can be perceived as inner elements referred to as **sub-components**.

- **Deployment node**: A component can be deployed in a deployment node, which brings to live the component from code to a running thing.

## Relationships between core concepts

The following shows the relationships between the core concepts.

```
     System
        |
        |
       / \
     Component  >--<  Deployment-node
        |
        |
       / \
     Sub-component >-|
             \ /     |
              |______|

```

## Proposed legend

![](images/legend.png)
