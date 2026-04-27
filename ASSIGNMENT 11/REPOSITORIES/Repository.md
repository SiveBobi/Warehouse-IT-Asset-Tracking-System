# Generic Repository Interface

```java
public interface Repository<T, ID> {

    void save(T entity);           // Create / Update

    Optional<T> findById(ID id);   // Read

    List<T> findAll();             // Read All

    void delete(ID id);            // Delete
}
```

## Justification

Generics were used to avoid duplication across repositories and promote reuse.

Benefits:
- Consistent CRUD behavior
- Reusable design
- Easy to support multiple entities
- Supports future storage backends
