Responses are simple messages that your assistant can send back to your users.
![[Pasted image 20230123081324.png]]

Response templates are defined in the domain.yml file.
![[Pasted image 20230123081533.png]]

Creating multiple responses
Your can include more than one possible response for a specific template. Rasa will the randomly select which response to pick.
![[Pasted image 20230123081740.png]]

**Using variables**

You can create more dynamic responses by including slots in the responses.
![[Pasted image 20230123082035.png]]


![[Pasted image 20230123082317.png]]

![[Pasted image 20230123082543.png]]


Adding buttons
	You can enrich your assistant's responses by including buttons for specific options. You can configure the text that is visible on the buttons as well as the payload that is being sent to Rasa after a specific button is pressed.
	
	Buttons can send the entities to the Rasa assistant backend.
	


![[Pasted image 20230124180659.png]]

Custom Payload

If you prefer, you can get your assistant to send a custom payload to your frontend.

![[Pasted image 20230124223453.png]]

Channel specific responses
	You can define responses that will be sent to a specific output channel
![[Pasted image 20230124223700.png]]

Training your assistant to use the responses
	To enable your assistant to actually use the defined responses, you have to include them into your training stories.
	 
	![[Pasted image 20230124223802.png]]