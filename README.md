Certainly! I'll create a README that incorporates the information from the original OpenAI Realtime Console and includes the additional details about the stock analysis functionality. Here's the revised README:

# Realtime Stock Analysis Agent

This project is a real-time stock analysis agent that uses OpenAI's Realtime API and Polygon.io's financial data API to provide up-to-date stock information and analysis. It is based on and extends the [OpenAI Realtime Console](https://github.com/openai/openai-realtime-console).

## Features

- Real-time voice interaction using OpenAI's Realtime API
- Stock information retrieval using Polygon.io API
- Interactive stock price chart
- Latest news related to the queried stock
- Push-to-talk and Voice Activity Detection (VAD) modes
- Event logging and visualization
- Audio input/output management with WavRecorder and WavStreamPlayer

## Prerequisites

- OpenAI API key with access to the Realtime API
- Polygon.io API key
- Node.js and npm installed

## Setup

1. Clone the repository
2. Install dependencies:
   ```
   npm install
   ```
3. Set up environment variables:
   - Create a `.env` file in the project root
   - Add your OpenAI API key:
     ```
     OPENAI_API_KEY=your_openai_api_key_here
     ```
   - Add your Polygon.io API key:
     ```
     REACT_APP_POLYGON_KEY=your_polygon_api_key_here
     ```

## Running the Application

1. Start the development server:
   ```
   npm start
   ```
2. Open your browser and navigate to `http://localhost:3000`

## Usage

1. Click the "Connect" button to start a conversation
2. Use the push-to-talk button or enable VAD mode to interact with the agent
3. Ask about stock information, e.g., "What's the current price of AAPL?"
4. View real-time stock information, charts, and news in the right panel

## Components

- `ConsolePage`: Main component that handles the UI and logic
- `LineChart`: Displays historical stock price data
- `WavRecorder`: Handles audio input
- `WavStreamPlayer`: Manages audio output
- `RealtimeClient`: Interfaces with OpenAI's Realtime API

## API Integration

- OpenAI Realtime API: Used for voice interaction and natural language processing
- Polygon.io API: Fetches stock information, historical data, and news

## Using a Relay Server

To use a relay server for more robust implementation:

1. Create a `.env` file with:
   ```
   OPENAI_API_KEY=YOUR_API_KEY
   REACT_APP_LOCAL_RELAY_SERVER_URL=http://localhost:8081
   ```
2. Run the relay server:
   ```
   npm run relay
   ```

## Realtime API Reference Client

This project uses the `RealtimeClient` from the `openai/openai-realtime-api-beta` package. For full documentation, refer to the [GitHub repository](https://github.com/openai/openai-realtime-api-beta).

## Audio Management

The project uses `WavRecorder` and `WavStreamPlayer` from the `wavtools` library for audio input and output management.

## Notes

- The application uses a local relay server to hide the API key and run custom logic
- You can switch between manual (push-to-talk) and VAD modes for voice input
- The event log displays real-time events from both the client and server

## Troubleshooting

If you encounter issues with API keys, you can reset them by clicking on the displayed key in the UI.

## Acknowledgements

This project is based on and extends the [OpenAI Realtime Console](https://github.com/openai/openai-realtime-console). We thank the OpenAI team for providing the foundation for this application.


## Contact

[david@largitdata.com](mailto:david@largitdata.com)
