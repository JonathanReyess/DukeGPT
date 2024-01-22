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

- **Greeting**: Handles greetings from users.
- **Feedback**: Manages user feedback.
- **Unknown Intent**: Deals with unknown user intents.
- **Person**: Manages conversations related to a person.
- **Reminder Conversation**: Handles reminders.
- **Session Expire Conversation**: Manages sessions that are about to expire.
- **HelloDialog**: Initiates a conversation with a hello.
- **EndConvo**: Ends the conversation.

Feel free to explore and modify these dialogs based on your requirements!

## Contributions

Contributions to DukeGPT are welcome. If you encounter any issues or have suggestions, please create a new issue or pull request. Let's make DukeGPT even better together!
