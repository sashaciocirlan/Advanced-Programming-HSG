# AI-Powered Weather Forecast Summaries

## Project Overview
We set out to create a weather summary application that provides detailed and entertaining weather reports for any city/location entered by the user. Our goal was to develop a tool that not only fetches and analyzes weather data but also presents it in a user-friendly and engaging format. It therefore generates multimedia content by combining weather summaries with images and audio, culmniating in some kind of video forecast.

The core of our project is built around the WeatherSummaryApp class, which follows object-oriented programming principles. This class integrates several APIs, such as Google Maps for geolocation, Open-Meteo for weather data, and OpenAI for generating text, audio, and images. The Python file WeatherSummaryApp.py includes the full implementation of this class and its methods.


### Technology Stack
- **Programming Language**: Python
- **Libraries**: pandas, requests, requests_cache, retry_requests, OpenAI API, MoviePy
- **APIs**: Google Maps, Open-Meteo API, OpenAI (text generation, text-to-speech, image generation)

## Flow
1. **User Input**
   - **Description**: Users input the desired city/location.
   - **Output**: City/location name.
2. **Google Maps API**
   - **Function**: Retrieves geographical coordinates for the specified city/location.
   - **Output**: Latitude and longitude.
3. **Open-Meteo API**
   - **Function**: Fetches weather data based on coordinates.
   - **Output**: Raw weather data including temperature, precipitation, UV index, wind speed, etc.
4. **Data Processing (Pandas)**
   - **Function**: Cleans and prepares the data for text generation.
   - **Output**: Structured and cleaned weather data.
5. **OpenAI Text Generation**
   - **Function**: Generates a textual weather summary based on the cleaned weather data.
   - **Output**: Text summary of the weather.
6. **OpenAI Text-to-Speech**
   - **Function**: Converts the text summary into an audio format.
   - **Output**: Audio file of the weather summary.
7. **OpenAI Image Generation**
   - **Function**: Creates an image based on the weather summary.
   - **Output**: Image file illustrating the weather conditions.
8. **Video Creation (MoviePy)**
   - **Function**: Combines the audio and image into a video format.
   - **Output**: Video file of the weather summary.

## Declaration of aiding material
   - We used ChatGPT to help us correcting our code.
   - We used YouTube Tutorials to help us implement certain features.

## Installation and Setup

### Prerequisites

- Ensure you have Python 3.8+ installed on your system. 
- You will also need API keys for Google Maps, Free Meteo, and OpenAI. If you need to connect to an API key with credits to access OpenAI, please get in touch with our team member Nikola (nikola.bulatovic@student.unisg.ch).

### Clone the Repository
```bash
git clone https://github.com/yourusername/ai-audio-weather.git
cd ai-audio-weather
