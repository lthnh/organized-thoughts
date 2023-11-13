## Theorem proving
Applying rules of inference directly to the sentences in *KB* to construct a proof of the desired sentence without consulting models.

## Logical equivalence
Two sentences $\alpha$ and $\beta$ are logically equivalent if they are true in the same set of models.

Notation $\alpha$ $\equiv$ $\beta$.

Alternative definition: Any two sentences $\alpha$ and $\beta$ are equivalent if and only if each of them entails the other.
$$
\alpha \equiv \beta \text{ if and only if } a \models \beta \text{ and } \beta \models \alpha
$$
## Validity
A sentence is valid if it is true in *all* models.

Also known as **tautologies** - sentences that are *always* true *regardless* of the truth values of the individual statements substituted for its statement variables.
Ex: $P \lor \neg P.$

## Deduction theorem
For any sentences $\alpha$ and $\beta$, $\alpha \models \beta$ if and only if the sentence ($\alpha \implies \beta$) is valid.

Hence, we can decide if $\alpha \models \beta$ by checking if $\alpha \implies \beta$ is true in every model or by proving that $\alpha \implies \beta$ is equivalent *True*.

Conversely, the deduction theorem states that every valid implication sentence describes a legitimate inference.
