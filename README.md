Try **Google Gemini Multimodal Live API** with **realtime vision** and **realtime screenshare detection** capabilities, it is a ready-to-use extension, along with powerful tools like **Weather Check** and **Web Search** integrated perfectly


### Prerequisites

| Category | Requirements |
|----------|-------------|
| **Keys** | • Agora [ App ID ](https://docs.agora.io/en/video-calling/get-started/manage-agora-account?platform=web#create-an-agora-project) and [ App Certificate ](https://docs.agora.io/en/video-calling/get-started/manage-agora-account?platform=web#create-an-agora-project)(free minutes every month) <br>• [OpenAI](https://openai.com/index/openai-api/) API key<br>• [ Deepgram ](https://deepgram.com/) ASR (free credits available with signup)<br>• [ FishAudio ](https://fish.audio/) TTS (free credits available with signup)|
| **Installation** | • [Docker](https://www.docker.com/) / [Docker Compose](https://docs.docker.com/compose/)<br>• [Node.js(LTS) v18](https://nodejs.org/en) |
| **Minimum System Requirements** | • CPU >= 2 Core<br>• RAM >= 4 GB |

<br>



<br>

### Next step

#### 1. Create `.env` file

```bash
cp ./.env.example ./.env
```

#### 2. Setup Agora App ID and App Certificate in `.env`

```bash
AGORA_APP_ID=
AGORA_APP_CERTIFICATE=
```

#### 3. Start agent development containers
```bash
docker compose up -d
```

#### 4. Enter container
```bash
docker exec -it ten_agent_dev bash
```

#### 5. Build agent 
```bash
task use
```

#### 6. Start the web server
```bash
task run
```

#### 7. Edit playground settings
Open the playground at [localhost:3000](http://localhost:3000) to configure your agent.
 1. Select a graph type (e.g. Voice Agent, Realtime Agent)
 2. Choose a corresponding module
 3. Select an extension and configure its API key settings


#### Running Gemini Realtime Extension
Open the playground at [localhost:3000](http://localhost:3000).

 1. Select voice_assistant_realtime graph
 2. Choose Gemini Realtime module
 3. Select v2v extension and enter Gemini API key

