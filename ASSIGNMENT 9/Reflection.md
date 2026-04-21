# Reflection: Domain Modeling and Class Diagram

Designing the domain model and class diagram for the Warehouse IT Asset Tracking System presented several challenges. One of the primary challenges was identifying the correct level of abstraction for the system entities. It was important to include enough detail to accurately represent the system while avoiding unnecessary complexity.

Another challenge was defining relationships between entities. Deciding when to use association, inheritance, or composition required careful consideration. For example, inheritance was used for Admin and Technician classes to extend the User class, as they share common attributes but have specialized behaviors.

Mapping the domain model to previous assignments was also crucial. The entities and relationships had to align with functional requirements, use cases, and state diagrams. For instance, the FaultReport entity directly supports the fault reporting use case, while the MaintenanceRecord entity aligns with maintenance tracking requirements.

Defining methods for each class was another area that required attention. The methods needed to reflect actual system behavior without being overly detailed. This balance ensured that the diagram remained understandable while still being useful for implementation.

One trade-off made was simplifying some relationships to keep the diagram readable. While more complex relationships could have been modeled, simplicity was prioritized to enhance clarity.

This assignment reinforced the importance of object-oriented design principles. It highlighted how proper modeling can improve system understanding and guide implementation.

Overall, the process improved my ability to design structured and scalable systems while maintaining alignment with requirements and user needs.
