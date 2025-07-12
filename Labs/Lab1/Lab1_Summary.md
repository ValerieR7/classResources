{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "provenance": []
    },
    "kernelspec": {
      "name": "python3",
      "display_name": "Python 3"
    },
    "language_info": {
      "name": "python"
    }
  },
  "cells": [
    {
      "cell_type": "markdown",
      "source": [
        "# Lab 1 Summary"
      ],
      "metadata": {
        "id": "CZuw9R7AGt7f"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Environment Setup\n",
        "- GCP Project ID: focal-furnace-465023-g3\n",
        "- GitHub Repository: https://github.com/ValerieR7/classResources\n",
        "- Data Lake Bucket: mgmt599-valerierobert-data-lake\n",
        "\n",
        "## Key Findings\n",
        "1. Roughly 1 in 5 orders currently result in a loss, indicating a significant issue with pricing, costs, or discounting strategies.\n",
        "2. Texas, Pennsylvania, and Illinois are the leading states for unprofitable orders, particularly within the Office Supplies and Furniture categories.\n",
        "3. Office Supplies and Furniture are the most problematic categories, and orders with discounts of 30-40% and 40%+ are disproportionately contributing to unprofitability.\n",
        "\n",
        "\n",
        "## DIVE Analysis Results\n",
        "\n",
        "1. Business Question Investigated: Compare orders where profit is negative but sales are positive, to understand their distribution across categories and states, and identify underlying causes.\n",
        "\n",
        "2. Main Discovery: Unprofitable orders are a widespread issue (roughly 20% of all orders), heavily skewed towards Texas, Pennsylvania, and Illinois, particularly in Office Supplies and Furniture. The primary driver appears to be overly aggressive discounting.\n",
        "\n",
        "3. Strategic Recommendation: Implement targeted interventions focusing on re-evaluating discounting policies in high-loss categories and states, optimizing product mix towards higher-margin items, and investigating regional operational inefficiencies to reduce costs.\n",
        "\n",
        "## Challenges and Solutions\n",
        "- Challenge faced: The challengge I faced was using my API Key and using bigquery in the notebook was slightly difficult.\n",
        "- How I solved it: I realized just helpful gemini is, and began asking it all my environment set up questions and quickly got the hang of it!\n",
        "\n",
        "## Time Spent\n",
        "- Environment setup: 40 minutes\n",
        "- Data lake creation: 20 minutes\n",
        "- Analysis: 30 minutes\n",
        "- Total: 1.5 hours\n"
      ],
      "metadata": {
        "id": "SvFAt1SAIUEw"
      }
    }
  ]
}