
# Holiday Gift Tracker

## Problem Description

Santa has a list of gifts to deliver this holiday season, but his elves made a mistake and scrambled the list! Your task is to help Santa organize the gift deliveries by solving the following problems.

### Input

You will be given the following as **lists**:
1. A list of gifts (`gifts`) Santa needs to deliver. Example:  
   ```python
   gifts = ["doll", "car", "puzzle", "bike", "teddy"]
   ```
2. A list of naughty children (`naughty_list`) who don't deserve gifts. Example:  
   ```python
   naughty_list = ["sam", "mia"]
   ```
3. A delivery order list (`delivery_order`) that specifies the order in which gifts need to be delivered. Example:  
   ```python
   delivery_order = [3, 1, 4, 2, 0]
   ```

Additionally:
- Each gift in the `gifts` list is intended for a specific child whose name is the **same as the gift, reversed** (e.g., the gift `"doll"` is for `"llod"`).  

---

## Tasks

1. **Find the Lucky Children**  
   Determine which children on the `naughty_list` should still receive gifts because their gift matches their name reversed. Output a list of their names.  

   **Example Output**:  
   ```python
   lucky_children = ["sam"]
   ```

2. **Sort the Delivery List**  
   Use the `delivery_order` to rearrange the `gifts` list into the correct delivery sequence.  

   **Example Output**:  
   ```python
   sorted_gifts = ["bike", "car", "teddy", "puzzle", "doll"]
   ```

3. **Calculate Gift Score**  
   Santa wants to reward well-behaved children by calculating a score for each gift. The score for a gift is the **sum of the ASCII values of all characters in the gift's name**. Output a list of scores for the `sorted_gifts`.  

   **Example Output**:  
   ```python
   gift_scores = [412, 218, 513, 751, 416]
   ```

4. **Optional Stretch Goal**  
   Write a function to determine which gift has the **highest score** and output the name of the gift.  

   **Example Output**:  
   ```python
   highest_score_gift = "puzzle"
   ```

---

## Hints

- Use slicing to reverse strings (e.g., `name[::-1]`).
- The `sorted()` function or list indexing can help with reordering.
- Use the `ord()` function to calculate ASCII values of characters in a string.
- Loop through lists and use `if` conditions for filtering or matching items.

---

## Example Starter Code

```python
# Input Data
gifts = ["doll", "car", "puzzle", "bike", "teddy"]
naughty_list = ["sam", "mia"]
delivery_order = [3, 1, 4, 2, 0]

# TODO: Solve each task!
```

---

## Submission

Encourage students to:
1. Commit their code to a local Git repository.  
2. Push their solution to a GitHub repository named `holiday-gift-tracker`.
