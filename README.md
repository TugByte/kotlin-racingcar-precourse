# kotlin-racingcar-precourse

## Functional Requirements

### Setup
- Ask the user to enter **car names** (comma-separated), e.g.:
pobi,woni,jun

- Ask the user to enter the **number of rounds** the race will run.

### Car Name Rules
- Each car must have a name.
- Car names **must not exceed 5 characters**.
- If the input is invalid (e.g. blank name or name longer than 5 characters), the program must:
- Throw an `IllegalArgumentException`
- Stop execution immediately

### Logic
- The race runs for the number of rounds entered by the user.
- In each round, every car:
- Randomly generates a number between **0 and 9**
- **Moves forward by one step** if the number is **4 or higher**
- Otherwise, the car stays in its current position

### Displaying Progress
- After each round, show how far each car has moved so far
- Format:
car-name : ---

- Each `-` represents one forward move

### Determining the Winner
- After the final round:
- Determine which car(s) moved the farthest
- Display the winner(s)

#### Output Format:
- **Single winner**:
-  **Multiple winners (tie)**:
