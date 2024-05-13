
# Hampter Pyth Tools

Tooling to pull Pyth's Market data programatically. 


## Why?

Pyth is great, but the ability to programmitcally pull which market IDs are availible is not availible through Hermes.

This tool will output a json file of all the market data+ids to the place you execute it.

This was built from a modified example in the Pyth SDK:  
[PYTH-GITHUB](https://github.com/pyth-network/pyth-sdk-rs/blob/main/pyth-sdk-solana/examples/get_accounts.rs)


## HOW 2 RUN

#### Linux

```
git clone https://github.com/HampterFi/hampter_pyth_tools.git
cd hampter_pyth_tools
chmod +x .\get_accounts
get_accounts -- https://api.mainnet-beta.solana.com <-- (Replace this with a custom RPC, will be slow without it)
```

#### Windows

In a CMD run:
```
git clone https://github.com/HampterFi/hampter_pyth_tools.git
cd hampter_pyth_tools
get_accounts.exe -- https://api.mainnet-beta.solana.com <-- (Replace this with a custom RPC, will be slow without it)
```

## Tips
Pyth Feed IDs on EVM are just the Solana Base58 IDs with Hex encoding. (Great Use of Encoding Pyth Team!)

This means you can easily convert the output of the market IDs into whatever chain you need to use them in. 
