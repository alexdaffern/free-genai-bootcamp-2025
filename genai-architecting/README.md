## Functional Requirements

The client requires all data to be stored and processed within their own network.

The client is willing to invest in dedicated hardware to host the LLM and necessary software locally.

Allocated budget for a single server is €12,000.

The client has multiple networked locations where the software will be used.

The expected usage pattern is consistent throughout the day rather than large spikes in concurrent users. Max student load 1000 at a time. 



## Assumptions

Open-source LLMs can be effectively prompt-engineered to deliver high-quality responses while running locally within the given budget.

The client has adequate database infrastructure available.

A single server with a €12,000 budget can support an adequately powerful LLM and associated software for the required tasks.

Networked client locations will not introduce significant latency issues when accessing the server.


## Data Strategy

All user and system-generated data will be stored locally on either the LLM server or the client's existing databases.

No external APIs or cloud services will be used for processing or storing data.

The LLM's training and fine-tuning (if necessary) will be performed using locally stored datasets.

## Promping Quality Optiisation Techinques Discovered

Initial tests showed that locally hosted models struggled with tasks requiring both translation and error correction.32B parameter models did not translate Finnish with sufficient precision.

A more reliable approach was identified: providing the LLM with the correct Finnish sentence in advance, allowing it to focus solely on the student's mistakes rather than hallucinating new words.
To maintain data privacy and accuracy while ensuring translations remain local, [LibreTranslate](https://libretranslate.com/) locally to keep everything locally as requested by the client.  can be hosted on-premises to translate English input before passing it to the LLM.
