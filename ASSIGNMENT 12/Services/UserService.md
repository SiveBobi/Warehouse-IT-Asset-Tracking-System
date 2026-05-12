# User Service

```java
public class UserService {

 private final UserRepository userRepo;

 public UserService(
 UserRepository userRepo){
   this.userRepo = userRepo;
 }

 public User createUser(User user){

   if(user.getEmail()==null){
      throw new IllegalArgumentException(
      "Email required");
   }

   userRepo.save(user);

   return user;
 }

 public List<User> getAllUsers(){
   return userRepo.findAll();
 }

}
```
