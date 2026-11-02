*This project has been created as part of the 42 curriculum by scamlett.*

# Python Module 03: Game Data

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?logo=python&logoColor=white)
![42](https://img.shields.io/badge/42-Málaga-000000)

## Description

This module is about Python's built-in collections and the different ways to
feed data into a program. Each exercise is a piece of a video game backend:
command-line arguments, player scores, 3D coordinates, achievements, an
inventory and a live stream of game events.

| Exercise | File | Topic |
|----------|------|-------|
| ex0 | `ft_command_quest.py` | Reading command-line arguments with `sys.argv` |
| ex1 | `ft_score_analytics.py` | Turning arguments into a list of scores and computing stats |
| ex2 | `ft_coordinate_system.py` | Tuples for `(x, y, z)` and distances with `math` |
| ex3 | `ft_achievement_tracker.py` | Sets: union, intersection and difference of achievements |
| ex4 | `ft_inventory_system.py` | Dicts built from `item:quantity` arguments, with `max()`/`min()` by value |
| ex5 | `ft_data_stream.py` | Generators: an infinite stream of random events consumed with `yield` |
| ex6 | `ft_data_alchemist.py` | List and dict comprehensions to transform and filter data |

## Instructions

Most exercises take their input from the command line:

```bash
python3 ex0/ft_command_quest.py hello world 42
python3 ex4/ft_inventory_system.py sword:1 potion:5 shield:2
python3 ex5/ft_data_stream.py
```

`ft_coordinate_system.py` asks for coordinates interactively in the form
`x,y,z`.

## What I learned

- `sys.argv` holds the program name at index 0 and the arguments after it
- When to pick a list, a tuple, a set or a dict, and what each one is good at
- Set operations make "what do these players have in common?" a one-liner
- `max(d, key=lambda k: d[k])` finds the key with the biggest value
- Generators produce values lazily with `yield`, so a stream can be infinite
  without filling up memory
- Comprehensions build a new list or dict from an old one, optionally with
  a filter
