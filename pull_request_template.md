## 📋 Project Assessment: Lab 04 - D&D + Abstract Classes

### 1. Git & Workflow
- [ ] **Commit Messages:** Descriptive and incremental (e.g., "Defined abstract methods in GameCharacter" or "Implemented Elf-specific attack logic").

### 2. Functional Requirements
- [ ] **Weapon (Concrete Class):**
    - [ ] **Instance Variables:** Implements 4 variables (name, damage, etc.) with correct types.
    - [ ] **Validation:** Error checks that `int` values are $\ge 0$ and `String` values are not null/empty.
    - [ ] **Standard Methods:** Includes full, no-parameter, and copy constructors; getters/setters; `toString`; and `equals`.
- [ ] **GameCharacter (Abstract Class):**
    - [ ] **Abstract Definition:** Correctly uses the `abstract` keyword; contains the 9 specified instance variables.
    - [ ] **Composition & Deep Copy:** Correctly handles first `Weapon` instance variables (not allowing `null`) with deep copying in setter and getter.
    - [ ] **Composition & Deep Copy:** Correctly handles second `Weapon` instance variables (allowing `null` for empty slots) with deep copying in setter and getter.
    - [ ] **Validation:** Comprehensive error checking for all `int` ($\ge 0$) and `String` (present) parameters.
    - [ ] **Abstract Methods:** Defines `assist(GameCharacter target)` and `attack(GameCharacter target)` without bodies.
- [ ] **Elf & Dwarf (Concrete Subclasses):**
    - [ ] **Inheritance:** Correctly uses `extends GameCharacter`.
    - [ ] **Constructors:** Implements full, no-parameter, and copy constructors using `super()` to initialize inherited state.
    - [ ] **assist() Implementation:** Provides a positive action (e.g., healing `hitPoints` or adding `gold`), implemented in both `Elf` and `Dwarf`.
    - [ ] **attack() Implementation:** Implements damage logic (e.g., based on `armorClass` and `expPoints`) in both `Elf` and `Dwarf`.
- [ ] **Driver Program (Main.java):**
    - [ ] **Implementation:** Instantiates at least one concrete character (`Elf` or `Dwarf`).
    - [ ] **State Verification:** All variables are set via constructors/setters and printed to console to verify accuracy.

### 3. Code Quality & Standards
- [ ] **OOP Standards:**
    - [ ] All instance variables are `private`.
    - [ ] Effectively uses the `GameCharacter` type for method parameters to support polymorphism.
- [ ] **Annotations:** `@Override` flag used correctly above all overridden methods.
- [ ] **Naming & Formatting:** Consistent `camelCase` for methods/variables and `PascalCase` for classes.
- [ ] **Code Structure:** Single-line blocks use curly braces; indentation is consistent throughout.
- [ ] **Constants:** Final constants are used for default character stats or weapon values.
- [ ] **Documentation:** Every method (excluding `@Override`) and class includes JavaDoc syntax. Includes class-level descriptions and class-invariants.
