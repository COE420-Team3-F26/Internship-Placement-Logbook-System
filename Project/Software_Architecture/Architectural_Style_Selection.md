
# Exercise 2: Select and Justify an Architectural Style

For our Internship Placement and Weekly Logbook System, we chose the Layered Architecture style. This style organizes the system into separate layers, with each layer responsible for a specific part of the system.

Our architecture consists of three layers:

1. Presentation Layer: This layer handles user access and interaction with the system. It includes User & Access Management, which provides authentication and controls what functions each user role can access.

2. Application Layer: This layer contains the main system functionality. It includes Application Management, Placement Management, Logbook & Progress Monitoring, and Notification & Feedback. Each component handles a different part of the internship process.

3. Data Layer: This layer is responsible for storing and retrieving information through the database, including user accounts, applications, placements, logbooks, and feedback records.

We selected Layered Architecture because it matches the way our system is organized. Separating the system into layers and components makes it easier to maintain, test, and update individual functions without affecting unrelated parts of the system.

This style also supports the design goals identified in Exercise 1. For security (DG-01), authentication and role-based access control are handled through User & Access Management. Maintainability (DG-02) is supported by separating the main system functions into components with clear responsibilities. Reliability (DG-03) benefits from centralized data storage, which allows records and relationships to be managed consistently. Performance (DG-04) is considered by keeping the functionality organized into separate modules, although the actual response-time requirements will still need to be tested.

One of the main advantages of this style is that the components can be developed and maintained separately. It also makes the structure easier to understand and allows changes to be made without redesigning the entire system.

However, there are some limitations. Communication between layers can introduce additional overhead, and changes to shared interfaces or the database may affect multiple components. These dependencies need to be considered during development.

Overall, Layered Architecture is suitable for our project because it provides an organized structure that supports the system's main functions and architectural design goals.
