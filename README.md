# rtk-pnpm-typecheck-rewrite-test

This repository is designed to reproduce and demonstrate an unexpected behavior of `rtk` (Rust Token Killer) when executing the command `rtk pnpm typecheck`.
This repository will be linked in a GitHub issue of the [rtk repository](https://github.com/rtk-ai/rtk) to help maintainers investigate.

---

## Steps to Reproduce

### 1. Install `rtk`
First, make sure `rtk` is installed on your system. You can install it using Homebrew or the official install script.
For more details, please refer to the [rtk Installation Guide](https://github.com/rtk-ai/rtk#installation).

**Homebrew:**
```bash
brew install rtk
```

**Shell Script:**
```bash
curl -fsSL https://rtk.wavespeed.ai/install.sh | sh
```

---

### 2. Clone this repository
Clone this repository to your local machine and navigate into the project directory:

```bash
git clone https://github.com/tanakalucky/rtk-pnpm-typecheck-rewrite-test.git
cd rtk-pnpm-typecheck-rewrite-test
```

---

### 3. Install `pnpm` (v9)
Make sure you have `pnpm` version 9 installed. You can install it using one of the following methods:

**Using Corepack (Recommended):**
```bash
corepack enable
corepack prepare pnpm@9.x --activate
```

**Using npm:**
```bash
npm install -g pnpm@9
```

---

### 4. Install dependencies
Install the project dependencies using `pnpm`:

```bash
pnpm install
```

---

### 5. Run the reproduction command
Run `rtk pnpm typecheck` at the project root:

```bash
rtk pnpm typecheck
```

Observe the output to confirm the unexpected behavior.
