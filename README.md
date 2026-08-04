<div align="center">

## Luciano Correa

**Full Stack Developer · Systems Programming · Rust Enthusiast**

<br/>

![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![Tauri](https://img.shields.io/badge/Tauri-24C8DB?style=for-the-badge&logo=tauri&logoColor=white)
![gRPC](https://img.shields.io/badge/gRPC-244C5A?style=for-the-badge&logo=trpc&logoColor=white)

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=for-the-badge&logo=nodedotjs&logoColor=white)

![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=for-the-badge&logo=cloudflare&logoColor=white)

<br/>

[💼 LinkedIn](https://www.linkedin.com/in/luccorreaa-dev/) &nbsp;·&nbsp; [📧 Email](mailto:lucianocorrea1112@gmail.com) &nbsp;·&nbsp; [🌐 Portfolio](https://luccorreaa.pages.dev)

</div>

---

### About

- Building **[anvil-zk](https://github.com/crab-forge/anvil-zk)** — distributed coordinator/worker system for zero-knowledge proof generation, in Rust
- Full stack developer at **WestDigital** — installable PWAs, React apps on server-rendered platforms, and Next.js product sites
- Interested in distributed systems, peer-to-peer networks, applied cryptography, and low-level programming
- Studying **Information Systems Engineering** @ UTN FRBA, Buenos Aires
- I take problems end-to-end — from architecture to production
- Open to collaborations and interesting engineering challenges

---

### Projects

**[mini-blockchain](https://github.com/luccorreaa/mini-blockchain)** — `Rust` `Tokio` `Axum` `libp2p`
P2P blockchain node built from scratch. Cryptographic core (SHA-256 chain linking, Ed25519 signatures,
Merkle tree, BIP-39 wallet encrypted with AES-256-GCM), a concurrent REST API, and a peer-to-peer layer
where nodes discover each other over mDNS and propagate blocks through Gossipsub. Transactions are
signed client-side — the private key never leaves the wallet.

**[anvil-zk](https://github.com/crab-forge/anvil-zk)** — `Rust` `gRPC` `NATS` `Docker`
Coordinator/worker system distributing proof generation. Every piece of infrastructure sits behind a
trait, so swapping an in-memory queue for NATS JetStream is an adapter change, not a redesign. A job's
lifecycle is an explicit state machine where invalid transitions can't be expressed — and the retry
budget is spent when proving *starts*, not when it fails, so a worker crashing in a loop can't requeue
forever.

**AI Interview Assistant** — `Tauri` `Rust` `React` `Whisper` `Claude API`
Desktop app that captures microphone and system audio in parallel, segments speech with voice activity
detection, transcribes it, and returns contextual suggestions. The window is excluded from screen
capture at the OS level, so it stays invisible while sharing your screen.

**notes-app** — `NestJS` `React` `PostgreSQL` `Prisma`
TypeScript monorepo deployed as two independent services, on PostgreSQL with the schema managed
through Prisma.

---

### How I work

I write the plan before the code, and comment the *why* rather than the *what*. I'd rather have a type
that makes the mistake impossible than a test that catches it — and when that isn't possible, I write
the test.
