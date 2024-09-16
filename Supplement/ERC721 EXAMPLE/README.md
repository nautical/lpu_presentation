##### Rinkeby deployment
- [Python](https://www.python.org/downloads/)
- Brownie
```
python3 -m pip install --user pipx
python3 -m pipx ensurepath
# restart terminal
pipx install eth-brownie
```
- A free [Infura](https://infura.io/) Project Id key for Rinkeby Network

### Deploy to Rinkeby

- Add a `.env` file with the same contents of `.env.example`, but replaced with your variables.

- In `scripts/deploy.py` change the value of `NAME`, `SYMBOL`, `COST`, `MAX_SUPPLY` and `MAX_MINT_AMOUNT_PER_TX` to custom ones for your Collection.

- Run the command:
```
brownie run scripts/deploy.py --network rinkeby
```
