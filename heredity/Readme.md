## Heredity Probability Calculator  

### Overview  
This program calculates the likelihood that individuals in a family have a specific genetic trait based on known data and family relationships. It uses probability rules to account for inheritance and mutation.  

### How It Works  

1. **Joint Probability Calculation**  
   - Computes the probability of a specific gene-trait combination for all individuals.  
   - Uses predefined probabilities for random inheritance.  
   - Considers parental inheritance if parents are known.  
   - Applies mutation probabilities when needed.  

2. **Updating Probability Distributions**  
   - Tracks probabilities for different gene counts (0, 1, or 2).  
   - Updates probabilities for having or not having the trait.  
   - Adjusts probabilities using the computed joint probability.  

3. **Normalization of Probabilities**  
   - Ensures gene probabilities sum to 1 for each person.  
   - Ensures trait probabilities sum to 1 for each person.  
   - Keeps relative proportions unchanged while making values valid.  

### Key Concepts  
- The program models inheritance without an explicit graph structure.  
- It evaluates all possible genetic trait combinations for accuracy.  
- The final result emerges from accumulated probabilities over multiple scenarios.  
