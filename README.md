# ai-zen
Progressive Framework for Agentic EA

# ollama 4 brew
<pre>
export HOMEBREW_NO_AUTO_UPDATE=0
brew upgrade ollama
brew services restart ollama
ollama -v
ollama version is 0.13.5
  
vi homebrew.mxcl.ollama.plist
    <key>OLLAMA_FLASH_ATTENTION</key>
    <string>1</string>
    <key>OLLAMA_KV_CACHE_TYPE</key>
    <string>q8_0</string>
    <key>OLLAMA_NUM_PARALLEL</key>
    <string>16</string>
    <key>OLLAMA_MAX_LOADED_MODELS</key>
    <string>8</string>
    <key>OLLAMA_MAX_QUEUE</key>
    <string>512</string>
    <key>OLLAMA_KEEP_ALIVE</key>
    <string>72h</string>
    <key>OLLAMA_NUM_THREADS</key>
    <string>16</string>
    <key>OLLAMA_CONTEXT_LENGTH</key>
    <string>20480</string>
    <key>OLLAMA_HOST</key>
    <string>0.0.0.0:11434</string>

#配置检查
plutil ./homebrew.mxcl.ollama.plist
diff ./homebrew.mxcl.ollama.plist  ~/Library/LaunchAgents/homebrew.mxcl.ollama.plist
cp ./homebrew.mxcl.ollama.plist  ~/Library/LaunchAgents/homebrew.mxcl.ollama.plist

#重载服务（不要用 brew services restart，否则可能覆盖环境变量）：
launchctl unload ~/Library/LaunchAgents/homebrew.mxcl.ollama.plist
launchctl load ~/Library/LaunchAgents/homebrew.mxcl.ollama.plist

#检查生效
lsof -iTCP:11434 -sTCP:LISTEN
ps eww $(pgrep ollama) | grep OLLAMA  
</pre>

# qwen3 /no_think
ollama create qwen3n -f qwen3n.Modelfile

![SDK](./share/chat-ai/embed.png "embed sdk")

![EA](./WechatIMG322.jpg "Progressive Framework L1-L4 for everyone")

![认知](./IMG_9548.jpeg "cognition")

![263759c6cc24be5039d7b558a35e1807](https://github.com/user-attachments/assets/6986da37-9d60-4350-b6f7-b9de31c409ff)

![f44340cdc2fed2459f05f9716c8eb81a](https://github.com/user-attachments/assets/3a8695a8-16fd-469d-9eac-3e406d32f1dc)

![b8eba24054d8b3af61578b2c5db9de3a](https://github.com/user-attachments/assets/1dd7b5bb-b17e-4496-881e-afe5553e5855)

![fceb5b8bbeb20d4ccf89e07c1d5ddd97](https://github.com/user-attachments/assets/665d69ca-0e2f-4dcd-b3a5-7aa1b6b5ee60)

![281e1bcbb4b97f788e6453c6afe54bb1](https://github.com/user-attachments/assets/229f0358-c5d3-4121-96bb-dd0950b16b3f)

![013edda4005b6a44bbd9723fe0367eba](https://github.com/user-attachments/assets/c146c296-5fc3-4011-b227-811c4bcc8836)

<img width="2670" height="1570" alt="1eec4a5dc79b70c60653afaf45249a1b" src="https://github.com/user-attachments/assets/8f1108e9-1181-4671-a0b6-74690939c0de" />

![35df4e63826eb3b544039668441c60d8](https://github.com/user-attachments/assets/812cd578-06a5-4bb4-8619-a195873fee36)

![02e9b04e6a026d51b84e6f4df9e4d42a](https://github.com/user-attachments/assets/a535bd19-6f4b-4876-a4e4-62c38a0c4e2e)

