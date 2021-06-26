# Read: Class 01
## Component-based architecture :
focuses on the decomposition of the design into individual functional or logical components that represent well-defined communication interfaces containing methods, events, and properties. It provides a higher level of abstraction and divides the problem into sub-problems, each associated with component partitions.
## Component:
is a modular, portable, replaceable, and reusable set of well-defined functionality that encapsulates its implementation and exporting it as a higher-level interface.
A component is a software object, intended to interact with other components, encapsulating certain functionality or a set of functionalities. It has an obviously defined interface and conforms to a recommended behavior common to all components within an architecture.
## Characteristics of Components:
1. **Reusability**
2. **Replaceable**
3. **Not context specific**
4. **Extensible**
5. **Encapsulated**
6. **Independent**
## Advantages of using components:
1. **Ease of deployment**:  As new compatible versions become available, it is easier to replace existing versions with no impact on the other components or the system as a whole.
2. **Reduced cost**:  The use of third-party components allows you to spread the cost of development and maintenance.
3. **Ease of development**: Components implement well-known interfaces to provide defined functionality, allowing development without impacting other parts of the system.
4. **Reusable**: The use of reusable components means that they can be used to spread the development and maintenance cost across several applications or systems.
5. **Modification of technical complexity**: A component modifies the complexity through the use of a component container and its services.
6. **Reliability**: The overall system reliability increases since the reliability of each individual component enhances the reliability of the whole system via reuse.
7. **System maintenance and evolution**: Easy to change and update the implementation without affecting the rest of the system.
8. **Independent**: Independency and flexible connectivity of components. Independent development of components by different group in parallel.
## Props:
Is a special keyword in React, which stands for properties and is being used for passing data from one component to another.
> * But the important part here is that data with props are being passed in a uni-directional flow. (one way from parent to child).
> * Furthermore, props data is read-only, which means that data coming from the parent should not be changed by child components.
## Using Props in React:
1. Define an attribute and its value(data)
2. Then pass it to child component(s) by using Props
3. Render the Props Data