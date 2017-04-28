# ChineseBot
Chinesebot
GREETING_KEYWORDS = ("hello", "hi", "greetings", "sup", "what's up",)
​
GREETING_RESPONSES = ["ni hao", "ni hao ma", "ni hao ni hao", "hello ni hao"]
​
def check_for_greeting(sentence):
    """If any of the words in the user's input was a greeting, return a greeting response"""
    for word in sentence.words:
        if word.lower() in GREETING_KEYWORDS:
            return random.choice(GREETING_RESPONSES)
​
