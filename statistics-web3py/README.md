
# statistics-web3py

Get the results of the simulation-web3py project we computed the two analysis phase: *transient* and *steady state* for each experiment.

During the last phase we are interested to measure some metrics that are:

- `avg_response_time`
- `min_response_time`
- `max_response_time`
- `median_response_time`
- `number_of_user`
- `mean_error`

These metrics are printed with different kinds of plot.

## Setup

To execute the script, Python must be installed([download](https://www.python.org/downloads/)), and some external libraries must be downloaded and installed using the pip (or pip3) package manager:

```bash
pip install -r requirements.txt
```

## Usage

```python
python experiment [-t]
```

To know the allowed parameters use

```python
python main.py -h
```

## Blockchain informations

| Blokchain | Consensus mechanisms        | Interarrival time Poisson (λ) |
| :--- |:----------------------------|:--- |
| GoQuorum | instanbul, qbft, raft | 2, 1, 1/2 |
| Hyperledger Besu | QBFT, IBFT, CLIQUE | 2, 1, 1/2 |
| Polygon | IBFT, PoS | 2, 1, 1/2 |