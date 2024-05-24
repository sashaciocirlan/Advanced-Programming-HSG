# WeatherSummaryApp
## Group ID: 3335

## Project Overview
We set out to create a weather summary application that provides detailed and entertaining weather reports for any city/location entered by the user. Our goal was to develop a tool that not only fetches and analyzes weather data but also presents it in a user-friendly and engaging format. It therefore generates multimedia content by combining weather summaries with images and audio, culmniating in some kind of video forecast.

The core of our project is built around the WeatherSummaryApp class, which follows object-oriented programming principles. This class integrates several APIs, such as Google Maps for geolocation, Open-Meteo for weather data, and OpenAI for generating text, audio, and images. The Python file WeatherSummaryApp.py includes the full implementation of this class and its methods.

## Features
1. **Fetch Coordinates**: Retrieves the geographical coordinates (latitude and longitude) of a city using the Google Maps API.
2. **Fetch Weather Data**: Retrieves hourly and daily weather data for the specified coordinates using the Open-Meteo API.
3. **Generate Weather Summary**: Creates a concise and engaging weather report using OpenAI's GPT model.
4. **Text-to-Audio Conversion**: Converts the generated weather summary text to speech using OpenAI's text-to-speech API.
5. **Image Generation**: Generates an image illustrating the current weather conditions using OpenAI's DALL-E model.
6. **Video Creation**: Combines the generated audio and image into an MP4 video file using the MoviePy library.

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

## Installation and Setup

### Prerequisites
- Python 3.8
- API keys for Google Maps and OpenAI. If you need to connect to an API key with credits to access OpenAI, please get in touch with our team member Nikola (nikola.bulatovic@student.unisg.ch).

### Required Libraries
Install the required Python libraries using pip:

```
pip install requests requests_cache pandas retry_requests openai moviepy
```

### Clone the Repository
```bash
git clone https://github.com/yourusername/ai-audio-weather.git
cd ai-audio-weather
```

## Usage
-----

1. Obtain API Keys:
   - Get a Google Maps API key from the Google Cloud Console.
   - Get an OpenAI API key from the OpenAI API Keys page. If you need to connect to an API key with credits to access OpenAI, please get in touch with our team member Nikola (nikola.bulatovic@student.unisg.ch).


2. Initialize the Application:
   Create an instance of the WeatherSummaryApp class by providing your Google Maps and OpenAI API keys.

3. Run the Application:
   Call the `run` method with the name of the city you want to generate the weather summary for.

### Example Usage

```python
if __name__ == "__main__":
    google_maps_key = 'YOUR_GOOGLE_MAPS_API_KEY'
    openai_key = 'YOUR_OPENAI_API_KEY'
    app = WeatherSummaryApp(google_maps_key, openai_key)
    city = input("Enter the city for the weather summary: ")
    app.run(city)
```

## Error handling
The application includes error handling to manage issues such as invalid city names, API request failures, and other exceptions. If an error occurs, the user will be prompted to run the application again with a valid city name.

## Contribution
Contributions to improve the application are welcome. Please fork the repository, make your changes, and submit a pull request.


## Declaration of aiding material
   - We used ChatGPT to help us correct our code.
   - StackOverflow references were made in the code if used as an inspiration.