As assigned our requirement is to use semaphore to avoid  race conditions and we  also and  to incorporate our own system call which required compiling of the entire  kernel. Given below is the detailed information about the problem at hand.
  
    • Four threads are involved: an agent and three smokers. The smokers loop forever, first      waiting for ingredients, then making and smoking cigarettes. The ingredients are tobacco, paper, and matches. 

    • We assume that the agent has an infinite supply of all three ingredients,    and each smoker has an infinite supply of one of the ingredients; that is, one smoker has matches, another has paper, and the third has tobacco.

    •  The agent repeatedly chooses two different ingredients at random and makes them available to the smokers. Depending on which ingredients are chosen, the smoker with the complementary ingredient should pick up both resources and proceed. 

    • For example, if the agent puts out tobacco and paper, the smoker with the matches should pick up both ingredients, make a cigarette, and then signal the agent.
