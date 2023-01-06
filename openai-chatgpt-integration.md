# OpenAI ChatGPT Integration

### Overview

An artificial intelligence research and deployment company,[ OpenAI](https://openai.com/) focuses on the creation of safe, artificial, general intelligence. Their latest AI model, called ChatGPT, has the ability to interact with a user in a conversational tone. When prompted, it composes responses relevant to the topic requested. Thunkable creators can utilize this model in their own apps and tap into the power of AI and natural language generation.&#x20;

### Create an OpenAI account and generate a secret API key

To use the OpenAI ChatGPT model in your Thunkable app, you need to generate a personal Open AI API key. To do this:

1. Navigate to [https://openai.com/api/](https://openai.com/api/)&#x20;
2. Click **Sign Up**.
3. On the Overview page, click your avatar to show the menu and select **View API Keys**.
4. Select **Create new secret key**.
5. Copy the secret key that is provided in the popup window. You will need to paste this into your Thunkable project.&#x20;

**⚠️ Important:** You will only be able to see this key once. You will not be able to copy it after the initial modal closes.

### OpenAI Integration Setup in Thunkable

To setup the OpenAI integration in Thunkable:&#x20;

1. Navigate to your project’s Blocks tab.
2. Scroll to the bottom of the blocks panel on the left side to access the Advanced section.
3. Click the expand chevron to show the Advanced components.
4. Click the plus icon next to Open AI Services (Beta).
5. Your “Open AI Services (Beta)” component will appear under the Open AI Services (Beta) drawer. Click the gear icon next to the component's name to access its properties dialog.
6. Paste your Open Secret API Key in the text box under APIKey (currently set to ‘default’).
7. Click Submit.

IMAGE

### Create a Thunkable Project Using the OpenAI Integration

#### Design Tab: Design the App’s User Interface

To utilize the OpenAI ChatGPT integration, your Thunkable project will need a minimum of:

* One text input
* One label
* Two buttons
* One image component

Below is a sample minimum viable product design:

![](<.gitbook/assets/Screenshot 2023-01-06 at 2.39.41 PM.png>)

#### Blocks Tab: Define the App’s Functionality

To access the OpenAI blocks at the bottom of the blocks panel on the left side, under the Advanced section, click the Open\_AI\_Services\_(Beta)1 component.

![](<.gitbook/assets/Screenshot 2023-01-06 at 2.35.21 PM.png>)

\
To use the OpenAI integration to display text and an image from a query, recreate the following block combination.

![](<.gitbook/assets/Screen Shot 2022-12-15 at 4.52.28 PM.png>)

Users of this app enter a query into the text input. The integration communicates with the OpenAI model and populates the label and image components when the corresponding button is clicked. The label component is populated with the text output from the OpenAI model, and the image component is populated by the image output from the OpenAI model.&#x20;

![](.gitbook/assets/Screenshot\_2023-01-03-15-55-59-63\_9dc5dd0bd3f5e5332cf0ed1172f4b46e.jpg)\
