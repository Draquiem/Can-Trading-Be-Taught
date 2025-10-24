# Can-Trading-Be-Taught
In this repo, I explore why trading can not be taught in the context of systematic and discretionary trading. I will provide mathematical context to support my reasonings for why this is the case while providing a better understanding of the space itself. I will also discuss what we CAN actually learn in this space.

1.) Edge: Expected Value
  - Any time we are dealing with a game or system that involves randomness, we want to know something about the income (wealth accumulation)
    - However, we don't know exactly what will happen to our wealth, this is because of uncertainty
    - This is quantified by expected value (either positive, negative, or zero sum), even if you are positive at one point in time, it does not mean you will continue to be positive
  - Notice how the short run vs long run traders have drastically different performances at the end
    - Short run does not provide enough data for us to see what wealth path the trader is on, the trader that originally started off well ended up liquidating his account
      
  Fixed Edges and Game of Chance
  - Notice that it is easier to compute if probability of the different outcome is well-defined and stable
    - Example: Roulette, P of landing on black, red, or green, does not change over time
    - There are nothing that these players can do except not transact, or go bankrupt

  Dynamic Edge and Games of Incomplete Information
  - Player action can influence edge, expected value, or EV, dictated by some sort of policy function (see machine learning literatures)
  - What should our policy function be to transact for optimal edge?
    - Blackjack stay at 16+ or stay at 20+ (not dynamic)
      
  Optimal Policies (Dynamic)
   - Martingaling Roulette
    - This is achieved by being able to control your bet size, which is why casinos DO NOT allow for this to happen
   - Counting cards in Blackjack
     - This now creates a positive edge for Blackjack, also contributes to the reason why casinos DO NOT allow for this to happen
     - Continuously optimize strategy (compare policy 1 of blackjack vs policy 2 in this context)

 2.) Learning to Play Poker and Trading
 
 - Now that we've covered optimal vs suboptimal policy function, you will have a better understanding, mathematically, of why nobody can teach you how to trade.
  - Pi* is the optimal policy function (NOT AN EASY TASK) We are unable to throw ML at to solve this issue (this is due to the need to define everything for an AI)
- Graph portrays how AI is insufficient. Although it does better than a naive strategy, it is unable to transact based on the strategy of counting cards.
  - overfitting noise, time-variable dynamics, etc..
- It will be easier for us to impose a policy on our own OR LEARN IT OURSELVES FROM EXPERIENCE, our goal is to find pi* (no set of rules around this beyond experience)
- Not something somebody can hand you, it is literally how you go about making decisions in the face of uncertainty to maximize your expected value, learn over time
    
Example: Hand of Poker (Pocket Aces)
- Game of incomplete information, thus we try to act in optimal way; if they were complete random, the Pros would not have any basis for long term wealth generating potential that transacts with positive EV
- Pi* is learned after an incredible # of hands
- It is very important to experience and understand the system that you are working with
  - How are you physically/mentally feeling? Did you lose the previous hand? Who are you playing against? Etc... All these variables MASSIVELY change how you play, even with the same system. 

Example: Trading Options (Selling a Staddle)
- Trader A sells straddle, goal is to maximize EV, we see A continuously updating his Pi* but acting optimally
  - What is the current macroeconomics? What is the current regime? How are people feeling about this company? What is the administration like? Is there more fear or greed? Etc...
- Trader B doesn't give a sh*t, and is just selling straddles in hopes of it being a good strategy; he is not vetting out this strategy 
- We must think about the space in policy function, EV, and how we are making these decisions to optimize our EV
  - THERE IS NO SYSTEM THAT INDEFINITELY PRINTS MONEY, this is a statistical impossibility

What the Pros CAN Teach You?
- Tight Bankroll
- Ergodic Theory
- No need to always transact
- Cut losses early
- Check your emotions
