```mermaid
flowchart TD
    Start([Start]) --> A[Create a random number]
    A --> B[Ask the user for a guess]
    B --> C{Is the user's input a valid value?}
    C -- "Yes" --> D{Is the user's guess correct?}
    C -- "No" --> E[Display bad input]
    E --> B
    D -- "Too High" --> F[Display is too high]
    F --> B
    D -- "Too Low" --> G[Display is to low]
    G --> B
    D -- "Correct" --> H[Display the user is correct!]
    H --> End([End])
```
## Step by step guide of my Guessing Game Diagram


Now we check if the input is valid:
*   If the user’s input is valid-- a numeric value that’s within range-- then proceed to the next step.
*	If the user’s input is invalid then display an error message and go back to prompting the user again.
