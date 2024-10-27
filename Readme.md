


# Chef GPT: Intelligent Culinary Assistant
## Prerequisites

- **Python 3.x** installed on your system.
- An **OpenAI API key**.  
  (Set your API key as an environment variable: `OPENAI_API_KEY`.
   from https://platform.openai.com/api-keys )


## Overview

Chef GPT is a conversational AI designed to assist users with culinary tasks. It can suggest dishes based on ingredients, provide detailed recipes for requested dishes, and critique user attempts at cooking with constructive feedback. This project uses the OpenAI API to simulate real-time chef interactions across different scenarios, making it a versatile cooking assistant.

## Features

- **Ingredient-Based Dish Suggestions:**  
  Users provide a list of ingredients, and the AI suggests possible dish names without full recipes.

- **Recipe Requests:**  
  Users provide a dish name, and the AI responds with a detailed recipe including ingredients and step-by-step instructions.

- **Recipe Critique and Improvement Suggestions:**  
  If users describe an issue with a recipe they tried, the AI offers constructive feedback and improvements.

- **Polite Input Handling:**  
  If the input is unclear or doesn’t fit a scenario, the AI politely asks for clarification.

## How It Works

1. **Automatic Input Detection:**  
   - The AI intelligently determines whether the input is an ingredient list, dish name, or recipe critique.
   - No need for the user to specify the input type manually.

2. **Real-Time Streaming:**  
   - The AI responds in real-time, making the interaction more dynamic and engaging.

3. **Politeness and Flexibility:**  
   - If the input is ambiguous, the AI prompts for a valid request or additional details.

---



### Required Libraries

Make sure to install the `openai` library:

```python
pip install openai
```

---

## Usage Instructions

1. **Clone the Repository** or place the `chef-gpt.py` file on your system.
2. **Set up the OpenAI API Key for Windows**:
   ```bash
   set OPENAI_API_KEY=your_api_key_here
   ```
3. **Run the Script**:
   ```bash
   python chef-gpt.py
   ```

4. **Interact with the AI Chef**:
   - **Ingredient Input**: Provide a comma-separated list of ingredients.
     ```
     Example: flour, potatoes, tamarind, spices
     ```
   - **Dish Name Input**: Provide a dish name.
     ```
     Example: Pani Puri
     ```
   - **Recipe Critique**: Provide feedback on your cooking attempt.
     ```
     Example: My Pani Puri turned out soggy, what can I improve?
     ```

5. **Exit the Program**:
   - Type `exit` to quit the script.

---

## Example Interaction

**User Input:**
```
flour, potatoes, tamarind, spices
```

**AI Chef Response:**
```
With those ingredients, you could make: Pani Puri, Aloo Tikki, or Samosa!
```

**User Input:**
```
Pani Puri
```

**AI Chef Response:**
```
Here’s a detailed recipe for Pani Puri: 
- Ingredients: Semolina, potatoes, tamarind chutney...
- Steps: 1. Prepare the puris by frying semolina dough... (continues)
```

---

## Error Handling

- **Invalid Input**: If the input doesn't fit any expected scenario, the AI will politely ask for clarification.
- **Ambiguous Requests**: The AI might request more specific input if needed.
