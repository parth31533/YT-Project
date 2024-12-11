# YouTube Channel Video Transcript Extractor  

## Overview  
This Python script extracts video transcripts from a specified YouTube channel using the YouTube Data API and the YouTube Transcript API. The transcripts are saved as text files and archived in a ZIP file. The script also provides yearly statistics for successfully transcribed and failed videos.  

## Features  
- Fetches all video links, titles, and release dates from a YouTube channel.  
- Extracts transcripts for videos with subtitles available.  
- Saves transcripts as individual `.txt` files and archives them in a ZIP file.  
- Provides statistics of transcripts by year, including success and failure counts.  

## Prerequisites  

1. **YouTube Data API Key**  
   - Obtain an API key from [Google Cloud Console](https://console.cloud.google.com/).  
   - Replace the placeholder in the script:  
     ```python
     API_KEY = "YOUR_YOUTUBE_API_KEY"
     ```

2. **Python Libraries**  
   Install the required libraries using pip:  
   ```bash
   pip install google-api-python-client youtube-transcript-api


How to Use
1. Clone the Repository
Clone this repository to your local machine:

bash
Copy code
git clone https://github.com/<parth31533>/<YT-Project>.git  
cd <YT-Project>

2. Update the Script
Open the script and make the following updates:

Replace the API_KEY variable with your YouTube Data API key.
Replace the channel_id variable in the script with the ID of the desired YouTube channel:
python
Copy code
channel_id = "UCsfp0zw1hNxpy_wDig8oExA"  # Replace with your channel ID

3. Run the Script
Run the script in your terminal or IDE:

bash
Copy code
python your_script_name.py

Output
Transcripts are saved in a ZIP file named Josh_Transcripts.zip in the current working directory.
The script logs statistics for transcripts generated per year in the terminal.
Adaptability
Changes for Customization:
YouTube Channel ID
Replace the channel_id variable with the desired channel's ID.
Use tools like YouTube Channel Finder if needed.

Output File Naming
Modify the sanitize_filename function in the script to match specific naming conventions or remove unwanted patterns from video titles.

Transcript Languages
By default, the script fetches English transcripts. Modify the get_transcript method to specify other languages using language_codes.

API Rate Limits
Be aware of YouTube Data API's quota limitations. To avoid exceeding the quota, use multiple API keys or optimize requests.

Additional Metadata
Extend the script to fetch and save other metadata (e.g., video duration, views, or descriptions) alongside transcripts.

Limitations
Transcripts are only available for videos with subtitles enabled.
Some videos may fail due to restricted access or missing transcripts.
API quota limits can restrict the number of requests per day.
License
This project is licensed under Apache 2.0.

Author
Parth Patel
