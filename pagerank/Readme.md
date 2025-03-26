### **PageRank Implementation Overview**  

This program calculates the PageRank of web pages using two different methods: **random sampling** and **iterative convergence**. PageRank measures the importance of each page based on how often it would be visited by a random web surfer.  

---

### **What I Did**  

I implemented three key functions to make the PageRank calculation work:  

#### **1. Transition Model**  
This function determines the probability of moving from one page to another:  
- If a page has outgoing links, the user:  
  - **85% of the time** follows one of the links at random.  
  - **15% of the time** jumps to any page in the corpus randomly.  
- If a page has no links, the user jumps to any page randomly.  

#### **2. Sampling-Based PageRank**  
This method simulates a user clicking around the web:  
- Start on a random page.  
- Use the **transition model** to decide the next page.  
- Repeat this **10,000 times** and track how often each page is visited.  
- The more visits a page gets, the higher its PageRank.  

#### **3. Iterative PageRank (Mathematical Approach)**  
This method uses math instead of simulation:  
- Start with an **equal probability** for all pages.  
- Update each page’s rank based on how many other pages link to it.  
- Keep updating until ranks **stop changing significantly**.  

---

### **Key Insights**  
The **random sampling method** is an approximation that works well for large datasets.  
The **iterative method** is mathematically precise and converges to the correct values.  
The **transition model** handles both linked and unlinked pages properly.  
