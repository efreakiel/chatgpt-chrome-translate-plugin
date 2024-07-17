### ChatGPT Translation Bot

This extension uses the OpenAI ChatGPT API to translate the selected text into your desired language. It supports 20+ languages and can be used with a proxy.

This is a completely free and open source project. You can configure your api key in the settings page of the extension and can trust it to protect your privacy.

## Features
- Automatically detect the language of the selected text and auto translate it into your desired language.
- Support the context menu and shortcut key to translate the selected text.
- Support proxy and custom headers for the people who use a proxy to access ChatGPT.
- Support a webhook url so the data can be sent to your own app/server.
- Support 20+ languages.
- Can highlight the selected text, just like a marker pen.

## Installation
Compile the extension with 'npm run build' or unzip the compiled_extension.zip file and Load the extension in Chrome by navigating to chrome://extensions/, enabling "Developer mode," and clicking "Load unpacked."
Then Select the extension's directory (the dist folder extracted from chrome_extension.zip).

## How to setting
- Go to the settings page of the extension.
- Fill in your OpenAI api key.
- Select the language you want to translate to.
- Click the save button.

**Attention:** Whenever you changed the settings, you need to refresh the page to make the new settings take effect.

![how to config](/images/how-to-config.png)

#### Other options:
- If you use a proxy to access ChatGPT, you can check the `Use proxy` option and fill in a proxy address.
if your proxy needs some custom headers, You can fill in the custom headers by checking the `Add custom headers` option.
- If you want to show the context menu, you can check the `Show context menu` option. If you don't want to show it, You can use the shortcut key **t or T** to translate the selected text.

## How to use
1. Select the text you want to translate.
2. Click the menu item from the context menu.(A context menu will appear automatically when you select text. The context menu only is shown when you check the `Show context menu` option in the settings page.)
3. You can also use the shortcut keys **T** or **t** to translate the selected text. The translated text will then be appended after the selected text. The translation shortcut default to the **T** key, but you can change it in the settings page. 


![how to use](/images/how-to-use.png)

5. You can use number key **1, 2, 3, 4, 5** to color the selected text like a marker pen. To use the number **6** to add text shadow to the selected text. If you want to remove the highlight, you can use the number **0**.   
The number **6** can be combined with other numbers(**1, 2, 3, 4, 5**) to form an overlay effect of color and font shadow.  

![how to use](/images/highlight-1.png)

![how to use](/images/highlight-2.png)

![how to use](/images/highlight-3.png)

![how to use](/images/highlight-4.png)

![how to use](/images/highlight-5.png)

![how to use](/images/highlight-6.png)

Click this link to see the [demo video](https://www.youtube.com/watch?v=JLqsyhCxiBM).

## About use proxy in this extension  
If you use a VPN tool to access ChatGPT or it's API, you need to turn on the VPN while using this extension. 
But if you don't want to use a VPN, we provide this free proxy **https://common.navitechai.com/v1** to drive this extension, you can try it in your country. Hope it works for you.  
To config proxy as the screenshot below: 
![config the proxy](/images/free-proxy.png)

(**Attention** Wen can't guarantee the stability of this free proxy, if it doesn't work, you can try to use a VPN tool to access ChatGPT.)

## Webhook URL Setting  
The Webhook URL if set will receive the following JSON variables: originalText, translatedText, targetLanguage  

## Common issues   
- **Can't translate the selected text and always show 'Translating...'**   

  **Solution:** Please check your network connection and make sure the ChatGPT([chat.openai.com](https://chat.openai.com)) is accessible. If you need a VPN to access the ChatGPT, to confirm the VPN is turned on. If all of these didn't work, please to confirm you have pre-billed your OpenAI API account. Since a couple of months ago, OpenAI has changed its policy, you need to pre-bill your account to use the ChatGPT API.  


## How to contribute
* If you like it, please give it a star to support it.   
* If you have any questions or suggestions, please feel free to open an issue.    
* If you want to contribute to this project, please feel free to open a pull request.     
