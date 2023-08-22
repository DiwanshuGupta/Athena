# Athena
Athena is an AI-powered chatbot designed to assist with various tasks and provide personalized experiences for users. Inspired by the Greek goddess of wisdom and strategic thinking, Athena's goal is to learn, adapt, and become a self-reliant AI agent. Built on the GPT-4 architecture, Athena communicates effectively through natural language processing and engages with a supportive human community to foster growth and development.


# Installation 

Before you begin, ensure you have the following installed:

- [Python 3.7](https://www.python.org/downloads/release/python-370/)
- [Docker](https://www.docker.com/get-started)
- [Node.js](https://nodejs.org/) (for running the React app)

Then:
- Obtain an API key from [OpenAI](https://beta.openai.com/signup/).
- Create a `.env` file in the Athena project folder with the following content:
OPENAI_API_KEY=<your_openai_api_key>
# How to open
On Windows: .\run_app.bat
### Manual Installation 

1. Install Python 3.11.

2. Clone the Athena repository:
git clone https://github.com/BillSchumacher/Athena.git
3. Change to the Athena directory:
cd Athena
4. Install the required Python packages:
pip install -r requirements.txt
#### API Mode 

1. Run the Docker container:
```
docker run -d -p 5000:5000 --name athena --env-file .env billschumacher/athena-api
```
2. Access the API at `http://localhost:5000/api/v1/athena`.
### Running the React App

1. Navigate to the `athena-app` directory:
cd athena-app
2. Install the required dependencies:
npm install
3. Start the React development server:
npm start
The React app should now be running on [http://localhost:3000](http://localhost:3000).

#### CLI Mode 

1. Run the Docker container:
```
docker run -it --rm --name athena -e ATHENA_MODE=cli --env-file .env billschumacher/athena
```
2. Interact with Athena using the command prompt.

### Running Athena Manually 

1. Change to the Athena directory:
cd Athena
2. Run the main script:
python -m athena
3. Interact with Athena using the command prompt.

## Debugging

In your .env add:
```
LOG_LEVEL=DEBUG

