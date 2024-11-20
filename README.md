# PoC Bypass SiteGround AI Antibot Protection

This is a proof-of-concept (PoC) script designed to bypass SiteGround's AI-powered antibot protection. The script utilizes Selenium WebDriver and Python's `requests` library to automate a browser session on Firefox.

## Usage

To use this script, you'll need to have the following prerequisites installed:

- Python 3.x
- Selenium WebDriver for Firefox
- requests library
1. Clone or download this repository.
2. Install the required dependencies by running `pip install -r requirements.txt`.
3. Update the `TARGET` variable in the script with your desired target URL.
## Usage Options

The script accepts two command-line arguments:

- `-t, --target`: The target URL to test against SiteGround's antibot protection.
- `-ua, --user-agent`: A custom User-Agent string (optional).
To run the script, execute it using Python:
```bash
python bypass_sitesground_antibot.py -t <TARGET_URL> [-ua <USER_AGENT_STRING>]
```

### Example Output

If the script is successful in bypassing SiteGround's antibot protection, you'll see the following output:
```bash
Valid Cookie ID and User-Agent

Use in your future requests:
Cookie: _I_: <COOKIE_ID>
Header: User-Agent: <USER_AGENT>

Example:
- curl -I "<TARGET_URL>" -H "Cookie: _I_=<COOKIE_ID>" -H "User-Agent: <USER_AGENT>"
```
##  Notes

- This script is for educational purposes only and should not be used to engage in malicious activities.
- SiteGround's antibot protection may change or evolve over time, making this PoC obsolete. Use at your own risk!
