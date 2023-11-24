---
layout: default
title: Writing the Code
has_children: false
nav_order: 2
---

This section relates mostly to Python code.

## Module (*.py file)

Short & all lowercase letter, underscores can be used

```aerodynamics.py, aircraft.py, weight_balance.py```

## Class

Starts with a capital letter

```python
class CommunicationBus

class InterfaceAVL
```

## Functions and Variables

all lowercase letters, separate by underscores if necessary

- Variables are nouns ```mass, lift, aircraft```
- Functions are verbs ```get, set, plot, save, run, calc```

## Variables

All variable names are words ```separated_with_underscores```.

Constants should be in CAPS separated with underscores
```GRAVITY_ACCELERATION```.

### Variable naming convention

1. Parameter name (mass, power, thrust, etc.)
2. Parameter descriptor (motor, propeller, baggage, etc.)
3. Prefix or aggregation (min, max, avg, total)
4. [Unit other than SI](Unit-usage)

```python
mass_propulsion_total
thrust_total_lbf
thrust_avg
```

### Number of items

Use words **number of** for total number of items and **index** to
refer to a specific item. Avoid use of word **total** in this context.

- ```num_motors``` - total number of motors
- ```idx_motor``` - specific index of the motor (1st or 5th)

### Total

Use word **total** for uncountable nouns. Like ```mass_total```
