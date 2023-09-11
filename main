# Hack's Loot Roll Simulator
# RUN to drop an item and roll to win!
from random import randint as r
import time
print("\n\n\n           Hack's Loot Roller\n           v1.0.c.2023")

# d = random.randint(1,50)
# d = r(1,50)
# Loot Rarity = random.randint(1,100)

## LOOT RARITY
# Default Drop Rates
# Rare = 30% (RareCheck3), Epic = 20% (RareCheck2), Legendary = 10% (RareCheck)
# If else = Common
RareCheck = 90
RareCheck2 = 70
RareCheck3 = 40

## Inventory Tracker
Legends: int = 0
Epics: int = 0
Rares: int = 0
Commons: int = 0

## Timer Delay
# time.sleep is measured in seconds for every character in string pass_time
# pass_time 7 Characters
def pass_time():
    pass_time = '       '
    for char in pass_time:
        print(char, end='')
        time.sleep(.1)

## Main Loop
Loop = 'z'
while Loop != 'y':
    print("<==={=======================-\n")
# quality type random 1-100
    Quality = r(1, 100)
# Rarity Check
    if Quality > RareCheck:
        print(' A LEGENDARY ITEM HAS DROPPED!')
        loot = 'legendary item!'
    elif Quality > RareCheck2:
        print(' An EPIC item has dropped!')
        loot = 'epic item!'
    elif Quality > RareCheck3:
        print('A rare item has dropped.')
        loot = 'rare item.'
    else:
        print(' A common item has dropped.')
        loot = 'common item.'

#user input
    input('\n       Press Enter to roll your dice.')
    print('\nYou roll two dice....')
    pass_time()

# Dice Rolls
    # User Roll 1
    d1 = r(1, 50)
    # User Roll 2
    d2 = r(1, 50)
    a = d1 + d2
    if a == 2:
        print('     You roll is 2 ... NANI!?')
    else:
        print("    You roll", a, "\n")
    input('       Press Enter for your opponents turn.')
    print('\nYour opponent now rolls their dice....')
    pass_time()

# Bot Roll 1
    d3 = r(1, 50)
# Bot Roll 2
    d4 = r(1, 50)
    b = d3 + d4
    if a == 2:
        print('Omae wa mou shindeiru.')
        print('Your opponent rolls ', b, '\n')
    else:
        print('Your opponent rolls ', b, '\n')
    print('               ', a, '-', b, '\n')
    pass_time()

## Results
    # Draw
    if a == b:
        print('Draw!\n')

    # Win
    elif a > b:
        if loot == 'legendary item!':
            Legends += 1
        if loot == 'epic item!':
            Epics += 1
        if loot == 'rare item.':
            Rares += 1
        if loot == 'common item.':
            Commons += 1
        print('You won the', loot, '\n')
    # Lose
    elif a < b:
        print('Your opponent won the', loot, '\n')

## End
# Loop breaks if user returns "y"
# Loop continues if "y" is not returned
# Inventory

    print('_______________________________________')
    print('_______________INVENTORY_______________')
    print('Legendary:', Legends, 'Epic:', Epics, 'Rare:', Rares, 'Common:', Commons)
    print('\n       Enter \"y\" to Quit!')
    print('     Press Enter to continue.\n')
    Loop = input()
