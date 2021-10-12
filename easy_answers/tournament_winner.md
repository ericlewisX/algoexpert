## Tournament Winner
There's an algorithms tournament taking place in which teams of programmers compete against each other to solve algorithmic
problems as fast as possible. 


Sample Input
```python
competitions = [
  ["HTML", "C#"],
  ["C#", "Python"],
  ["Python", "HTML"],
]
results = [0, 0, 1]
```

Sample Output
```python
"Python"
// C# beats HTML, Python Beats C#, and Python Beats HTML.
// HTML - 0 points
// C# - 3 points
// Python - 6 points
```
 
## Hints
<details>
  <summary>Hint 1</summary>
  Don't overcomplicate this problem. How would you solve it by hand? Consider that approach, and try to translate it 
  into code.
</details>

<details>
  <summary>Hint 2</summary>
  Use a hash table to store the total points collected by each team, with the team names as keys in the hash table. Once you know how many
  points each team has, how can you determine which one is the winner?
</details>

<details>
  <summary>Hint 3</summary>
  Loop through all of the competitions, and update the hash table at every iteration. For each competition, consider the name of the winning team;
  if the name already exists in the hash table, update that entry by adding 3 points to it. If the team name doesn't exist in the hash table, add a new
  entry in the hash table with the key as the team name and the value as 3 (since the team won its first competition). While looping through all of the
  competitions, keep track of the team with the highest score, and at the end of the algorithm, return the team with the highest score.
</details>

<details>
  <summary>Optimal Space & Time Complexity</summary>
  O(n) time | O(k) space - where n is the number of competitions and k is the number of teams
</details>
