                     
# Jira User Story Reviewer using Langflow Agent

This project automates the review of Jira User Stories using a Langflow-based AI agent. It fetches user stories from Jira, processes them through an LLM, and generates a review score based on best practices.

## Langflow Components used:

1. **API Request**  
   Connects to Jira REST API to fetch user story details using the issue key.

2. **Parser (Stringify)**  
   Converts the JSON response from Jira into a plain text format that the LLM can understand and process.

3. **Groq (Field Extraction)**  
   Extracts only the relevant fields from the user story — title, description, and acceptance criteria.

4. **Prompt Template (ICE-POT)**  
   Structures the prompt using the ICE-POT template format, passing the extracted user story as a variable for consistent evaluation.

5. **Groq (Review Generation)**  
   Analyzes the user story against best practices and generates a review score with feedback.

6. **Write File**  
   Saves the final "User Story Review Summary" along with the score into a text file for documentation.

## Output

The agent produces an HTML/Text output summarizing the user story review with actionable feedback and a quality score.

