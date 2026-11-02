# Statistics — Homeworks

Ludovico Toto · MSc Cybersecurity, Sapienza University of Rome · 2026/2027

| Homework | Page |
|---|---|
| HMWK 1 — Exercise 1: Private key → public key with elliptic-curve scalar multiplication | https://lurbik.github.io/statistics/hmwk1.html |
| HMWK 1 — Exercise 2: From wallet seed to Ethereum address | https://lurbik.github.io/statistics/hmwk2.html |
| HMWK 2 — ECC, Caesar cipher and cryptanalysis | https://lurbik.github.io/statistics/Vero_HMWK2.html |
| HMWK 3 — Penetration scores: LLN, variance scaling and CLT with n systems and m attackers | https://lurbik.github.io/statistics/HMWK3.html |
| HMWK 4 — Welford's recurrences and sampling mean & variance (overview of Ex. 1 and Ex. 2) | https://lurbik.github.io/statistics/HMWK4.html |

## Files
- `hmwk1.html` — HMWK 1, exercise 1. Toy curve y² = x³ + 7 (mod 17): point addition, scalar multiplication Q = kG (repeated addition and double-and-add), step-by-step canvas visualisation, statistical exploration and discussion. Plain HTML/CSS/JavaScript, no libraries.
- `hmwk2.html` — HMWK 1, exercise 2. Ethereum wallet pipeline (BIP-39 → BIP-32/44 → secp256k1 → Keccak-256 → EIP-55) computed live in the browser with ethers.js, statistical tests on the hash-based steps, historical context. Links back to the relevant sections of exercise 1.
- `metamask.png` — screenshot used in HMWK 1 exercise 2, section 9 (test mnemonic imported in MetaMask).
- `Vero_HMWK2.html` — HMWK 2. One message encrypted with didactic EC ElGamal on secp256k1 and with the Caesar cipher; frequency-based (chi-squared) cryptanalysis of Caesar, empirical evaluation across ciphertext lengths, attack on a restricted ECC key space, structural comparison and self-tests. Plain HTML/CSS/JavaScript, no libraries.
- `HMWK3.html` — HMWK 3. Monte Carlo simulation of Bernoulli and Rademacher penetration scores for n systems and m attackers: distributions of Sₙ, Sₙ/n and Sₙ/√n, LLN, variance under the three normalizations, CLT, aggregate score and effect of m, self-tests and CSV export. Plain HTML/CSS/JavaScript, no libraries, synthetic data only.
- `HMWK4.html` — HMWK 4 overview page linking the two exercises.
- `HMWK4_ex1.html` — HMWK 4, exercise 1. Derivation of Welford's recurrences for the sum of squares and the variance from Knuth's update of the mean, three-line implementation, interactive step-by-step trace and a numerical-stability comparison with the textbook formula.
- `HMWK4_ex2.html` — HMWK 4, exercise 2. m hackers × n systems with scores in [0, 10] from a chosen distribution; per-hacker sampling mean and variance computed with Welford, averages compared with μ and σ², variability versus n, confidence-interval coverage, self-tests and CSV export.

All wallet examples use the public test mnemonic `test test … junk`; no real wallet is involved. All other data is synthetic and generated in the browser.
