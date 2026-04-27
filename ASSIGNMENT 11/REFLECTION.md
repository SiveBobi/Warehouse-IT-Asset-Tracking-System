# Reflection

Implementing a persistence repository layer highlighted the importance of separating storage concerns from business logic.

One challenge was designing a generic repository that remained reusable while supporting asset-specific behavior. Generics solved duplication concerns while entity-specific repositories preserved flexibility.

Another challenge was deciding between Dependency Injection and Factory Pattern. Factory Pattern was selected because it provides simpler storage switching for this project while supporting future extensibility.

Implementing the in-memory HashMap repository reinforced CRUD concepts and demonstrated how repositories improve testability without requiring a real database.

Future-proofing through stub implementations also showed how scalable software design anticipates growth.
