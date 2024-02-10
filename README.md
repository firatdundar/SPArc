# SPArc: Single Line Protein Architecture
Welcome to SPArc, a project designed to represent protein architecture in a single-line format. This tool takes a protein ID as input and generates a 2D backbone visualization, displaying protein domains as rectangles along a single line. The visualization prioritizes simplicity, offering an intuitive representation of protein domains.

## Contents
- `index.html`: Main HTML file for the search page.
- `resultPage.html`: HTML file for visualizing the protein backbone.
- `server.js`: JavaScript file responsible for processing protein data.

## Setup

1. Clone the repository to your local machine:

    ```bash
    git clone https://github.com/your-username/SPArc.git
    ```

2. Navigate to the project directory:

    ```bash
    cd SPArc
    ```

3. Install Node.js dependencies:

    ```bash
    npm install
    ```

4. Start the data processor:

    ```bash
    node server.js
    ```

5. Open the `index.html` file in your web browser.

## Usage

1. Open `index.html` in your web browser.
2. Enter a protein ID in the search bar.
3. Click the search button to generate the 2D backbone visualization.
4. Explore the initial summary of protein domains displayed on the visualization page (`resultPage.html`). 

## Explore Detailed Domains

- Upon generating the 2D backbone visualization, an initial summary of protein domains is presented, combining information from various databases to provide a comprehensive overview.
- To explore detailed information for each domain, click the buttons associated with each domain. Each button corresponds to a different database.

## Configuration

Customize the order of domain display by modifying the code in `resultPage.html`. Adjust the `rankingArray` array to reflect your preferred ranking.

```javascript
// Example: Adjust the order based on ranking
let rankingArray = [
    "pfam",
    "cathgene3d",
    "ssf",
    "panther",
    "cdd",
    "profile",
    "smart",
    "ncbifam",
    "prosite",
    "prints",
    "hamap",
    "pirsf",
    "sfld"
];
```
## Dependencies

SPArc relies on Node.js for data processing. Ensure Node.js is installed on your machine before running the project. If Node.js is not installed, you can download it from [nodejs.org](https://nodejs.org/).

SPArc itself does not have additional external dependencies.

## Notes

- The visualization represents protein domains as rectangles along a single line, offering a simplified view of protein architecture.
- Ensure an active internet connection for fetching protein data from specified databases.
- Feel free to reach out for further assistance or customization. Explore the world of proteins with SPArc!
