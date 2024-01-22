# DukeGPT

DukeGPT is a project developed as part of the 2023 Code+ Program in collaboration with Duke’s Office of Information Technology, Microsoft, and various partners across campus. The goal was to design and develop an AI customer service chat platform for Duke University.

## Getting Started

To run DukeGPT locally, follow these simple steps.

### Clone Project

Clone the project using the following command in your terminal:

```bash
git clone git@github.com:JonathanReyess/DukeGPT.git
```

### .NET Core SDK

Make sure you have the .NET Core SDK installed. This bot is written in C#, and C# requires the .NET Core SDK. Install .NET Core SDK 7.0 from [here](https://dotnet.microsoft.com/en-us/download/dotnet/7.0). To verify your installation, run the following command:

```bash
dotnet --version
```

### Environment

Fill in the appropriate keys, which can be found within your Azure service, in `/DukeGPT/settings/appsettings.json`, along with your publishing profile.

### Web Chat

If you are on a Mac, disable AirPlay to run the bot in the web chat within Bot Framework Composer. Navigate to System Settings -> General -> Airdrop & Handoff -> Airplay Receiver.

### Bot Framework Composer

To make changes and publish your bot, install Bot Framework Composer from [here](https://github.com/microsoft/BotFramework-Composer/releases/download/v2.1.2/BotFramework-Composer-2.1.2-mac.zip).

### Bot Framework Emulator

To run your bot locally on your PC, install the appropriate version of Bot Framework Emulator for your device from [here](https://github.com/Microsoft/BotFramework-Emulator/releases/tag/v4.14.1).

### Publishing a Bot

The current chatbot uses the resources listed in the `publishing_profile.txt` file.

## Dialogs

DukeGPT supports various dialogs to handle different scenarios:

- **Greeting**: Handles different greetings from users and when to initiates the conversation.
- **Feedback**: The dialog prompts users to provide feedback, collects their input,and stores it in Azure Blob Storage for easy access.
- **Unknown Intent**: Deals with unknown user intents by routing to our configured GPT 3.5 Turbo model. 
- **Person**: Manages conversations related to a person.
- **Reminder Conversation**: Action is performed automatically when there is no interaction between the user and bot within a timeframe.
- **Session Expire Conversation**: Manages when the session expires due to lack of activity.
- **EndConvo**: Ends the conversation, stores chat history in our Blob Storage and sends an email to the user with Azure Logic Apps. 

Feel free to explore and modify these dialogs based on your requirements!

