	# rule  bases AI python chatbot
import datetime
import time

name= input(" sogut h, enter your name:")
presenthour= datetime. datetime.now().hour

if 5<=presenthour<=11:
	print("good morning",name)
elif 11<=presenthour<=17:
	print("good afternoon",)
elif 17<=presenthour<=20:
	print("good evening",name)
else:
	print("good night",name)

print (" namasta! wlecome to your chatbot")
print(" you can ask me basic question, 'type' to exit from the bot")

#chatbot memory chatbot [ dictionary]
responses = {
    "hello": "Hi, welcome. How can I help you?",
    "how are you": "i am very fine. thank you",
    "who are you": "I am smart AI chatbot",
    "motivate me": "Keep going. Every bug makes you better",
    "happy": "Great to hear that",
    "functions kya hote hai": "Function ek block of code hota hai"

}
# method/function to get responed of  chatbot 

def getresponsebot(userquestion):
	userQuestion= userquestion.lower()
	for eachkey in responses:
		if eachkey in userquestion:
			return responses[eachkey]

	return "i am not able to tall that yeet.mea jald hi yee  shik lung gea"

			
# take user input



while True:
	userInput= input("please ask your question")
	reply= getresponsebot(userInput)
	print(" bot responed:",reply)

	if "byy" in userInput.lower():
			breakpoint


 