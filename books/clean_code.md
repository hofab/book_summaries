#Clean Code

### Meaningful Names
The hardest thing about choosing good names is that it requires good desscriptive skills and a shared cultural background. This is teaching issue rather than a technical, business, or managment issue. You will probably end up suprising someone when you rename, just like you might with any oher code improvment. **Don't let is stop you in your racks**

### Functions
- Small
- Do one Thing
- One Level of Abstraction per Function
- Use Descriptive Names
- Avoid Flag Argumets (boolean)
- Use Argument Lists
- Error Handling is One Thing

### Comments
- Explain yourself in Code
- **Good Comments**
  - Legal Comments
  - Informative Comments
  - Explanation of Intent
  - Clarification
  - Warning of Consequences
  - TODO Comments
  - Amplification
- **Bad Comments**
  - Mumbling
  - Redundant Comments
  - Mandated Comments
  - Journal Comments
  - Noise Comments
  - Scary Comments
  - Closing Brace Comments
  - Commnted-Out Code
  - Nonlocal Information
  - Too much information
  - Inobvious Connection
- Don't use a Comment When you can use a function or variable
- Short functions don't need much description

### Formatting
- **Have Team Rules** everybody can agree on
- Use tools to format

### Objects and Data Structures
- Objects hide their data behind abstactions and expose functions that operate on the data.
- Data sructures expose their data and have no meaningful functions.
- Objects expose behavior and hide data. this makes it easy to add new kinds of objects without changing existing behavors. It also makes it hard to add new behaviors to existing objects.
- Data structures expose data and have no significant behavior. This makes it easy to add new behavior to exising data sructures but makes it hard to add new data structures to existing funcions.

### Error Handling
- **Don't pass NULL**

### Boundaries
- Wrap classes or interfaces that provide excessive functionality. The resulting interface should be tailored and constrained to meed the needs of the application. The resulting class can enforce design and business rules.
- Write **Learning Test** for libraries or interfaces you want to use. These are usually simple boundary tests. It simplifies migration to newer versions, by ensuring strict behavior.
- Useing Code that does not yet exist. Write placeholder interfaces which can be filled in later. A glue adapter can be written to transform the placeholder interface to the actual implemenation.

### Unit Tests

