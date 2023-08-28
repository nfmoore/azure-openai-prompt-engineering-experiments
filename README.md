# Prompt Engineering Experiments with GPT-3.5 on Azure OpenAI

Prompt engineering is an essential part of working with Azure OpenAI. It allows you to customize the behavior of the model to your specific use-case. This repository includes a Jupyter notebook that demonstrates how to use prompt engineering with Azure OpenAI. It will provide examples of how to use prompt engineering can be used to generate better results across several use-cases. By exploring this repository you will have a better understanding of how to use prompt engineering with Azure OpenAI and how it can help you build better models.

Use-cases explored in this repository include:

- Text sumarization
- Information retrieval
- Entity recognition
- Sentiment analysis
- Text translation
- Code generation

Two publically available texts have been used in these experiments:

- [Microsoft 2022 Shareholder Letter](https://www.microsoft.com/investor/reports/ar22/download-center/)
- [Reuters news article on the Microsoft acquisition of Activision Blizzard](https://www.nasdaq.com/articles/uk-blocks-microsoft-$69-bln-activision-deal-over-cloud-gaming-concerns)

> **Note:**
>
> All experiments have been conducted with following Azure OpenAI deployment:
> - Model name: gpt-35-turbo-16k
> - Model version: 0613
>
> It is recommended to use the same deployment to reproduce the results.

## Getting Started

### Create conda environment

Create a new conda environment from the [`conda.yml`](environment/conda.yml) file. This file contains all dependencies needed to run the Jupyter notebook. Activate the environment:

```bash
conda env create -f environment/conda.yml
```

### Create environment variables

Create a new file called `.env` in the root of the repository. Add the following environment variables to the file:

```bash
AZURE_RESOURCE_NAME=<your-resource-name>
OPENAI_API_KEY=<your-api-key>
OPENAI_DEPLOYMENT_NAME=<your-deployment-name>
```

These environment variables are used to connect to your Azure OpenAI resource. You can find the values for these variables in the Azure portal.

### Run the Notebook

Open the jupyter notebook [`prompt-engineering.ipynb`](src/prompt-engineering.ipynb), choose a use-case and run the notebook. Ensure you run this notebook in the conda environment you created earlier.

## Resources

- [Azure OpenAI Documentation](https://learn.microsoft.com/azure/cognitive-services/openai/overview/)
