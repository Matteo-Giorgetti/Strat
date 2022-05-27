# Jesse Strategy Template Extended
[![Sourcery](https://img.shields.io/badge/Sourcery-enabled-brightgreen)](https://sourcery.ai)

Migrated from k3_base 0.2.4 strategysd

If self.use_initial_balance is True then
1 - the strategy will use the initial balance as the starting position
2 - calculate available margin based on the initial balance.
Don't use self.use_initial_balance and save profits together.

Update:
Added avail_margin, margin balance != avail margin.

Update:
Added liquidation price calculation.

## TODO
Average entry price mismatch.

### Installation
```bash
pip install -e .
```

### How to use
Modify Strategy import

from:
```python
from strategysd import Strategysd
```

to:

```python
from strat import Strat
```

and use the new class name

```python
class k3_base(Strategysd) -> class k3_base(Strat)
```

## License

[MIT](https://choosealicense.com/licenses/mit/)
