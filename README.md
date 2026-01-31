                     
# Jira User Story Reviewer using Langflow Agent

## Langflow Components used:

1. **API Request** - Here I fetch user story from Jira API.

2. **Parser** - 'Stringify' to convert the user story which is understandable by LLM. API response gives many values.

3. **Groq** - To extract only the required fields like title, description, and acceptance criteria of the user story.

4. **Prompt Template** - ICE-POT template is used to give the prompt along with a variable.

5. **Groq** - To generate the review score.

6. **Write File** - To write the "User Story Review Summary" along with score into a text file.



