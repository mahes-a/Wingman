# Wingman
Azure Open AI Virtual chat Assistant that can be deployed in multiple channels like Teams , Slack , Web App

## Azure Architecture ##

![image](https://github.com/mahes-a/Wingman/assets/120069348/c245b468-3d1e-4a2f-ab7b-47b6e4dc48e5)

## Getting Started ##

**NOTE** In order to deploy and run this example, you'll need an Azure subscription with access enabled for the Azure OpenAI service. You can request access [here](https://aka.ms/oaiapply).

### Prerequisites

1. In Azure Open AI Create a GPT 3.5 deployment 

   <img width="864" alt="image" src="https://github.com/mahes-a/Wingman/assets/120069348/dd9b5f1e-7ee2-47aa-9ade-bd2c750ffa62">



2. Install Bot Composer [here](https://learn.microsoft.com/en-us/composer/install-composer?tabs=windows).



3. Clone the repository:

      git clone https://github.com/mahes-a/Wingman.git

4. Update the appsettings.json file in Wingman\Wingman\settings to include the OPENAI_API_KEY and OPENAI_API_ENDPOINT

 <img width="189" alt="image" src="https://github.com/mahes-a/Wingman/assets/120069348/62fac7a7-2a61-4aab-9587-1dbf98886ecc">


   The OPENAI_API_KEY and endpoint can be retrieved from Azure Portal Azure OpenAI resource under Keys and Endpoint section
    
  <img width="620" alt="image" src="https://github.com/mahes-a/Wingman/assets/120069348/646b0ebf-bf99-45cd-bc90-ee0fcf384b1c">
    
   The OPENAI_API_ENDPOINT should be combination of your Azure Open AI Endpoint followed by ChatGPT deployment name followed by the api version 
    
   https://**endpointname**/deployments/**deploymentname**/chat/completions?api-version=2023-03-15-preview

   Example
   
   https://youropenai.openai.azure.com/openai/deployments/chatgpt35/chat/completions?api-version=2023-03-15-preview
   
   Open the Project from Bot Composer
    <img width="810" alt="image" src="https://github.com/mahes-a/Wingman/assets/120069348/f28ac610-1599-41fa-b73f-89fcdf4ae399">

  
### Publish
5. Publish the Bot to Azure from bot composer [refer here](https://learn.microsoft.com/en-us/composer/how-to-publish-bot?tabs=v2x)

7. To Acess the bot in teams channel [refer here](https://techcommunity.microsoft.com/t5/modern-work-app-consult-blog/publish-bot-app-to-teams-channel-with-bot-framework-composer-and/ba-p/3341876)
