#  Solana Hello World Deployment – Assignment 2 (Blockchain Technologies 2)
Tapen Tomiris SE-2316 , Ayaulym Kenzhekul SE-2314
##  Setup Instructions

This project demonstrates setting up the Solana CLI, compiling a smart contract in Rust, and deploying it to the **Devnet**.

### Clone the repository 
```bash
git clone https://github.com/tomiristapen/assignment2_bt2.git
cd assignment2_bt2
```

---
### Solana CLI Installation


![Снимок экрана 2025-04-10 134633](https://github.com/user-attachments/assets/daeb3c3a-ea91-4dc6-8ca7-21b8f64c2ea8)
```bash
curl --proto '=https' --tlsv1.2 -sSf https://solana-install.solana.workers.dev | bash
```
---


### Configuring CLI for Devnet
![Снимок экрана 2025-04-10 140745](https://github.com/user-attachments/assets/788fc9f5-a9fc-4eb0-b957-84eed82288d8)
```bash
solana config get
solana config set --url devnet
```
### Generating a New Wallet (Keypair)


![Снимок экрана 2025-04-10 140839](https://github.com/user-attachments/assets/dfd07306-a639-43bc-8f4e-47ce26979277)
- Wallet creation & address
- Airdrop & balance check

```bash
  solana-keygen new
  solana config set --url devnet
  solana address
  solana balance
  solana airdrop 2
```
---
###  Implementing the core of a Solana program using Rust
![Снимок экрана 2025-04-10 143238](https://github.com/user-attachments/assets/eec7e1a7-c646-476e-9fd3-5f6fb50687ed)

```bash
cd hello_world
cargo add solana-program@1.18.26
```
###  Build Program

![Снимок экрана 2025-04-10 152209](https://github.com/user-attachments/assets/4b745a4b-0e80-49e4-a3c7-c8a431bd619c)


---

###  Deployment

![Снимок экрана 2025-04-10 153453](https://github.com/user-attachments/assets/f14c41d3-6941-4be3-a9c1-5261759c756a)


---

###  Solana Explorer

![Снимок экрана 2025-04-10 153805](https://github.com/user-attachments/assets/a1bbbe30-8ff5-4ddd-97e4-9e72a7177a19)


