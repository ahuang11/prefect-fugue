# prefect-fugue

## Welcome!

Fugue Prefect integration

## Getting Started

### Python setup

Requires an installation of Python 3.7+.

We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.

These tasks are designed to work with Prefect 2.0. For more information about how to use Prefect, please refer to the [Prefect documentation](https://orion-docs.prefect.io/).

### Installation

Install `prefect-fugue` with `pip`:

```bash
pip install prefect-fugue
```

### Write and run a flow

```python
from prefect import flow
from prefect_fugue.tasks import (
    goodbye_prefect_fugue,
    hello_prefect_fugue,
)


@flow
def example_flow():
    hello_prefect_fugue
    goodbye_prefect_fugue

example_flow()
```

## Resources

If you encounter any bugs while using `prefect-fugue`, feel free to open an issue in the [prefect-fugue](https://github.com/fugue-project/prefect-fugue) repository.

If you have any questions or issues while using `prefect-fugue`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).

## Development

If you'd like to install a version of `prefect-fugue` for development, clone the repository and perform an editable install with `pip`:

```bash
git clone https://github.com/fugue-project/prefect-fugue.git

cd prefect-fugue/

pip install -e ".[dev]"

# Install linting pre-commit hooks
pre-commit install
```
