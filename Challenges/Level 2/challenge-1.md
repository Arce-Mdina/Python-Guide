**Challenge:** Building a program where it outputs stars `*` in an entered number of rows and an entered number of stars per row.

**Skills required:** Input & output; variables; loops (for)

**Possible Solution**:
```python
# Rows of stars
print("How many rows of stars would you like?")
rows_stars = int(input(">"))

# Number of stars per row
print("How many stars per row of stars would you like?")
num_stars = int(input(">"))

# Final execution
for x in range(rows_stars):
  print("*" * num_stars)
```
