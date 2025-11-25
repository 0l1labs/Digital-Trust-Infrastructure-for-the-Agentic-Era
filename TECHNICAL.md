# Technical Architecture

## Zero-Knowledge Proof Flow
```
User Action → Witness Generation → Circuit Compilation → Proof Generation → On-Chain Verification
```

### 1. Witness Generation
Client-side WASM module processes private inputs (biometric data, activity logs, click signatures) and generates witness values.

### 2. Circuit Compilation
Circom circuits define the zero-knowledge statement:
- "This user is a unique human" (without revealing identity)
- "This conversion is legitimate" (without revealing browsing data)
- "This achievement occurred" (without revealing health metrics)

### 3. Proof Generation
Groth16 prover generates succinct proof (~200 bytes) in <2 seconds.

### 4. On-Chain Verification
Solana smart contract verifies proof validity. Only proof hash is stored on-chain - never personal data.

## Privacy Guarantees

- **Zero-knowledge:** Verifier learns nothing except statement validity
- **Unlinkability:** Same user's proofs cannot be correlated
- **Non-interactivity:** No back-and-forth communication needed
- **Succinctness:** Proofs are ~200 bytes regardless of statement complexity

## Security Model

- Trusted setup performed via multi-party computation (MPC)
- Circuit audits by [Third-party auditor - TBD]
- Open-source implementation for community review
- Bug bounty program launching Q1 2026

## Performance Optimizations

- WASM compilation for browser-based witness generation
- GPU acceleration for high-volume proof batching
- Recursive proofs for complex multi-step verification
- Lazy verification for cost optimization

---

**More technical documentation coming Q1 2026**
