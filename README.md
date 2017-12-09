![OctoCore Logo](https://i.imgur.com/kt0QmIo.png)

## **About** 
OctoCore is a C# library intended for Twitch and Youtube streamers. It allows them to create advanced apps based on six well-known social networking sites wrapped in one big THING. Those APIs are:
* Twitch
* YouTube
* Twitter
* Facebook
* Discord
* PayPal
 
 
 
## **Getting Started**
#### For Twitch API:
1. Add reference to OctoCore.dll and Newtonsoft.Json.dll.

2. Add using statement.
```csharp
using OctoCore;
```

3. Initialize Twitch.Credentials and Twitch.Client:
```csharp
Credentials apiCredentials = new Credentials();
apiCredentials.ApplicationID = "your_application_ID_here";
apiCredentials.Secret = "your_application_secret_here";
apiCredentials.RedirectURI = "your_application_redirect_url_here"; //currently accepting http://localhost only

Client twitchClient = new Client(apiCredentials);
```

4. When initialized, twitchClient will attempt to open an authorization link in a default browser.
	* If user clicks Agree, library will return success page.
	* If user clicks Cancel, library will return failure page and close it's local web server.

#### For YouTube API:

#### For Twitter API:

#### For Facebook API:

#### For Discord API:

#### For PayPal API:
 
 
 
## **Functions**
#### Twitch:
* send and receive chat messages, commands, whispers
* get newest follows, subs, hosts
* read user data

#### YouTube:

#### Twitter:

#### Facebook:

#### Discord:

#### PayPal:
