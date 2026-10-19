# DS 402 Week 7 Travel Agent

Travel assistant built in OpenAI Agent Builder for DS 402. A classifier reads the user's message and sends it to either a Flight Agent or an Itinerary Agent.

## Goals
- Build and publish the workflow in Agent Builder (Oct 18)
- Route at least 8 of 10 test messages to the right agent (Oct 25)
- Turn it into the multi-agent version for the W7 assignment (Oct 25)

## How it works
1. Start node takes the message as input_as_text
2. Classifier (gpt-6-astra) returns JSON with a classification field
3. If/else sends "flight_info" to the Flight Agent (uses web search) and everything else to the Itinerary Agent

## Setup
1. Open https://platform.openai.com/agent-builder in the DS402 Wk7 Travel Agent project
2. Create your own API key in that project
3. Keep keys in a local .env file. Never commit them.

## Contributors
- Neel Modi (Penn State, Data Sciences): workflow, prompts, testing, repo
