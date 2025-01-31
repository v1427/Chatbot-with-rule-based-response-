# Chatbot-with-rule-based-response-
def rule_based_chatbot():
    print("Chatbot: Hello! I'm your rule-based chatbot. Type 'bye' to end the conversation.")
    
    while True:
        user_input = input("You: ").strip().lower()
        
        # Exit the conversation
        if user_input == "bye":
            print("Chatbot: Goodbye! Have a great day!")
            break
        
        # Rule 1: Greetings
        elif any(word in user_input for word in ["hello", "hi", "hey"]):
            print("Chatbot: Hi there! How can I help you?")
        
        # Rule 2: Ask for the chatbot's name
        elif "your name" in user_input:
            print("Chatbot: I'm RuleBot, your rule-based chatbot!")
        
        # Rule 3: Ask how the chatbot is
        elif "how are you" in user_input:
            print("Chatbot: I'm just a bot, but I'm doing great! How about you?")
        
        # Rule 4: Ask about the weather
        elif "weather" in user_input:
            print("Chatbot: I'm not connected to a weather service, but I hope it's nice where you are!")
        
        # Rule 5: Thank the chatbot
        elif "thank you" in user_input or "thanks" in user_input:
            print("Chatbot: You're welcome! Let me know if you need anything else.")
        
        # Rule 6: Default response for unknown inputs
        else:
            print("Chatbot: Sorry, I didn't understand that. Can you rephrase or ask something else?")

# Run the chatbot
rule_based_chatbot()
