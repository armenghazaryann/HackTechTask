# AI Bot Conversation Quality Evaluation

## Objective
The goal of this task is to create and execute a system that evaluates AI bot responses to lead inquiries on a scale of 1 to 10. This evaluation will assess the quality of the bot's responses based on how well it addresses lead questions, fulfills their needs, and adheres to predefined instructions during conversations.

## Bot Instructions
A lead management bot interacts with new leads who have not had prior conversations. The bot aims to book leads by suggesting available intro classes in groups of three and answering their questions. The final goal is a successful booking. Upon detecting interest in any of the suggested classes, the bot asks the lead to confirm the booking. If the lead replies positively, the bot proceeds with the booking and sends a success message.

### Specific Instructions:
The bot should respond with the message:
"One of our representatives will be in touch with you shortly to assist you further" whenever any of the following is detected during a conversation:
- The lead wants to bring someone else (e.g., a friend, daughter, etc.).
- The lead asks about gift cards, payments, discounts, or costs.
- The lead wants to use 1Pass (onepass) credits.

## Dataset
The dataset contains conversations between leads and the AI bot. Each entry in the dataset includes:
- Lead and bot messages identified by numbers in the 'source' column (2 for lead, 1 for bot).
- `lead_id` and the message content.

## Output
The final deliverables for this task include:
1. A Jupyter Notebook with the code used for the evaluation.
2. A CSV file containing the results, where each row includes a lead ID and the corresponding conversation score.


### For Installing Requirements
```
pip install -r requirements.txt
```