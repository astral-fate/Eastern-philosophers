# Eastern Philosophers: An Interactive Exploration

This project is a web-based, interactive application designed to explore the lives, works, and influences of prominent philosophers and thinkers in the Islamic world. It provides a visually engaging and informative journey through the history of Islamic thought, from the early days of "kalam" to the great minds of the Golden Age and beyond. The application presents the data in three distinct, interactive formats: a chronological timeline, a categorized view, and a dynamic influence map.

## Features

* **Interactive Timeline:** A scrollable, chronological timeline of philosophers, allowing users to visualize the historical progression of thought and the eras in which these thinkers lived.
* **Categorized View:** Philosophers are grouped by their primary fields of thought (e.g., "Falsafa," "Kalam," "Sufism," "Science & Natural Philosophy"), making it easy to explore specific intellectual traditions.
* **Influence Map:** A dynamic, force-directed graph that visually represents the intellectual connections between philosophers, showing who influenced whom.
* **Detailed Information:** Clicking on any philosopher in any of the views opens a modal window with detailed information, including their biography, key areas of interest, major works, and who they were influenced by.
* **Responsive Design:** The application is designed to be fully responsive and accessible on a wide range of devices, from desktops to mobile phones.

## Technologies Used

* **HTML5:** For the structure and content of the web page.
* **CSS3:** For styling and layout, including a modern, clean design and responsive media queries.
* **JavaScript (ES6):** For the core application logic, including data handling, DOM manipulation, and interactivity.
* **D3.js (v7):** A powerful JavaScript library used to create the dynamic and interactive influence map.

## Project Structure

The repository contains the following files:

* `index.html`: The main HTML file that defines the structure of the application.
* `style.css`: The stylesheet that contains all the CSS rules for the application's appearance.
* `script.js`: The JavaScript file that contains the data and the logic for all the interactive features.

## How It Works

The application's functionality is driven by the `script.js` file, which contains a comprehensive array of philosopher objects. Each object includes detailed information about a specific philosopher.

When the page loads, the script dynamically generates the content for each of the three views:

1.  **Timeline View:** The script sorts the philosophers chronologically and renders them as cards along a central timeline.
2.  **Categories View:** The script identifies all unique categories and groups the philosophers accordingly, displaying them in expandable category cards.
3.  **Influence Map View:** The script processes the `influence` property for each philosopher to create a network of nodes (philosophers) and links (influences). D3.js is then used to render this network as a force-directed graph.

Event listeners are used to handle user interactions, such as switching between tabs, clicking on philosopher cards to open the detailed modal view, and interacting with the nodes on the influence map.
