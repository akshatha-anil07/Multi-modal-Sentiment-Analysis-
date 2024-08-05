# Traffic-Flow-Optimization

## Overview

Traffic Flow Optimization is a real-time traffic flow optimization system that uses uAgents to manage different aspects of traffic, including congestion, accidents, and public transportation schedules. The system leverages APIs to gather real-time data and provides users with optimal routes based on current traffic conditions and public transport availability.

## Directory Structure

Sure, here's a complete README.md file for the project:

markdown
Copy code
# TrafficFlowOptima

## Overview

TrafficFlowOptima is a real-time traffic flow optimization system that uses uAgents to manage different aspects of traffic, including congestion, accidents, and public transportation schedules. The system leverages APIs to gather real-time data and provides users with optimal routes based on current traffic conditions and public transport availability.

## Directory Structure

TrafficFlowOptima/
├── poetry.lock
├── pyproject.toml
├── README.md
└── src
├── agents
│ ├── traffic_agent.py
│ ├── public_transport_agent.py
│ ├── user_agent.py
│ └── init.py
├── main.py
├── messages
│ └── init.py
└── utils
└── init.py

## Getting Started

### Prerequisites

- Python 3.7+
- [Poetry](https://python-poetry.org/) for dependency management
- API keys for Google Maps (or other relevant services)

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/TrafficFlowOptima.git
   cd TrafficFlowOptima
2. Install dependencies using Poetry 
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
