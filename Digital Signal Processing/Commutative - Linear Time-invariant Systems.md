Due to this property, LTI systems sequential order can be rearranged with no change in their final output

```mermaid
flowchart LR
	a["x(n)"] --> b["LTI
	System #1
	"]
	b -->|"f(n)"|c["LTI
	System #2
	"]
	c --> d["y(n)"]
```
```mermaid
flowchart LR
	a["x(n)"] --> b["LTI
	System #2
	"]
	b -->|"f(n)"|c["LTI
	System #1
	"]
	c --> d["y(n)"]
```

The graph above show LTI systems in series. Swapping order of the two systems does not change the output $y(n)$