Multi-modal Sentiment Analysis 

## Overview

This project integrates the BLIP model for image captioning with a sentiment analysis model to perform multi-modal sentiment analysis. The system is designed to analyze social media posts that include both images and text, generating captions for images and evaluating the sentiment of both the captions and accompanying text. The overall sentiment score provides a comprehensive view of the sentiment expressed in the content.

## Instructions to Run the Project

### Prerequisites

- Python (v3.10+ recommended)
- Poetry (A Python packaging and dependency management tool)
- HuggingFaceAPI Token

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-repo/blip-integrations.git
   cd blip-integrations/src

2. Create and Configure .env File

Create a .env file and add your HuggingFaceAPI Token: 
 ````bash
    nano .env

3. Add the following line to the .env file:

plaintext
Copy code
export HUGGING_FACE_ACCESS_TOKEN="Your HuggingFaceAPI Token"
      poetry install

### Configuration
1. Set your Google Maps API key in the traffic_agent.py and public_transport_agent.py scripts.
      google_maps_api_key = "YOUR_GOOGLE_MAPS_API_KEY"

### Running the Project
1. Start the agents
    python src/agents/traffic_agent.py
    python src/agents/public_transport_agent.py
2. Start the main application
     python src/main.py

### Usage
1. Run the user_agent.py script to interact with the system:
     python src/agents/user_agent.py
2. Enter the starting and destination locations when prompted to get the optimal routes based on real-time traffic and public transportation data

### Project Structure
- agents: Contains the implementation of different agents.
  - traffic_agent.py: Monitors real-time traffic conditions, including congestion and accidents.
  - public_transport_agent.py: Manages public transportation schedules and availability.
  - user_agent.py: Interacts with the user to get their current and destination locations.
  - main.py: The main script to coordinate the agents.
- messages: Reserved for message handling (if required).
- utils: Reserved for utility functions (if required).
