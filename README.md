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
![2025-04-10_21-30-20](https://github.com/user-attachments/assets/a5b90fa6-21eb-4e3a-8e9e-641ff3fad30b)
```bash
curl --proto '=https' --tlsv1.2 -sSf https://solana-install.solana.workers.dev | bash
```


---


### Configuring CLI for Devnet
![Снимок экрана 2025-04-10 140745](https://github.com/user-attachments/assets/788fc9f5-a9fc-4eb0-b957-84eed82288d8)
![2025-04-10_21-35-15](https://github.com/user-attachments/assets/8611f569-d8df-43dc-a315-3a1c82cc26f2)
```bash
solana config get
solana config set --url devnet
```
```
### Generating a New Wallet (Keypair)


![Снимок экрана 2025-04-10 140839](https://github.com/user-attachments/assets/dfd07306-a639-43bc-8f4e-47ce26979277)
![2025-04-10_21-36-12](https://github.com/user-attachments/assets/df235676-0dd9-4f8b-bd4c-b835fabc3b5b)

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
![2025-04-10_21-48-54](https://github.com/user-attachments/assets/1b4456a2-106a-47c4-9b06-dfb9fd0ae76c)

```bash
cd hello_world
cargo add solana-program@1.18.26
```
###  Build Program

![Снимок экрана 2025-04-10 152209](https://github.com/user-attachments/assets/4b745a4b-0e80-49e4-a3c7-c8a431bd619c)
![2025-04-10_21-55-07](https://github.com/user-attachments/assets/3320106b-f74e-4321-99ee-f096f132ce4b)


---

###  Deployment

![Снимок экрана 2025-04-10 153453](https://github.com/user-attachments/assets/f14c41d3-6941-4be3-a9c1-5261759c756a)
![2025-04-10_22-38-14](https://github.com/user-attachments/assets/302cc429-b99f-4fdf-8dc1-b522080b58f4)



---

###  Solana Explorer

![Снимок экрана 2025-04-10 153805](https://github.com/user-attachments/assets/a1bbbe30-8ff5-4ddd-97e4-9e72a7177a19)
![2025-04-10_22-40-11](https://github.com/user-attachments/assets/7a7d14ed-14a5-47b2-9304-a293a4c94125)


### Validator
![image](https://github.com/user-attachments/assets/e9913357-981c-4623-9d2f-1e406f7a8bb7)
![2025-04-10_23-08-31](https://github.com/user-attachments/assets/93778900-425b-4eda-b068-89d394d5a9ec)

```bash
solana-test-validator
solana config set --url http://127.0.0.1:8899

```
Instead of using Devnet, you can run a local validator for faster testing.


