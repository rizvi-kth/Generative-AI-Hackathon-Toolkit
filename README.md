# Generative AI Hackathon 

This repository contains snippets of code from the OpenAI Cookbook as well as exaple data and articles on Generative AI. In the `examples` folder, you will find the following folders:

- `evaluation`: Contains code for evaluating the performance of the models
- `fine-tuned-qa`: Contains code for fine-tuning the models
- `multi-modal`: Contains code for multi-modal models
- `vector-databases`: Contains code for using vector databases to store and query data, although FAISS is used in the `quickstart.ipynb` notebook.
- `utils`: Contains code for generating embeddings and other utility functions.

## Setup

1. Clone the repository
```bash
git clone https://github.com/sammyahmedtech/Generative-AI-Hackathon-Toolkit.git
```

2. Install the dependencies

* Install docker, see [here](https://docs.docker.com/engine/install/)
* If you haven't already, install `python` and `pip`
* Recommend using Cursor as your code editor, see [here](https://docs.cursor.sh/getting-started/installation)
* Create a new `.env` file in the root of the repository and set the `OPENAI_API_KEY` environment variable. (Ask me for the API key)

```bash
OPENAI_API_KEY=<your API key>
```
You can then access it in your code with `os.getenv("OPENAI_API_KEY")` or through the `dotenv` library by running `load_dotenv()` at the beginning of your script.
```bash
from dotenv import load_dotenv
load_dotenv()
```
* Create a virtual environment and install the dependencies, in the command prompt run the following:
```bash
python -m venv venv
./venv/Scripts/activate # On Windows
source venv/bin/activate # On macOS and Linux
pip install -r requirements.txt
```
3. Run the quickstart.ipynb notebook in the root of the repository.



