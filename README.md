# DukeGPT

2023 Code+ Program project where we worked with Duke’s Office of Information Technology, Microsoft, and partners across campus to design and develop an AI customer service chat platform for Duke University.

## 

## Getting Started

To get a local copy up and running follow these simple steps.

### Clone Project

Paste the following command into your terminal:

```
git clone -b DukeGPT https://gitlab.oit.duke.edu/codeplus/fixit_ai.git
```

### .NET Core SDK 

Install .NET Core SDK

This bot is running on C#. C# requires the .NET Core SDK.
Install .NET Core SDK 7.0.

https://dotnet.microsoft.com/en-us/download/dotnet/7.0 

To make sure you have .NET installed run the following command in your terminal:

```
dotnet --version
```

### Environment

Fill in the appropriate keys which can be found within your Azure service in /DukeGPT/settings/appsettings.json along with your publishing profile. 

### Web Chat

If you are on Mac, make sure you have disabled airplay in order to run the bot in the web chat within Bot Framework Composer.

System Settings -> General -> Airdrop & Handoff -> Airplay Receiver

### Bot Framework Composer

To make changes and publish your bot, install Bot Framework Composer. 

https://github.com/microsoft/BotFramework-Composer/releases/download/v2.1.2/BotFramework-Composer-2.1.2-mac.zip

### Bot Framework Emulator 

To run your bot locally on your PC, install the appropriate version of the Framework Emulator for your device.

https://github.com/Microsoft/BotFramework-Emulator/releases/tag/v4.14.1

### Publishing a Bot 

The current chatbot is using the resources listed in the publishing_profile.txt file. 







