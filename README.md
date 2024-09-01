This code defines a class wich is a Knowledge Space. A Knowledge Space is a pair (K,Q) where Q is a set of items and K is a set of subsets of Q which contains 
the empty set and Q. 

The class knowledge_learning_space is instanced which the required arguments Q, K_mathcal and Xi, the last argument gives the learning rate of the algorithm.

The nonrequired arguments are beta_q which gives the probability of fail for an understood item, prob_distribution which is the initial probability of 
each state of knowledge, K0 is the real state of knowledge of the student (K0 is required if we use the code for simulating), student_name.

The class has three methods: simulation simulates that the student response to one item and the results depends on K0, response_item takes as argument 0 or 1
depends that the student fails or not the item.

The attribute of the class are the following: 
Q: the set of items
K_mathcal: the set of states of knowledge
K0: the true state of knowledge of the student
beta_q: a dictionary which keys are the items in K0 and the values are the probability to fail to the corresponding items.


prob_distribution: the probability of each state of knowledge to be the true state of knowledge.
prob_distribution_items: the probability of each item to be in the true state of knowledge.
responded_items: dictionary which keys are the responded items and value is the list of associated results.
next_item: the next item that the student will responde. It corresponds to one of the items which probability is closest to 1/2.
