# EX-NO-14 — HASH ALGORITHM

## AIM

To implement Hash Algorithm.

---

# ALGORITHM

1. A Hash Algorithm is used to convert input data into a fixed-size hash value.

2. Initialize:

   * Choose a message `M`
   * Choose a hash function `H`

3. Message Processing:

   * Convert the message into blocks.
   * Apply padding if necessary.

4. Hash Generation:

   * Process the message using the hash function.
   * Generate a fixed-size hash value.

5. Output:

   * The final hash value uniquely represents the message.

6. Security:

   * Hash algorithms provide integrity and collision resistance.

---

# PROGRAM

```c id="7qrrzi"
#include <stdio.h>
#include <string.h>

int main() {
    char message[100];
    int i, hash = 0;

    printf("Enter the message: ");
    scanf("%s", message);

    // Simple hash generation
    for(i = 0; i < strlen(message); i++) {
        hash = hash + message[i];
    }

    printf("\nHash Value: %d\n", hash);

    return 0;
}
```

---

# SAMPLE OUTPUT

```text id="pknzv0"
Enter the message: hello

Hash Value: 532
```

---

# RESULT

The Hash Algorithm program was implemented and executed successfully.
