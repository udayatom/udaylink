NLU pipeline and dialogue policy configuration are the core your assistant
![[Pasted image 20230124224145.png]]

NLU pipeline and dialogue policies are defined inside of your config.xml file
![[Pasted image 20230124224354.png]]

NLU pipeline defines the steps user messages will be passed through until a decision on what user's message is about is made.
![[Pasted image 20230124224643.png]]


Rasa comes with a number of components you can use to define your custom pipeline
![[Pasted image 20230124225256.png]]

Tokenizers - They are used to parse user inputs into separate tokens(eg: words)
![[Pasted image 20230124225354.png]]

Featurizers - They are used to exrtract features from the tokens
![[Pasted image 20230124225504.png]]

Classifiers -  Models used to assign a label to the user's input

![[Pasted image 20230124225621.png]]


Entity extracts - Used to extract important details from the user messages.

![[Pasted image 20230124225706.png]]

Training policies are techniques your assistant uses to decide on how to respond back to the user

![[Pasted image 20230124225917.png]]
Policy priority defines how assistant makes decision when multiple policies predict the next action with same accuracy.

![[Pasted image 20230125074556.png]]

Two types of policies available in Rasa

* Rule Policies
  Assistant makes the decision on how to respond based on rules defined inside of your rules.yml file.
  
* Machine learning policies
  Assistant makes the decision on how to respond by learning from the data defined inside of the stories.yml file.
  
**Rule policy**
Rule policy is the policy that allows you to impose a strict rule-based behaviour on your assistant.	
  ![[Pasted image 20230125075049.png]]
Rule policy is the policy that allows your to impose a strict rule-based behaviour on your assistant.
![[Pasted image 20230125075156.png]]

**Memoization policy**
Memoization policy remembers the stories from your stories.yml file.
![[Pasted image 20230125075440.png]]

**TED Policy**
The transformer Embedding Dialogue(TED) policy is a multi-taks architecture for next action prediction and entity recognition.

![[Pasted image 20230125075546.png]] 

Max History parameter defines how many conversational steps your assistant keeps in the memory when making the prediction
![[Pasted image 20230125075817.png]]

 * Can be configured inside of the config.yml file
 * In order to handle more complicated conversations your will likely need to set this parameter to a higher number
 * Higher max_history parameters means bigger model which will take longer to train.
 