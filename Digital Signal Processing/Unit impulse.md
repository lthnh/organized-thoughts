![Unit impulse](https://qph.cf2.quoracdn.net/main-qimg-54c1ef4b3a30c8e6abd82f15b6120e7f.webp)
This is an image of unit impulse.

In DSP, an impulse sequence called a *unit impulse* takes the form
$$
x(n) = ...0,0,0,A,0,0,0...
$$
The value $A$ is often set equal to one. The above sequence is called $A$-valued sample.
## Notes
The leading sequence $A$-valued sample must be a bit longer than the length of the [[Transient response]] of the system (in case you want to test it).