<!-- markdownlint-disable MD030 -->

# Flowise Embed No watermark REACT COMPONENT ONLY



Install:

```bash
npm i flowise-embed-no-watermark-custom-styles
```

```bash
npm i flowise-embed-react-no-watermark-plus-minor-tweaks
```
## You need both for the watermark to be gone. 
Replace 

```
import {Chatbot} from embed-react-no-watermark-plus-minor-tweaks
```

## After use it as shown below 
Watermark is gone !!

```html
<script type="module">
  import Chatbot from 'https://cdn.jsdelivr.net/npm/flowise-embed/dist/web.js';
  Chatbot.init({
    chatflowid: '91e9c803-5169-4db9-8207-3c0915d71c5f',
    apiHost: 'http://localhost:3000',
    chatflowConfig: {
      // topK: 2
    },
    theme: {
      button: {
        backgroundColor: '#3B81F6',
        right: 20,
        bottom: 20,
        size: 'medium',
        iconColor: 'white',
        customIconSrc: 'https://raw.githubusercontent.com/walkxcode/dashboard-icons/main/svg/google-messages.svg',
      },
      chatWindow: {
        title: 'Flowise Bot',
        titleAvatarSrc: 'https://raw.githubusercontent.com/walkxcode/dashboard-icons/main/svg/google-messages.svg',
        welcomeMessage: 'Hello! This is custom welcome message',
        backgroundColor: '#ffffff',
        height: 700,
        width: 400,
        fontSize: 16,
        poweredByTextColor: '#303235',
        botMessage: {
          backgroundColor: '#f7f8ff',
          textColor: '#303235',
          showAvatar: true,
          avatarSrc: 'https://raw.githubusercontent.com/zahidkhawaja/langchain-chat-nextjs/main/public/parroticon.png',
        },
        userMessage: {
          backgroundColor: '#3B81F6',
          textColor: '#ffffff',
          showAvatar: true,
          avatarSrc: 'https://raw.githubusercontent.com/zahidkhawaja/langchain-chat-nextjs/main/public/usericon.png',
        },
        textInput: {
          placeholder: 'Type your question',
          backgroundColor: '#ffffff',
          textColor: '#303235',
          sendButtonColor: '#3B81F6',
        },
      },
    },
  });
</script>
```
## License
Source code in this repository is made available under the [MIT License](https://github.com/FlowiseAI/Flowise/blob/master/LICENSE.md).