# token_original_id

original_id represent contract address hash on EVM based blockchain, coin id on Cosmos SDK based blockchain or any other IDs which is able to identify tokens uniquely.
For example, ATOM can possess multiple original_ids since ATOM is available on Ethereum, Binance Smart Chain, Osmosis, etc.

## Setup

Install poetry preview version

```sh
curl -sSL https://install.python-poetry.org | python - --preview
```

Install dependencies with poetry

```sh
poetry config virtualenvs.in-project true && poetry install
```

## Linting

Run lint scripts before commit

```sh
poetry run python scripts/sort_csv.py && git diff --name-only --exit-code
poetry run python scripts/check_csv.py
```

## Testing

Run tests with pytest

```sh
poetry run pytest
```
