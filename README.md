# Proxy Automation Bot

A Python-based application with a GUI for managing browser automation with unique proxy configurations.

## Features

- Load proxies from CSV/Excel files or enter them manually (supports format: hostname:port:username:password)
- Open multiple browser instances (Chrome/Edge) with different proxy configurations
- Run browsers with or without proxies using a simple checkbox option
- Configure thread count, run duration, and target URL
- Page scrolling with configurable duration to simulate user activity
- Real-time monitoring through an activity log
- Save and load configuration settings
- User-agent rotation to avoid detection
- Headless mode option for resource efficiency
- Gradual browser shutdown to prevent system slowdowns

## Requirements

- Python 3.7 or higher
- Required packages (listed in requirements.txt)

## Installation

1. Install the required Python packages:

```
pip install -r requirements.txt
```

2. Run the application:

```
python proxy_automation.py
```

## Usage

### Proxy Management

- **Load from file**: Select a CSV or Excel file containing proxy information
  - Supports format: hostname:port:username:password (e.g., `aus.360s5.com:3600:38783650-zone-custom-region-US:nEIaeYpg`)
- **Manual entry**: Enter details for individual proxies
- **Enable/Disable Proxies**: Toggle the "Use Proxies" checkbox in Settings

### Settings

- **Target URL**: Set the website to open in each browser instance
- **Browser Type**: Choose between Chrome and Edge
- **Thread Count**: Define how many browser instances to run simultaneously
- **Run Duration**: Set how long each browser instance should remain open
- **Auto Close**: Choose whether to automatically close browsers after the specified duration
- **Headless Mode**: Run browsers without a visible UI to save resources
- **Rotate User Agents**: Automatically change browser user agent strings to avoid detection
- **Use Proxies**: Enable or disable proxy usage
- **Enable Page Scrolling**: Activate automatic page scrolling to simulate real user activity
- **Scroll Duration**: Set how long the application should scroll each page

### Running the Bot

1. Configure your settings and load proxies if needed
2. Click "Start Automation" to begin
3. Monitor progress in the Activity Log tab
4. Use "Stop Automation" to gradually shut down all browser instances

## Note on Proxy Usage

- Each browser profile uses a unique proxy from the available pool
- Once a proxy is used for a profile, it won't be reused in the same session
- The application tracks active and used proxies separately

## Developer

Developed by Arslan Malik
- [GitHub](https://github.com/arslanmalik)
- [Upwork](https://www.upwork.com/freelancers/arslanmalik)

## License

This project is free to use and modify.
