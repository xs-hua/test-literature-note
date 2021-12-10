
*Trade-off between on-chain and off-chain while designing* [Xu et al., 2019]
- **On-chain:**
    - Data and computation are placed inside the blockchain component, using the ledger and smart contracts
    - The shortcomings sit at limited amount of computational power, limited data storage space, limited control of read accesses on a blockchain and so on
    - Usually small-sized public data is placed on-chain, while large or private data is placed off-line.

- **Off-chain:**
    - data and computation are hosted off-line outside the blockchain component, application logic implemented externally. 
    - A typical overhead sit at the interface between on-chain and off-chain logic.
    - It is inevitable to keep large data off-chain.

*Design Patterns of Blockchain-based Application*

- **Oracle**
    - introducing the state of external systems into the closed blockchain execution environment.
    - The execution environment of blockchain is isolated, but in a blockchain-based system it needs to access the other external components.
    - The self-contained blockchain component is connected with the external world via Oracle.

- **Reverse Oracle**
    - The off-chain components of an existing system rely on smart contracts run-ning on a blockchain to supply requested data and check required conditions.
    - The data and property of blockchain is accessible to the non-blockchain com-ponent by integrating blockchain component into existing system via reverse oracle.

- ...

*Challenges of testing blockchain-based app:*
- lack of best practices. [Lal., 2021]
- Currently there are new tools available for testing, debugging and development, but they are either not mature or don’t meet all needs during the testing process.
- the immutability of blockchain is a considerable challenge, the data once committed will be on-chain, and testing can be only executing properly in a proper test environ-ment. Therefore, re-running tests requires re-establishing the test environment [Weber et al., 2021]
- similar problems encountered when testing distributed system. 

<br/>

*References:*

*Xu, X., Weber, I., and Staples, M. (2019). Architecture for Blockchain Applications. Springer, 2019, pp. 83-148.*
*Koul, Rohan. Blockchain Oriented Software Testing – Challenges and Approaches.  In: 2018 3rd International Conference for Convergence in Technology.*


