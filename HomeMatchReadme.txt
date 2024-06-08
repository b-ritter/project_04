# Home Match Hawaii Project

documentation file that explains the functionality, how to run the code, and any prerequisites or dependencies.

## Overview

The Home Match Hawaii project is a fictionalized real estate agent that takes into account a user's preferences (location, amenities, etc.) and returns a personalized list of recommendations. In this small-scope project, the  recommendations are llm-generated based on a specific region and state, presumably within the United States. I chose Oahu, Hawaii as the region/state combo, because it is awesome. The user could easily expand this to multiple locations.

## Functionality
Home Match Hawaii implements a RAG (Retrieval Augmented Generation) architecture to tailor its responses. It uses LangChain as a helper library for prompt engineering and document retrieval. The large language model and embeddings are OpenAI's ChatGPT 3.5. For vector db storage, I use LanceDB. 

## Prerequisites
A few libraries are required to be installed in addition to the default Udacity workspace prior to running the notebook. To create a conda environment suitable for running the notebook, you can run the following command:

`conda create --name <env_name> --file requirements.txt`

## How to Run the Code
Finally, make sure to provide your OpenAI key either in the code or as an environment variable.

Once all the above requirements have been met, run all the cells. Note that to provide alternate personas, it is necessary to comment/uncomment lines in the "User Preference" section of the document.

## Additional Notes
The initial prompt to generate listings is included as a separate file because it is a bit verbose.