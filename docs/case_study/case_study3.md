# Case Study 3

The module `tool_calling.py` has 4 tools and they form pairs to test multiple tool calling in a sequence.

TOOL 1:
- get weather (fake api) gets weather for a city.

TOOL 2:
- Checks for seating availablity

These two answer the question: 'What is the temperature in Munich and are there seats indoors/outdoors available'

TOOL 3:
- Converts Centigrade to Fahrenhiet

TOOL 4:
- For a given temperature in F, gives a lable of COLD, MILD, WARM or HOT.

Tools 3 and 4 are sequential in answering the question 'What is 12C in Fahrenheit and give me the label/description of that temperature'

Of course, this could be just one tool but this is a demo of sequential tool calling and checking correct tools and arguments are used as well as giving the correct outputs.