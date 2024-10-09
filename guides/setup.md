# Setup Guide

This guide will help you set up the development environment for the Campus Resource and Event Management App.

## Setting Up the Development Environment

### Node.js

1. **Install Node.js**:
   - If you don't already have Node.js on your machine, download it [here](https://nodejs.org) before continuing with the next steps.
   - You can check if you already have it by running the following command in your terminal:
     ```bash
     node --version
     ```

2. **Clone the Repository**:
   - If you haven't already, clone this repository:
     ```bash
     git clone <repository-url>
     ```
   - If you have the repository cloned already, make sure to do a `git pull` to get the latest changes.

3. **Install Node.js Modules**:
   - While inside the repository folder, run:
     ```bash
     npm install
     ```
   - This will install all necessary dependencies.

4. **Running the Frontend Development Server**:
   - To start the frontend development server, run:
     ```bash
     npm run dev-svelte
     ```
   - This will spin up a local development server, serving the web page at the URL shown in the terminal after running the command. Any changes you make will automatically reload the web page. For certain types of changes, you may need to manually refresh the page.

### Python

1. **Install Python**:
   - If you don't already have Python installed, download it [here](https://www.python.org/downloads/). Also, install Python's package manager (pip) if you don't already have it.

2. **Set Up the Python Environment and Install Packages**:
   - **macOS/Linux Instructions**:
     ```bash
     cd ./api
     python3 -m venv .venv
     . .venv/bin/activate
     pip install Flask
     ```

   - **Windows Instructions**:
     ```bash
     cd .\api
     py -3 -m venv .venv
     .venv\Scripts\activate
     pip install Flask
     ```

3. **Running the Backend Development Server**:
   - To get the Python server up and running, execute:
     ```bash
     npm run dev-api
     ```
   - You can now access the example page on the frontend, and the "Get Data From Server" button should now work.

### Running the Frontend and Backend Development Servers Simultaneously

- To run both servers at the same time, run the following command:
  ```bash
  npm run devall
  ```


### Summary
This Markdown format provides clear sections and step-by-step instructions for setting up the development environment. Feel free to modify any part of it or let me know if you need any changes or additional information!
