# Wingman
Azure Open AI Virtual chat Assistant that can be deployed in multiple channels like Teams , Slack , Web App

## Azure Architecture ##

![image](https://github.com/mahes-a/Wingman/assets/120069348/697e719e-6d38-4833-bb7c-e3ea0e0ccd04)

## Getting Started ##

**NOTE** In order to deploy and run this example, you'll need an Azure subscription with access enabled for the Azure OpenAI service. You can request access [here](https://aka.ms/oaiapply).

### Prerequisites

1. In Azure Open AI Create a GPT 3.5 deployment 

    <img width="703" alt="image" src="https://github.com/mahes-a/Wingman/assets/120069348/44420fbb-1afa-4aa5-a55f-425d79f52202">


2. Install Bot Composer [here](https://learn.microsoft.com/en-us/composer/install-composer?tabs=windows).



3. Clone the repository:

      git clone https://github.com/mahes-a/Wingman.git

4. Update the appsettings.json file in Wingman\Wingman\settings to include the OPENAI_API_KEY and OPENAI_API_ENDPOINT

 <img width="200" alt="image" src="https://github.com/mahes-a/Wingman/assets/120069348/2b749da4-3d54-4a9e-9b7a-f393307e48fb">

   The OPENAI_API_KEY and endpoint can be retrieved from Azure Portal Azure OpenAI resource under Keys and Endpoint section
    
  <img width="699" alt="image" src="https://github.com/mahes-a/Wingman/assets/120069348/4185efc8-7b3e-428b-8205-fe7681986912">
    
   The OPENAI_API_ENDPOINT should be combination of your Azure Open AI Endpoint followed by ChatGPT deployment name followed by the api version 
    
   https://**endpointname**/deployments/**deploymentname**/chat/completions?api-version=2023-03-15-preview

   Example
   
   https://youropenai.openai.azure.com/openai/deployments/chatgpt35/chat/completions?api-version=2023-03-15-preview
   
   Open the Project from Bot Composer
   <img width="779" alt="image" src="https://github.com/mahes-a/Wingman/assets/120069348/fb0e2f29-16dc-4e86-8fca-97660ac3eb54">
  
### Publish
5. Publish the Bot to Azure from bot composer [refer here](https://learn.microsoft.com/en-us/composer/how-to-publish-bot?tabs=v2x)

7. To Acess the bot in teams channel [refer here](https://techcommunity.microsoft.com/t5/modern-work-app-consult-blog/publish-bot-app-to-teams-channel-with-bot-framework-composer-and/ba-p/3341876)
