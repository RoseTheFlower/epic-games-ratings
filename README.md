# Epic Games Ratings

This repository contains Python code to data-mine ratings at the Epic Games Store (EGS).

## Requirements

-   Install the latest version of [Python 3.X][python-download-url].
-   Install the required packages:

```bash
pip install -r requirements.txt
```

## Usage

To retrieve the `pageSlug` for every store product, run:
```bash
python download_store_products.py
```
Caveat: different store products can be associated with the same `pageSlug`, despite having different `title` values.

To retrieve the `sandboxId` associated with every `pageSlug`, run:
```bash
python download_sandbox_ids.py
```

To retrieve the ratings associated with every `sandboxId`, run:
```bash
python download_game_ratings.py
```

Alternatively:

-   Run [`epic-games-ratings.ipynb`][colab-notebook]
[![Open In Colab][colab-badge]][colab-notebook]


## References

- [`nikop/epic-games-ratings`][madjoki-egs-ratings]
- [`ToutinRoger/EpicGraphQL`][egs-api-graphql]

<!-- Definitions -->

[madjoki-egs-ratings]: <https://github.com/nikop/epic-games-ratings>
[egs-api-graphql]: <https://github.com/ToutinRoger/EpicGraphQL>
[colab-notebook]: <https://colab.research.google.com/github/woctezuma/epic-games-ratings/blob/colab/epic-games-ratings.ipynb>
[colab-badge]: <https://colab.research.google.com/assets/colab-badge.svg>

