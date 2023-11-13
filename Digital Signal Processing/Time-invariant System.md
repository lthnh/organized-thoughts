A time-invarient system is one where a time delay (or shift) in the input sequence causes an equivalent time delay in the system's output sequence.
Ex:
$$
\displaylines{
x(n) \xrightarrow{\text{results in}} y(n) \\
x'(n) = x(n+k) \xrightarrow{\text{results in}} y'(n) = y(n+k)
}
$$
where $k \in \mathbb{Z}$ and represents $k$ sample period time delays.

For system to be time-invariant, the above equation must hold true for any integer value of $k$ and any input sequence.

Formally stated, a time-invariant system is one where a time shift in an input sequence results in an equal time shift in the output sequence. In the literature this is called *shift-invariant* systems.