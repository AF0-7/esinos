# esinos

A simulated operating system kernel written in Python (university OS project).
Everything runs in user space; nothing touches the real hardware.

## Features

1. **CPU scheduler**: FCFS, SJF (non-preemptive), Round Robin (user-chosen quantum),
   Priority (non-preemptive). Text Gantt chart, per-process waiting and
   turnaround times, and averages.
2. **Memory manager**: paging, logical-to-physical address translation, page faults,
   page replacement (FIFO, LRU, Optimal) shown step by step, TLB and effective
   access time (EAT).
3. **Mini file system (bonus)**: inode-based.
4. **Integrated menu** to reach every module.

## Requirements

- Python 3.8 or newer
- Standard library only (no `pip install` needed)
- Runs on Linux, macOS and Windows

## How to run

```bash
cd code
python3 main.py        # on Windows: py main.py
```

## Input format

### Process file (scheduler)

One process per line: `pid arrival burst priority`
(a lower priority number means a higher priority). Blank lines and lines
starting with `#` are ignored.

```
# pid arrival burst priority
1 0 5 2
2 1 3 1
```

See `tests/processes_example.txt`.

### Page reference string (page replacement)

_TODO: to be defined._

## Team

_TODO_
