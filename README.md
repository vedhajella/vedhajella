
```markdown
# Live Cricket Score Application

This is a Python-based desktop application that displays live cricket scores and match summaries using a graphical user interface (GUI) built with Tkinter. The app scrapes live data from Cricbuzz and also provides features for sending score updates via SMS using Twilio and desktop notifications using Plyer.

## Features

- **Live Match Updates**: Get real-time cricket scores, summaries, and match information directly within the app.
- **User Interface**: Easy-to-use interface built using Tkinter, with match options available via a dropdown menu.
- **Desktop Notifications**: Displays real-time notifications with match details.
- **SMS Notifications**: Sends SMS notifications of match scores to a specified phone number using Twilio.

## Installation

### Prerequisites

- Python 3.x
- Required Python libraries:
  - `tkinter`
  - `Pillow`
  - `BeautifulSoup`
  - `requests`
  - `plyer`
  - `twilio`

You can install the necessary packages using pip:

```bash
pip install tkinter Pillow beautifulsoup4 requests plyer twilio
```

### Clone the Repository

```bash
git clone https://github.com/yourusername/cricket-score-app.git
cd cricket-score-app
```

### Setup Twilio Credentials

To enable SMS notifications, you need to set up your Twilio credentials:

1. Replace the placeholder values in the script with your Twilio `account_sid`, `auth_token`, and Twilio phone number.

```python
self.account_sid = 'your_account_sid'
self.auth_token = 'your_auth_token'
self.twilio_phone_number = '+your_twilio_number'
self.target_phone_number = '+recipient_phone_number'
```

## How to Run

Run the application with the following command:

```bash
python main.py
```

## Usage

1. Start the application, and you will see a window showing the available live matches.
2. Select a match from the dropdown menu.
3. Click the "Check Score" button to view match details and receive notifications.

## Screenshots

![App Screenshot](screenshot.png) <!-- Add a screenshot if you have one -->

## Technologies Used

- **Tkinter**: For creating the graphical user interface.
- **BeautifulSoup and Requests**: For web scraping live cricket scores from Cricbuzz.
- **Plyer**: For sending desktop notifications.
- **Twilio**: For sending SMS notifications.

## Future Enhancements

- Add more detailed statistics like player information, wickets, and overs.
- Add support for multiple notification channels (e.g., email, push notifications).
- Improve error handling and user feedback.

## Contributing

Feel free to fork this repository and contribute via pull requests. If you find any bugs or want to request features, please open an issue.
