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
  
