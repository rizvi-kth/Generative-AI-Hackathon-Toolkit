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
OPENAI_API_KEY="<your API key>"
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

# Dataset connected to Use-cases

## 3. AI-Generated Financial Report Summarization and stock trading recommendations 

Location: `./data/fsi` 

### Unstructued Data (PDF) 

the dataset contains the Annual (10-K) SEC reports for the years 2020-2023 for the following companies: 

- [Apple Inc.(AAPL)](https://investor.apple.com/sec-filings/default.aspx) 

- [Microsoft Corporation (MSFT)](https://www.microsoft.com/en-us/investor/sec-filings.aspx) 

- [Alphabet Inc. (GOOGL)](https://abc.xyz/investor/) 

- [Nvidia Corporation (NVDA)](https://investor.nvidia.com/financial-info/sec-filings/default.aspx) 

- [Amazon.com Inc. (AMZN)](https://ir.aboutamazon.com/sec-filings) 

 

The data was obtained from the the investor relations sites of the respective companies. 

 

### Structured Data (CSV) 

 

As structured data we prepared a database with the Historical Stock Prices. 

 

The data was obtained from the following sources: [Nasdaq Historical Data](https://www.nasdaq.com/market-activity/quotes/historical) 

 
## 4. Outfit styling assistant  

Location: `./data/sample_clothes` 

### Unstructued Data (Images) 

The dataset contains a collection of clothing item images in the `./data/sample_clothes/sample_images` folder. These images showcase various clothing items, accessories, and outfits. The images are used by the outfit styling assistant to visually represent clothing options and combinations.

### Structured Data (CSV) 

The dataset contains metadata for the images in the `./data/sample_clothes/sample_images` folder.

## 5. Hotel Invoice Data Extraction

Location: `./data/hotel_invoices`

The dataset contains pdfs of hotel invoices as well as JSONs containing the extracted data performed in two steps schemaless extraction followed by schema guided extraction. 

## 6. Internal SharePoint QA 

Location: `./data/sharepoint_qa`

## 8. CV Matching  

Location: `./data/cv_matching`
