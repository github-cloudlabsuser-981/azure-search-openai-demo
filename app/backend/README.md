# Backend Documentation

This documentation provides an overview of the backend part of the application located in the `/app/backend` directory.

## Directory Structure

- `app/backend/approaches`: This directory contains different approaches for handling user requests.

## Key Files

- `chatreadretrieveread.py`: This file contains the approach used for the chat tab. It calls the OpenAI ChatCompletion API to turn the user question into a good search query, queries Azure AI Search for search results for that query, and then combines the search results and original user question to answer the question based on the sources.

## Running the Backend

To run the backend locally, follow these steps:

1. Navigate to the `app/backend` directory.
2. Run your application.

Please note that the exact commands may vary depending on your application setup.

## Customization

You can customize the backend by modifying the classes in the `app/backend/approaches` directory. The `system_message_chat_conversation` variable is currently tailored to the sample data and should be changed to match your data.

## Deployment

After the application has been successfully deployed you will see a URL printed to the console. Click that URL to interact with the application in your browser. Note that it may take 5-10 minutes after you see 'SUCCESS' for the application to be fully deployed. If you see a "Python Developer" welcome screen or an error page, then wait a bit and refresh the page.

> NOTE: Running the deployment command will incur immediate costs, primarily from the AI Search resource. These resources may accrue costs even if you interrupt the command before it is fully executed. You can run `azd down` or delete the resources manually to avoid unnecessary spending.