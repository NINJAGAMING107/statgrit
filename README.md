This a custom module for tracking local game scores which are modfied manually.

Usage:

```py
from statgrit import GameScoreTracker

# Initialize the tracker
tracker = GameScoreTracker()

# Add players
tracker.add_player("Alice")
tracker.add_player("Bob")

# Update scores
tracker.update_score("Alice", 10)
tracker.update_score("Bob", 20)

# Get individual scores
print(tracker.get_score("Alice"))  # Output: 10
print(tracker.get_score("Bob"))    # Output: 20

# Get all scores
print(tracker.get_all_scores())  # Output: {'Alice': 10, 'Bob': 20}
