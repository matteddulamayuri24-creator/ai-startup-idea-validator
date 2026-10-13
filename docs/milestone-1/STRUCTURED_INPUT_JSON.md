# Structured Startup Idea Input

## 1. Purpose
The application converts form input into JSON so that the backend
and AI agents can process the startup idea consistently.

## 2. Example Input

- Startup Idea Name: RentRight AI
- Description: A platform that helps students and working
  professionals find rental accommodation.
- Target Customers: Students and working professionals
- Industry: Real Estate Technology
- Additional Information: Focus on affordable rental options.

## 3. Example JSON Output

json
{
  "startup_name": "RentRight AI",
  "description": "A platform that helps students and working professionals find rental accommodation.",
  "target_customers": [
    "Students",
    "Working professionals"
  ],
  "industry": "Real Estate Technology",
  "additional_information": "Focus on affordable rental options."
}


## 4. Field Descriptions

| Field | Data Type | Purpose |
|---|---|---|
| startup_name | String | Name of the startup |
| description | String | Explanation of the idea |
| target_customers | Array of strings | Intended customer groups |
| industry | String | Relevant business sector |
| additional_information | String | Optional details |

## 5. Validation Rules
- Startup name must not be empty.
- Description must not be empty.
- Target customers must be provided.
- Industry must be selected or entered.
- Additional information is optional.
- The application should reject invalid input before analysis.

## 6. Processing Approach
The form will collect the information, and the Python backend will
convert it into JSON. An LLM may assist with normalizing free-text
input if necessary, but basic JSON creation does not require an LLM.

## 7. Current Status
This is an example data structure. It will be tested against the
actual application during implementation.
