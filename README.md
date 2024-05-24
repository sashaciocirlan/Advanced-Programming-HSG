# AI-Powered Audio Weather Forecast Summaries


## Project Overview
This application provides real-time audio weather forecast summaries by fetching and analyzing weather data based on user-specified locations and time frames. The summaries are generated using APIs to convert textual weather information into authentic audio reports.

### Objective
Develop a user-friendly application that allows users to obtain audio weather forecasts summaries for a location chosen by the user.

### Technology Stack
- **Programming Language**: Python
- **Libraries**: pandas, OpenAI API
- **APIs**: Google Maps, Free Meteo API, OpenAI (text generation as well as text-to-speech)


## Project Description

### Functional Requirements
- **Input Interface**: Users can select any location/city worldwide.
- **Geolocation Retrieval**: Utilizes Google Maps API to retrieve longitudinal and latitudinal coordinates based on the user's input.
- **Weather Data Retrieval**: Uses the Free Meteo API to fetch weather data for the respective coordinates.
- **Data Processing**: Employs pandas to clean and structure the data.
- **Text Summary Generation**: Generates a weather summary through OpenAI's text generation API, incorporating the weather data. 
- **Audio Conversion**: Converts the text summary into audio using OpenAI's text-to-speech API.
- **Audio Storage**: Saves the audio file on the user's machine.

### Non-Functional Requirements
- **Usability**: The application must be easy to use for the user.
- **Error Handling**: Implements robust error handling to manage and report issues effectively.
- **Performance**: Ensures the audio generation process completes within 1 minute after data retrieval.


## Flow
1. **User Input**
   - **Description**: Users input the desired city/location.
   - **Output**: City/location name.
2. **Google Maps API**
   - **Function**: Retrieves geographical coordinates for the specified city/location.
   - **Output**: Latitude and longitude.
3. **Free Meteo API**
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
7. **Audio Output**
   - **Description**: Plays the audio weather summary to the user.
   - **Output**: User hears the weather summary.


## Installation and Setup (XXX to be completed XXX)

### Prerequisites

Ensure you have Python 3.8+ installed on your system. You will also need API keys for Google Maps, Free Meteo, and OpenAI.

If you need to connect to an API key with credits to access OpenAI, please get in touch with our team member Nikola (nikola.bulatovic@student.unisg.ch).

### Clone the Repository

```bash
git clone https://github.com/yourusername/ai-audio-weather.git
cd ai-audio-weather