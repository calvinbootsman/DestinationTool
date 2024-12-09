# Booking.ipynb

## Overview
`booking.ipynb` is a Jupyter Notebook designed to handle the booking process for the Destination Tool project. This notebook includes code for managing bookings, processing user inputs, and generating booking confirmations.

## Requirements
To run `booking.ipynb`, you need the following:
- Python 3.x
- Jupyter Notebook
- Required Python libraries (listed in `requirements.txt`)

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/calvinbootsman/DestinationTool.git
    ```
2.  Install the required libraries:
    ```bash
    pip install -r requirements.txt
    ```

## Usage
1. Open Jupyter Notebook from the command line:
    ```bash
    jupyter notebook
    ```
2. In the Jupyter Notebook interface, navigate to the `booking.ipynb` file and open it.
3. **Cell 1** will generate a file containing a list of nearby cities, given the minimum and maximimum distance from a given start location. 
4. **Cell 2** will read the file created by **cell 1** into a pandas frame. This frame will then be filtered out keeping only the selected countries. 
5. **Cell 3** Will fetch hotel data from booking.com. Needs to be run in order to perform the search.
6. **Cell 4** will perform a multithreaded search to fetch hotel data for multiple cities in parallel. This may get you blocked from booking.com. Be careful.
7. **Cell 5** will perform a single-threaded search to fetch hotel data for multiple cities sequentially. This may get you blocked from booking.com. Be careful.
8. **Cell 6** will create a list of unique cities from the fetched hotel data, which can be loaded into Google Maps.
