Here's Noir circuit to prove and verify ownership of a NFT from a paricular collection (i.e. address) on Aztec. \
The circuit takes block number as a point for which assertions are made and required data. The proof asserts that the address has a note from the contract and it's not nullied.
For proving user needs access to the PXE with their data and preimage of the note they'd like to use for proving. For verification only exported data of the block is needed, so it could be done *completely without access to the chain* (or even Internet if user can handover the proof).

Coming soon:
- generalization to accept more notes types,
- folding proofs at number of blocks,
- if you have a demand -- add it as an issue.

<./artifacts>       contains compiled items. \
The contract dir    contains the helper contract needed to get witnesses from PXE while proving. \
<./circuit>         contains the Noir app. \
<./tests>           contains script and data useful for development. 

There couple of ways to run a circuit. <https://noir-lang.org/docs/dev/tutorials/noirjs_app#some-noirjs> describes JS way to use it.

# example
will be added here from <tests/ts/index.ts> \
(use the file meanwhile)