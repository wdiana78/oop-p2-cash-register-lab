# Object Oriented Programming (OOP) Part 2 - Cash Register Lab

## Overview

This project builds a `CashRegister` class to simulate basic cash register functionality for an e-commerce application.

## Features

The Cash Register can:

- Store a discount percentage.
- Track the current total.
- Track items added to the register.
- Track previous transactions.
- Add items with optional quantities.
- Apply discounts to the current total.
- Void the most recent transaction.
- Validate discount values between 0 and 100 inclusive.

## CashRegister Attributes

The `CashRegister` object contains:

- `discount` - percentage discount applied to the total.
- `total` - current total price.
- `items` - list of items currently in the register.
- `previous_transactions` - list of transactions added to the register.

## Methods

### `add_item(item, price, quantity=1)`

Adds an item to the register, updates the total, records the item for each quantity, and stores the transaction.

### `apply_discount()`

Applies the configured percentage discount to the total and displays the updated price.

If there is no discount to apply, the register displays:

`There is no discount to apply.`

### `void_last_transaction()`

Removes the most recent transaction, updates the total, and removes the corresponding items.

If there is no transaction to void, the register displays:

`There is no transaction to void.`

## Testing

The project uses `pytest`.

Run the test suite with:

```bash
pytest
```
