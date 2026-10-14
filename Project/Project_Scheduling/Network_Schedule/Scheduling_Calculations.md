# Exercise 6: Network-Based Scheduling

The Task-on-Node network diagram was created using the 12 tasks,
durations, and dependencies from the WBS.

## Scheduling Calculations

### Forward Pass
- ES = Maximum EF of predecessors + 1
- EF = ES + E - 1

For T5:
ES = max(8, 13) + 1 = 14
EF = 14 + 6 - 1 = 19 days

### Backward Pass
- LF = Minimum LS of successors - 1
- LS = LF - E + 1

For T6:
LF = min(25, 28) - 1 = 24
LS = 24 - 5 + 1 = 20 days

### Slack
Slack = LS - ES

- T3: 10 - 5 = 5 days
- T8: 28 - 25 = 3 days

All other tasks have zero slack.