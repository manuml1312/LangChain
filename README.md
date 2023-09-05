# LangChain
This repository contains a python notebook with implementation of different types of foundational chains available in the LangChain library.I have used an LLM from the hugging face repository called the Flan-T5.You can use any LLM or API's such as ChatGpt or other complex models available for which you need to import the appropriate kits within the langchain library. More details are available at their official site.
# Types of Chains
## 1. LLM Chain:
An LLMChain is a simple chain that adds some functionality around language models. It is used widely throughout LangChain, including in other chains and agents.
An LLMChain consists of a PromptTemplate and a language model (either an LLM or chat model). It formats the prompt template using the input key values provided (and also memory key values, if available), passes the formatted string to LLM and returns the LLM output.
## 2. Sequential Chain:
SimpleSequentialChain: The simplest form of sequential chains, where each step has a singular input/output, and the output of one step is the input to the next.
SequentialChain: A more general form of sequential chains, allowing for multiple inputs/outputs.
## 3. Router Chain:
To create a chain that dynamically selects the next chain to use for a given input.
Router chains are made up of two components:
The RouterChain itself (responsible for selecting the next chain to call)
destination_chains: chains that the router chain can route to
