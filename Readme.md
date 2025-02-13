# LangDB.ai & Rasa-pro Conversational AI Starter Pack

Welcome to the ultimate repository for building a scalable, next-gen conversational AI using **LangDB.ai** and **Rasa-pro**! This starter pack leverages the CALM architecture and an Intentless policy to provide seamless AI integration solutions—perfect for PoCs, final year projects, or enterprise applications.

## Features

- **Seamless Integration:** Easily merge LangDB.ai with Rasa-pro.
- **Scalable Chatbot:** Build chatbots using advanced CALM architecture.
- **Advanced AI Observability:** Leverage AI analytics, operational visibility, and enterprise AI governance.
- **Free Starter Credit:** Kickstart your project with a $10 free credit from LangDB.ai!

## Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/langdb/rasa-starter-pack.git
   cd rasa-starter-pack
   ```

2. **Set Up Your Environment:**
   ```bash
   conda create -n rasa-env python=3.10
   conda activate rasa-env
   pip install uv
   uv pip install rasa-pro --extra-index-url=https://europe-west3-python.pkg.dev/rasa-releases/rasa-pro-python/simple/
   ```

3. **Initialize Your Rasa Project:**
   - Obtain your Rasa-pro license key and set it in your environment:
     ```bash
     # For Windows:
     set RASA_PRO_LICENSE=your-key
     # For macOS/Linux:
     export RASA_PRO_LICENSE=your-key
     ```
   - Initialize the project with CALM template:
     ```bash
     rasa init --template calm
     ```

4. **Configure LangDB.ai Integration:**
   - Update your `config.yml` and `endpoints.yml` with your project details.
   - Set the following environment variables:
     ```bash
     export OPENAI_API_KEY=your-api-key
     export OPENAI_BASE_URL=https://api.us-east-1.langdb.ai/your-project-id/v1
     export RASA_PRO_LICENSE=your-rasa-pro-license-key
     ```

5. **Train and Run Your Model:**
   ```bash
   rasa train
   ```
   - Open two terminal windows:
     - **Terminal 1:** Start the actions server:
       ```bash
       rasa run actions
       ```
     - **Terminal 2:** Launch the interactive chat UI:
       ```bash
       rasa inspect --debug
       ```

## Getting Started

Dive into the code and instructions to customize your conversational AI. For more details, check out our [Blog](https://blog.langdb.ai/how-to-build-an-epic-conversational-ai-with-langdbai-and-rasa-pro-and-get-10-free-credit) and [Youtube Video](https://youtu.be/Se_pEedNe_4). 
Remember to claim your $10 free credit from LangDB.ai to experiment with these cutting-edge tools without any upfront cost!


## Contributing

Contributions are welcome! Please open issues or submit pull requests to help improve this project.

## License

This project is licensed under the MIT License.

---

Happy coding, and may your AI always be as smart, scalable, and observable as possible!