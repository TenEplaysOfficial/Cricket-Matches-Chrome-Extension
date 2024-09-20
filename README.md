# Cricket Matches Chrome Extension

A simple Chrome extension that displays ongoing cricket matches globally or filtered by series types such as ODI, IPL, or T20. It fetches live match data from the Free Cricket Data API (cricketdata.org) and presents it in a user-friendly popup. You can filter matches by specific series using the series ID.

## Features
- Display ongoing global cricket matches.
- Filter matches by series type (ODI, IPL, T20, etc.).
- Responsive and easy-to-use design.

## Setup

### 1. Clone the repository

```bash
git clone https://github.com/TenEplays/Cricket-Matches-Chrome-Extension.git
cd Cricket-Matches-Chrome-Extension
```

### 2. Add Your API Key

Replace the API key in the `script.js` file with your own from [cricketdata.org](https://cricketdata.org/).

```javascript
const apiKey = 'YOUR_API_KEY_HERE';
```

### 3. Load the Extension in Chrome

1. Open Chrome and go to `chrome://extensions/`.
2. Enable "Developer Mode" in the top right corner.
3. Click "Load unpacked" and select the folder where you cloned the repository.

### 4. Use the Extension

Click on the extension icon to view ongoing cricket matches or filter them by series type.

## API Filtering

To filter matches by series type like ODI, IPL, or T20, you can modify the API request in `script.js` and filter results using the `series_id`. For example:

```javascript
const filteredMatches = matchesList.filter(match => match.series_id === 'desired_series_id');
```

## Files

- `manifest.json`: Configures the Chrome extension.
- `index.html`: The popup displaying the cricket matches.
- `styles.css`: Styles for the popup.
- `script.js`: Fetches and processes match data from the Free Cricket Data API.

## Sample Output

The extension will display ongoing cricket matches in a list format:

```
India vs Australia, Live
England vs South Africa, Scheduled
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

*Stay connected! Follow me on [Socials](https://linktr.ee/tenegames).*