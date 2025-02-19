# Trivia Question Array Builder
*Will spit out JSON of 100-500 difficult answers in the form of questions for 5 provided categories*

### Answer the following questions based on the provided meeting transcript text:
What are the desired outcomes from a Microsoft perspective including next steps?
What is success for the customer? What are the next steps?
Include customer's technology footprint if it's relevant for this engagement
Topics of Interest / Use Cases
What are the key time frames/issues driving the schedule?
What are the key risks, topics or hot buttons to avoid with the customer?
What resources, process, or condition that is vital for success of the outcome?
Will they be attending?

Rules of Operation:
1. If you don't have an answer it's ok to answer with "insufficient data"
2. Here's the schema for generation: {  "type": "object",  "properties": {    "What are the desired outcomes from a Microsoft perspective including next steps?": {      "type": "string"    },    "What is success for the customer? What are the next steps?": {      "type": "string"    },    "Include customer's technology footprint if it's relevant for this engagement": {      "type": "string"    },    "Topics of Interest / Use Cases": {      "type": "string"    },    "What are the key time frames/issues driving the schedule?": {      "type": "string"    },    "What are the key risks, topics or hot buttons to avoid with the customer?": {      "type": "string"    },    "What resources, process, or condition that is vital for success of the outcome?": {      "type": "string"    },    "Will they be attending?": {      "type": "string"    }  }}
3. Don't confuse the schema with the output. The output should honor the schema but not be the schema.
4. Good Example:
{ "What are the desired outcomes from a Microsoft perspective including next steps?": "A paragraph or so answer to the question",
... the rest of the questions and answers
}
5. Bad example:
{  "type": "object",  "properties": {    "What are the desired outcomes from a Microsoft perspective including next steps?": {      "type": "string"    },    "What is success for the customer? What are the next steps?": {      "type": "string"    },    "Include customer's technology footprint if it's relevant for this engagement": {      "type": "string"    },    "Topics of Interest / Use Cases": {      "type": "string"    },    "What are the key time frames/issues driving the schedule?": {      "type": "string"    },    "What are the key risks, topics or hot buttons to avoid with the customer?": {      "type": "string"    },    "What resources, process, or condition that is vital for success of the outcome?": {      "type": "string"    },    "Will they be attending?": {      "type": "string"    }  }}