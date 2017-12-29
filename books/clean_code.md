# Clean Code

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
- **Three Laws of TDD**
  - **First Law:** You may no write production code until you have witen a failing unit test.
  - **Second Law:** You may not write more of a unit test than is sufficient to fail, and not compiling is failing.
  - **Thirs Law:** You may not wrie more productions code than is sufficient to pass the currently failing test.
- Keep tests clean
- **One assert per test**
- Test only one single concept
- **F.I.R.S.T.**
  - **Fast**
  Tests should be fast. They should run quickly. When tests run slow, wou won't want to run them frequently. If you don't run them freequently, you won't find problems early enough to fix them easily. Wou won't feel as free to clean up he code. Evntually the code will begin to rot.
  - **Independent**
  Tests should not depend on each other. One test should not set up he conditions for the next tests. ou should be able to run each test independently and run the tests in any order you like. When tests depend on each other, then the first one to fail causes a cascade of downstream failures, making diagnosis difficulat and hiding downstream defects.
  - **Repeatable**
  Tests should be repeatable in any environment. You should be able to run the tests in the production environment, in the QA environment, and on your laptop while riding home on he train without a network. If your tests aren't repeatable in any environmen, hen you'll always have an excuse for why they fail. You'll also find yourself unable to run the tests when the environment isn't available.
  - **Self-Calidating**
  The tests should have a boolean output. Either the pass or fail. You should not have to read hrough a log file to tell wheher the tests pass. You should no have to manually compare two different tecx files to see whether the tests pass. If the tests aren't self-validating, then failure can become subjective and running tests can require a long manual evaluation.
  - **Timely**
  The tests need to be writen in a timely fashion. Unit tests should be writen just before the production code that makes them pass. If you write tests after the producion code, then you may find the production code to be hard to test. you may decided that some production code is too hard to test. you may not design the production code to be testable.

### Classes 
- Encapsulation
- Classe should be small
- The **single reesponsibility principle** sates that a class or module should have one, and only one, reason to change.
- Maintaining cohesion results in many small classes
- Classes should be open for etension but closed for modification (**Open-Closed Principle**)
- Isolating from change
