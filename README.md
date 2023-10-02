# Weather Alert System with Twilio Integration

## Table of Contents

- [Description](#description)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)

## Description

This Python project utilizes the OpenWeatherMap API to provide weather alerts via SMS using Twilio. It checks the hourly weather forecast and sends an SMS notification if rain is expected within the next 12 hours. This project serves as a simple weather notification system.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.x installed
- Twilio account SID and auth token
- OpenWeatherMap API key
- Latitude and longitude coordinates for your location
- Environmental variables set for `OWM_API_KEY` and `AUTH_TOKEN`

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/ozesince02/RainAlert-OpenWeather-Twilio.git
   ```

2. Install the required Python packages using pip:

   ```bash
   pip install requests twilio
   ```

## Usage

To use this weather alert system, follow these steps:

1. Set the environmental variables for `OWM_API_KEY` and `AUTH_TOKEN` with your OpenWeatherMap API key and Twilio auth token.

2. Configure the `weather_params` dictionary with your latitude and longitude coordinates.

3. Replace `"YOUR TWILIO VIRTUAL NUMBER"` with your Twilio virtual number and `"YOUR TWILIO VERIFIED REAL NUMBER"` with the recipient's phone number in the `message.create()` method.

4. Run the script:

   ```bash
   python weather_alert.py
   ```

The script will check the weather forecast and send an SMS notification if rain is expected within the next 12 hours.

## Configuration

You need to configure the following in the `weather_alert.py` script:

- `api_key`: Your OpenWeatherMap API key.
- `account_sid`: Your Twilio account SID.
- `weather_params`: Latitude and longitude coordinates of your location.
- Twilio virtual number and recipient's real number in the `message.create()` method.

## Contributing

Contributions are welcome! If you want to improve this project, please:

1. Fork the repository.
2. Create a new branch for your feature: `git checkout -b feature-name`
3. Make your changes and commit them: `git commit -m 'Add feature-name'`
4. Push your changes to your fork: `git push origin feature-name`
5. Create a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
