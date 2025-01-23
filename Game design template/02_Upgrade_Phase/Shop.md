# #Shop 

Period during which the game is paused, allowing the purchase of #Cards. It appears once a #Waves is finished. Cards can be bought or upgraded using #DeliriumCoins , not spending coins, save them for the next stores.


When the store time is established, three #Cards card options (1) are offered for purchase, with the possibility of rerolling (2) the pool of cards presented. The #Reroll  also individually changes the #Rarity of each card and costs #DeliriumCoins. Once drawn, a card goes to your hand (3) and remains visually present on the screen. Cards in your hand can be sold and upgraded(4). Buy and/or sell movements can be triggers used on cards to enhance adverse effects, for example: when selling a card, increase its damage by 10%. The main methodology for creating cards is based on improving choice making in 20MTD (5) and maintains dynamism and simplicity (6). To close the store you need to press a skip button. It is possible to purchase upgrades, including purchasing upgrades from the pool of three cards or directly upgrading the cards in your hand (this action being considerably more expensive)

apertar um botão de skip. É possível comprar upgrades, incluindo comprar upgrades no pool das três cartas ou diretamente upar as cartas na mão (esta ação sendo consideravelmente mais cara)

### 1. Card Options for Purchase

#### Card Selection
- Upon entering the shop, three cards are offered for purchase.
- The player can choose to buy none, some, or all of the cards, depending on their availability of #DeliriumCoins.

#### Card Rarity
- Cards are categorized into three #Rarity: Common, Rare, and Epic.
- When generating a card, the system prioritizes cards that the player does not currently own to allow for the purchase of upgrades, which is more economical than upgrading directly.

#### Rarity Calculation
- The rarity of a card is determined by the following formula:  
  **Chance = (Base Chance per Level × (Current Level − Minimum Level) × (1 + Luck))**

#### Luck
- #Luck is a game attribute #Stats that influences the formula above.

#### Rarity Check Order
1. First, the system checks if the card will be Epic.
2. If not Epic, it checks if the card will be Rare.
3. If not Rare, the card will be Common.
4. The chance for each rarity cannot exceed its maximum value.

#### Rarity Chances Table(Example: might change INGAME)

| Rarity  | Available from Level | Minimum Level | Base Chance | +Chance per Level | Max Chance |
|---------|-----------------------|---------------|-------------|-------------------|------------|
| Common  | 1                     | 1             | 100%        | 0%                | 100%       |
| Rare    | 2                     | 1             | 0%          | 5%                | 60%        |
| Epic    | 4                     | 3             | 0%          | 2%                | 25%        |
### Example lvl 16 with 0 luck

| Level | 1    | 2    | 3    | 4     | 5     | 6     | 7     | 8     | 9     | 10    | 11    | 12    | 13    | 14    | 15     | 16     |
|-------|-------|-------|-------|-------|-------|-------|-------|-------|-------|-------|-------|-------|-------|--------|--------|
| C     | 100%  | 95%   | 90%   | 83,3% | 76,8% | 70,5% | 64,4% | 58,5% | 52,8% | 47,3% | 42%   | 36,9% | 32%   | 27,3% | 22,8%  | 18,75% |
| R     | 0     | 5%    | 10%   | 14,7% | 19,2% | 23,5% | 27,6% | 31,5% | 35,2% | 38,7% | 42%   | 45,1% | 48%   | 50,7% | 53,2%  | 56,25% |
| E     | 0     | 0     | 0     | 2%    | 4%    | 6%    | 8%    | 10%   | 12%   | 14%   | 16%   | 18%   | 20%   | 22%   | 24%    | 25%    |


### 2. #Reroll

#### Function:
- Allows the player to reroll cards, resetting the chances of obtaining rare cards.

#### Reroll Cost:
- The cost of a reroll is calculated as:  
  **Reroll Cost = (1 + Number of Rerolls)**  Starts on 1 every shop
  - The minimum cost for a reroll is 3 units.  
  - The cost is always rounded to the nearest integer.

#### Price Increment:
- Each time a reroll is performed, the cost of the next reroll increases by 1 unit.

---

### 3. Hand/Deck

#### Visualization:
- The hand, representing the player's #Deck, is always visible when accessing options or entering the shop.  
- All cards in the hand are visible, providing a complete view of the deck at any moment.

#### Interaction and Limits:
- The hand is limited to a maximum #HandSize #Stats
- The player can interact with cards directly, clicking and dragging to perform actions.  

#### Options for Selling or Upgrading Cards:
- Dragging the card to a specific field for selling or upgrading.  
- Clicking on the card, which opens a menu with options for selling and upgrading (similar to the game "Balatro").  

#### Trigger Effects:
- Cards with trigger effects in the shop (e.g., effects activated upon selling) will display visual animations (VFX) to signal these events.  
- These animations highlight when a card activates another effect, providing clear visual feedback to the player.

#### Interaction Flow:
- Players can drag cards to fields for selling or upgrading, simplifying #Deck management.  
- Alternatively, clicking on a card opens a contextual menu with sell and upgrade options, ensuring intuitive and efficient interaction.

---

### 4. Purchases/Upgrades/Selling

#### Purchases:
- **Common Cards**: Cost ranges from 1-5 #DeliriumCoins.  
- **Rare Cards**: Cost ranges from 3-7 #DeliriumCoins.  
- **Epic Cards**: Cost ranges from 6-10 #DeliriumCoins.  
- Each card has preset values within these ranges.

#### Upgrades:
-Upgrading a card just pay the difference between the rarity costs.
- **Common Cards**: Upgrade costs **+2** from the initial card value (value of the rare version).  
- **Rare Cards**: Upgrade costs **+3** from the initial card value (value of the epic version).  

#### Selling:
- **Sell Cost Formula**:  
  **sell_cost = floor(buy_cost / 2)**  
  - Rounded down to the nearest integer.  
  - Minimum sell cost is 1 #DeliriumCoin. 
