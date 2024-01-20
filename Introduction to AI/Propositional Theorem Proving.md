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

## Satisfiability
A sentence is satisfiable if it is true in *some* model.

Validity and satisfiability are connected: $\alpha$ is valid iff $\neg \alpha$ is unsatifiable; contrapositively, $\alpha$ is satisfiable iff $\neg \alpha$ is not valid.

We also have the following useful result:
$$
\alpha \models \beta \text{ if and only if the sentence } (\alpha \land \neg \beta) \text{ is unsatisfiable.}
$$
Intuition for the result above:
$$
(\alpha \implies \beta) \equiv (\neg \alpha \land \beta) \equiv \neg (\alpha \lor \neg \beta) \text{ (De Morgan)}
$$

Proving $\beta$ from $\alpha$ by checking the unsatisfiability of $(\alpha \lor \neg \beta)$ corresponds exactly to the standard mathematical proof technique of *reductio ad absurdum* - reduction to a absurd thing. It is also called proof by **refutation** or proof by **contradiction**.

## Proof by resolution

To do this, we introduce a single inference rule called **resolution** that yields a complete inference algorithm when coupled with any complete search algorithm.

For example, we have $A \lor B \lor C$ in the knowledge base. Then we also $\neg A \text{ and } \neg B$. We can resolve with the knowledge base by applying resolution rule to give the *resolvent*:
$$
\displaylines{
A \lor B \lor C \text{ resolves with } \neg A \text{ gives resolvent } B \lor C \\
B \lor C \text{ resolves with } \neg B \text{ gives resolvent } C
}
$$

These last two inference steps are examples of the **unit resolution** inference rule
$$
\begin{prooftree}
\AXC{$l_{1} \lor \ldots \lor l_{2}$}
\AXC{m}
\BIC{$l_{1} \lor \ldots \lor l_{i-1} \lor l_{i+1} \lor \ldots \lor l_{k}$}
\end{prooftree}
$$
where each $l$ is a literal and $l_{i}$ and $m$ are **complementary literals**(i.e., one is the negation of the other).

This can be generalized to the full **resolution** rule
$$
\begin{prooftree}
\AXC{$l_{1} \lor \ldots \lor l_{2}$}
\AXC{$m_{1} \lor \ldots \lor m_{n}$}
\BIC{$l_{1} \lor \ldots \lor l_{i-1} \lor l_{i+1} \lor \ldots \lor l_{k}
	\lor m_{1} \lor \ldots \lor m_{j-1} \lor m_{j+1} \lor \ldots \lor m_{n}$}
\end{prooftree}
$$
where $l_i$ and $m_{j}$ are complementary literals.
This says that resolution takes two clauses and produces a new clause containing all the literals of the two original clauses *except* the two complementary literals.

You can resolve *only one* pair of complementary literals at a time.

The resulting clause should contain only one copy of each literal. The removal of multiple copies of literals is called **factoring**.

### Conjunctive normal form
Every sentence of propositional logic is logically equivalent to a conjunction of clauses.
$$
\displaylines{
CNTSentence \rightarrow Clause_{1} \land \ldots \land Clause_{n} \\ 
Clause \rightarrow Literal_{1} \lor \ldots \lor Literal_{m} \\
Fact \rightarrow Symbol \\
Literal \rightarrow Symbol \mid \neg Symbol \\
Symbol \rightarrow P \mid Q \mid R \\
HornClauseForm \rightarrow DefiniteClauseForm \mid GoalClauseForm \\
DefiniteClauseForm \rightarrow Fact \mid (Symbol_{1} \land \ldots Symbol_{l}) \implies Symbol \\
GoalClauseForm \rightarrow (Symbol_{1} \land \dots \land Symbol_{l}) \implies False
}
$$
Above is the grammar for conjunctive normal form, Horn clauses, and definite clauses.