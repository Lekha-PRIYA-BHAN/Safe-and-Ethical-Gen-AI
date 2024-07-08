# Multi Layered Framework for Safe and Ethical GenAI Applications

Developing GenAI applications are fraught with a potential for generating content that may be unsafe and unethical. Here we provide a multi layered framework to decrease the frequency of generation of unsafe or unethical responses.

This is an initial version.

![image](https://github.com/Lekha-PRIYA-BHAN/Safe-and-Ethical-Gen-AI/assets/167432155/21c85c16-7756-4cd3-b58c-e639b6cfae2b)


[I]()n the above diagram a GenAI application only having the blue lines (labeled 1, 5, 6, 10) would have the highest frequency of unsafe and unethical responses. However as we introduce other spokes labeled (2 through 9) we expect to considerably reduce this frequency. The spoke labelled 0 corresponds to defining and executing test cases during the testing phas of the GenAI application to catch any unsafe responses. Those spokes that are circled (i.e., 2, 8, 9, and 0) are areas where Entity should develop capabilities and experience to provide a differentiation. Note, the ordering of the spokes around the GenAI indicate the natural order in which the functionality represented by the spokes will be executed.

## Prompt Validator

This applies rules to the final Prompt before it is issued to the LLM. The rules detect if there are checks and balances to prevent any unsafe or unethical responses. Also checks the user query which would be embedded within the template for undesirability.

## Static Input / Output Filters

These input and output filters operate on the prompt as well as the response (or LLM output), respectively. They identify instances of unsafe / unethical occurences within the content passed to the filters.

## Moderation Serivce

This is a service that may be offered by the LLM vendor (for example OpenAI offers one). The service checks the content to comply with polices and returns a rating vector.

## Adaptable Filter - Monitors for Anomalies

As the name suggest this capability would adapt to detecting and flagging anomalies.

## Human

A human could be involved to check anomalies or randomly check prompts / outputs for unsafe / unethical content.
