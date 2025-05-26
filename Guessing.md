# Guessing Game Flowchart

```mermaid
flowchart TD
    Start([Start]) --> GenerateNumber([Generate Random Number])
    GenerateNumber --> GetUserInput([Get User Guess])
    GetUserInput --> CheckGuess([Check Guess])
    CheckGuess -->|Too High| GetUserInput
    CheckGuess -->|Too Low| GetUserInput
    CheckGuess -->|Correct| End([End])
