<b>Description</b><br>
This script is designed to be run in the browser's console on the Tinder website to unblur the images of users who have liked you in the "Fast Match" section. Normally, Tinder blurs these images, and you need to swipe or pay for a premium service to see them clearly. This script bypasses the blur by fetching the unblurred images directly from Tinder's API and replacing the blurred images on the webpage.

<b>How It Works</b><br>

1. <b>Fetch Data from Tinder API</b><br>
   The script sends a request to the Tinder API to retrieve data about users who have liked you. It includes an authentication token (`X-Auth-Token`) stored in your browser's local storage.
   
2. <b>Extract Teaser Data</b><br>
   The response from the API includes a list of teasers, each containing information about a user who liked you. This data includes their unique user ID and photo information.

3. <b>Unblur the Images</b><br>
   The script selects the DOM elements corresponding to the blurred images in the "Fast Match" section.
   It then constructs the URL of the unblurred image using the user ID and photo ID from the API response and sets this URL as the background image of the corresponding DOM element, effectively replacing the blurred image with the unblurred one.

<b>How to Use the Script</b><br>

1. <b>Navigate to Tinder Web</b><br>
   Open your web browser and go to the Tinder website (https://tinder.com/).

2. <b>Open Developer Tools</b><br>
   Right-click anywhere on the page and select "Inspect" or press `Ctrl+Shift+I` (Windows/Linux) or `Cmd+Option+I` (Mac) to open the Developer Tools.
   Go to the "Console" tab within the Developer Tools.

3. <b>Paste and Run the Script</b><br>
   Copy the entire script provided below.
   Paste the script into the console and press `Enter` to execute it.

4. <b>View the Unblurred Images</b><br>
   After running the script, the previously blurred images in the "Fast Match" section should now be unblurred, and you can see the users who have liked you without needing to swipe or upgrade your account.

<b>Notes</b><br>

<b>Use Responsibly</b><br>
This script is intended for educational purposes and security testing. Using it to bypass Tinder's paid features might violate Tinder's terms of service, potentially leading to your account being suspended or banned. Use it at your own risk.

<b>Browser Compatibility</b><br>
The script is designed to work on modern web browsers that support JavaScript ES6 features like async/await.

<b>API Token Requirement</b><br>
The script requires an active Tinder session with a valid API token stored in the browser's local storage. Ensure you are logged into Tinder before running the script.

<b>Disclaimer</b><br>
This script is provided for educational and security testing purposes only. The author of this script is not responsible for any misuse or consequences that arise from its use.

By using this script, you acknowledge that:

It may violate Tinder's terms of service.
Using this script to bypass Tinder's premium features could result in your account being suspended or permanently banned by Tinder.
The author is not liable for any actions taken by Tinder or other third parties as a result of your use of this script.
Use this script at your own risk, and consider the potential consequences before running it.
