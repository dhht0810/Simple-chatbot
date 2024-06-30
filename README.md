# Simple-chatbot

## Simple Chatbot App with Streamlit and HugChat

This is a basic chatbot application built using Streamlit and HugChat. It allows users to interact with a large language model (LLM) in a conversational way.

**Features:**

-   **Simple user interface:** Streamlit provides a user-friendly interface for text input and chatbot responses.
-   **HugChat integration:** Leverages HugChat, an unofficial port to the Hugging Face Chat API, to interact with an LLM.
-   **Real-time conversation:** Users can type their questions or prompts, and the app displays the LLM's generated responses.

**Requirements:**

-   Python 3.x ([https://www.python.org/downloads/](https://www.python.org/downloads/))
-   Streamlit ([https://docs.streamlit.io/](https://docs.streamlit.io/))
-   HugChat ([https://github.com/dataprofessor/hugchat](https://github.com/dataprofessor/hugchat))
-   A Hugging Face account and access to an LLM model (e.g.,  [https://huggingface.co/docs/transformers/en/index](https://huggingface.co/docs/transformers/en/index))

**Installation:**

1.  Clone this repository or download the files.
    
2.  Install required libraries:
    
    Bash
    
    ```
    pip install streamlit hugchat
    
    ```
    

    
3.  Create a Hugging Face account and obtain an API token ([https://huggingface.co/docs/hub/en/security-tokens](https://huggingface.co/docs/hub/en/security-tokens)).
    
4.  Store your API token securely (**not** in the code itself). Refer to Streamlit documentation for secrets management ([https://docs.streamlit.io/deploy/streamlit-community-cloud/deploy-your-app/secrets-management](https://docs.streamlit.io/deploy/streamlit-community-cloud/deploy-your-app/secrets-management)).
    

**Usage:**

1.  Run the app:
    
    Bash
    
    ```
    streamlit run app.py
    
    ```

   2.  Type your questions or prompts in the text box.
    
3.  The app will display the LLM's response below the input field.
    

**Explanation:**

-   **main.py:** This script contains the core logic of the app.
    -   Imports necessary libraries (Streamlit, HugChat).
    -   Loads your Hugging Face API token (securely).
    -   Creates a Streamlit layout with a text input field for user queries.
    -   When the user types and submits their input, the script sends it through HugChat to interact with the LLM.
    -   The app then displays the LLM's response back to the user.

**Customization:**

-   You can experiment with different LLM models available on Hugging Face for potentially more specialized responses.
-   The app can be extended to store conversation history or implement functionalities like user authentication.
