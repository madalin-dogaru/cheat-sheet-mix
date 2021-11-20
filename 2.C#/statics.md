- Static means “associated with the class, not an instance”. Thus any static member is accessed from the class, not an instance   
- If you tried to access a static member from an instance (like f.Definition) you would get an error    
- When creating static methods we add static to both the field definition and method Define(). This is because a static method can only access other static members.   
  It cannot access instance members.
