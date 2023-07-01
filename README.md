
# ✨ MiMC5 Circom Circuit ✨
This circuit takes two inputs, x and k and return the hash of x.

# Requirements 🔧

- [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
  - You'll know you did it right if you can run `git --version` and you see a response like `git version x.x.x`
- [Nodejs](https://nodejs.org/en/)
  - You'll know you've installed nodejs right if you can run:
    - `node --version` and get an output like: `vx.x.x`
- [Circom](https://docs.circom.io/getting-started/installation/#installing-circom)
  - You'll know you've installed nodejs right if you can run:
    - `circom --help` and get an output like: `Circom Compiler 2.x.x`
# Usage 📝
First, install packages running:
```
npm install
```
## Compile The Circuit 🔨

```
circom circuit.circom --r1cs --wasm
```

## Run The Circuit 🚀

```
node circuit_js/generate_witness.js ./circuit_js/circuit.wasm input.json
```

### Convert witness.wtns to json 📝

```
snarkjs wtns export json witness.wtns witness.json
```