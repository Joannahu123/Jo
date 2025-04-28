---
layout: post
title: Simulation/Games and Random Algorithms Submission
hide: false
---



<h2>Popcorn Hack 1</h2>
<p><strong>Name two real-world applications where random number generation is essential and briefly explain why:</strong></p>

<ul>
  <li><strong>Video Games:</strong> Usernames can be randomly generated for users who don’t want to make their own username. Randomly generated numbers can also be stored in a database and referred to more easily.</li>
  <li><strong>YouTube:</strong> Random video generation on the Explore page helps show users a variety of videos they might not have searched for, keeping the experience fresh and engaging.</li>
</ul>

<hr>

<h2>Popcorn Hack 2</h2>

<pre><code>import random

def magic_8_ball():
    rand_num = random.random()  # generates a number between 0.0 and 1.0
    if rand_num &lt; 0.5:
        return "Yes"
    elif rand_num &lt; 0.75:
        return "No"
    else:
        return "Ask again later"

# Test your function
for i in range(10):
    print(f"Magic 8-Ball says: {magic_8_ball()}")
</code></pre>

<hr>

<h2>Popcorn Hack 3</h2>

<pre><code># Traffic light simulation (no randomness)

states = ["Green", "Yellow", "Red"]
durations = {"Green": 5, "Yellow": 2, "Red": 4}
timeline = []

# Simulate 20 time steps
time = 0
state = "Green"
counter = 0

while time &lt; 20:
    timeline.append((time, state))
    counter += 1
    if counter == durations[state]:
        counter = 0
        current_index = states.index(state)
        state = states[(current_index + 1) % len(states)]
    time += 1

for t, s in timeline:
    print(f"Time {t}: {s}")
</code></pre>

<h3>Short Answer:</h3>
<p>This is a simulation because it models the real-world behavior of a traffic light over time without physically building one. Simulations like this can help city planners test traffic patterns and optimize light timings to reduce traffic congestion and accidents.</p>




<br>

<h1>Homework Hack 1: Create a Simple Dice Game (Randomness AND Simulation)</h1>

<h2>Dice Game Features:</h2>
<ul>
  <li>Player rolls two dice.</li>
  <li>If the sum is 7 or 11, the player wins immediately.</li>
  <li>If the sum is 2, 3, or 12, the player loses immediately.</li>
  <li>If the sum is any other number, that becomes the “point.”</li>
  <li>Player continues to roll until they either roll the point again (win) or roll a 7 (lose).</li>
  <li>Track win/loss statistics.</li>
</ul>

<hr>

<h2>Completed Dice Game Code:</h2>

<pre><code>import random

def roll_dice():
    """Roll two dice and return their values and sum."""
    die1 = random.randint(1, 6)
    die2 = random.randint(1, 6)
    dice_sum = die1 + die2
    print(f"You rolled a {die1} and a {die2} (Sum: {dice_sum})")
    return dice_sum

def play_dice_game():
    """
    Play one round of the dice game.
    Returns True if player wins, False if player loses.
    """
    sum_dice = roll_dice()

    # Immediate win
    if sum_dice in [7, 11]:
        print("You win!")
        return True
    # Immediate loss
    elif sum_dice in [2, 3, 12]:
        print("You lose!")
        return False
    else:
        # Establish point
        point = sum_dice
        print(f"Your point is now {point}. Keep rolling!")

        while True:
            sum_dice = roll_dice()
            if sum_dice == point:
                print("You hit your point! You win!")
                return True
            elif sum_dice == 7:
                print("You rolled a 7. You lose!")
                return False

def main():
    """Main game function with game loop and statistics."""
    wins = 0
    losses = 0

    while True:
        play = input("Do you want to play a round? (yes/no): ").strip().lower()
        if play == "yes":
            if play_dice_game():
                wins += 1
            else:
                losses += 1
        elif play == "no":
            break
        else:
            print("Please enter 'yes' or 'no'.")

    print("\nGame Over!")
    print(f"Total Wins: {wins}")
    print(f"Total Losses: {losses}")

if __name__ == "__main__":
    print("Welcome to the Dice Game!")
    main()
</code></pre>

<hr>