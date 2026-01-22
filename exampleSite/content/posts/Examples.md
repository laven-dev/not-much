+++
title = 'Examples'
date = 2026-01-19T13:50:33+10:30
lastmod = 2026-01-21T09:30:00+10:30
draft = false
summary = 'Showing off cool stuff'
+++

This is a list of things you can do with this theme.

```python
test = "this is a python code block"
for i in test:
    gluntch = i
```

**This is a code block with specific lines highlighted**
{{< highlight python "hl_lines=12-13">}}
#!/usr/bin/env python3


import sys
with open(sys.argv[1] if len(sys.argv) > 1 else "input.txt") as f:
    data = f.read().splitlines()

data = [x.split() for x in data]
left = sorted([int(x[0]) for x in data])
right = sorted([int(x[1]) for x in data])

diff = 0
for (l, r) in zip(left, right):
    diff += abs(l - r)

print(f"Silver: {diff}")

sim = 0
for l in left:
    sim += (l * right.count(l))

print(f"Gold: {sim}")

{{< /highlight >}}

[This is an external link](https://github.com/laven-dev "Git")

{{< notice "Notice" >}}
This is a notice block.
{{< notice "success" >}}
These can be nested.
```python
str = "Code blocks can also be used in a notice."
```
{{< /notice >}}
{{< /notice >}}