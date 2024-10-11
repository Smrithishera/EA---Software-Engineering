This is a simulation prepared as a Software Engineer in Electornic Arts through Forage.
In this I completed two major tasks

### Improved Inventory System
Completed the class definitions for the game objects outlined in the class diagram from the previous task. Each class is designed to support the expected interactions and operations required for the game.

### Created Characters
After completing the core functionality of the inventory system, I took the opportunity to review and improve the existing code. Specifically, I focused on the way items were stored in the inventory. 

#### Improvements Made

 **Transition from C-style Arrays to `std::vector`**:
   - **Original Implementation**: The inventory system initially used a C-style array to store items. This approach had several drawbacks, including fixed size limitations, manual memory management, and potential buffer overflow risks.
   - **New Implementation**: I replaced the C-style array with `std::vector`. This change offers several advantages:
     - **Dynamic Sizing**: Vectors automatically resize as items are added or removed, eliminating the need for manual memory management and making the inventory system more flexible.
     - **Safety**: Using vectors minimizes the risk of buffer overflows, as they handle bounds checking internally.
     - **Ease of Use**: The STL (Standard Template Library) provides various member functions for vectors, such as `push_back()`, `pop_back()`, and `size()`, which simplify adding and removing items from the inventory.
     - **Cleaner Code**: The implementation becomes more straightforward and readable, reducing boilerplate code associated with manual array management.
