# 🚀 Gaia Node Installation Guide


## System Requirements to run the node

| System | Minimum Requirements |
|--------|----------------------|
| **OSX with Apple Silicon (M1-M4 chip)** | 16GB RAM (32GB recommended) |
| **Ubuntu Linux 20.04 with Nvidia CUDA 12 SDK** | 8GB VRAM on GPU |
| **Azure/AWS** | Nvidia T4 GPU Instance |



### 📥 Installing the Node

Use the following command to download the latest version of the Gaia Node:

```bash
curl -sSfL 'https://github.com/GaiaNet-AI/gaianet-node/releases/latest/download/install.sh' | bash
```

After installation, run the command displayed in the terminal to set up the environment path. This command will start with `source`.

![Description](quick-start-96fed073147105b82f4885934602852b.png)


---

### ⚙️ Initializing Gaia Node

Use the following command to initialize the Gaia Node according to the configuration options in `$HOME/gaianet/config.json`. By default, Gaia is initialized with the Llama 3.2 LLM and a knowledge base about Paris. This process may take some time as it requires downloading a large LLM file.

```bash
gaianet init
```

---

#### ▶️ Starting Gaia Node

Use the following command to start the node:

```bash
gaianet start
```

##### 📡 After Starting

If the startup is successful, the terminal will display a public URL for the node. Open a browser and visit this URL to view node information and chat with the AI agent.

🔗 **Example URL:**

```
https://0xf63939431ee11267f4855a166e11cc44d24960c0.gaianet.xyz
```

---

## ⏹️ Stopping Gaia Node

To stop the node, run the following command:

```bash
gaianet stop
```

