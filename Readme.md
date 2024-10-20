# Meta Hackathon 2024 - Karya AI Team

## Problem Statement
The urgent need to earn a living leaves people from low-income and marginalized backgrounds with little time to educate themselves on relevant and immediately beneficial topics such as financial and data literacy. Additionally, any educational material they might encounter is likely to be academic and culturally irrelevant in nature.

## Solution
Since its inception in 2021, Karya has provided marginalized communities across India with opportunities to augment their income by offering remote, flexible, and fairly compensated digital data generation work. Although Karya enables these individuals to earn supplemental income from this digital work, their educational opportunities are scarce. In an effort to tackle this, Karya’s recent research has demonstrated that integrating a story-based curriculum with the platform’s voice-annotation framework could significantly enhance Karya workers' financial literacy in matters such as budgeting, banking, and loan taking.  However, these stories were written manually, requiring several months of human effort.
In our solution, we build on our previous success in story-based education by automating the process of story-generation through a Retrieval Augmented Generation (RAG) component. This RAG component will be built using a comprehensive dataset of publicly available information. It will be integrated with the pre-trained Llama 3.1 to generate diverse and culturally relevant stories through a multi-agent approach.

We restrict ourselves to two educational domains: financial literacy and data literacy. Data sources will be validated by our on-ground experts before the RAG training process. Finally, since Llama 3.1 provides support for Hindi, we will maintain Hindi as the medium of instruction to increase our outreach to a wide population of Indian speakers.  These stories, disseminated on the Karya platform through voice-annotation tasks, will provide employment and critical supplementary income for marginalized workers while equipping them with essential knowledge on socially relevant topics.

## Tech Stack
- Python
- Ollama
- Llama 3.1
- NLTK
- Azure
- [Karya Platform](https://karya.in)

## Infrastructure
1. We hosted LLAMA model on Azure GPU VM with A100 GPU.
2. We used Ollama for inference over different models

## LLAMA Model
LLAMA3.1-70b instruct finetune and LLAMA3.1-8b instruct finetune models were used for the project.
LLAMA3.1-8b instruct finetune model was used for smaller tasks and agents while LLAMA3.1-70b instruct finetune model was used for larger tasks and agents.


## How to run the code
1. Clone the repository
2. Install the requirements - ollama
3. Open the juptyer notebook fill the prompts and system instructions in the code and run the code

## Team Members
1. [Aasim Mirza](aasim.mirza@karya.in)
2. [Nidhi Kulkarni](nidhi@karya.in)
3. [Aditya Yadavalli](aditya@karya.in)
4. [Ananya Saxena](ananya@karya.in)

Note: For the sake of privacy, we have not included the dataset and the prompts in this repository. Please reach out to us for the same.