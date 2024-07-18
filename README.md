# GitHub Repositories Viewer

This project is a simple GitHub Repositories Viewer built with Next.js. It fetches and displays a list of repositories, allowing users to search, sort, and paginate through the list.

## Features

### 1. Fetch Repositories
- Fetches a list of repositories from GitHub using the `fetchRepositories` function.

### 2. Search Functionality
- Allows users to search for repositories by name.
- Updates the displayed list of repositories in real-time as the user types.

### 3. Sort Functionality
- Allows users to sort repositories based on:
  - **Stars**: Sorts repositories by the number of stars in descending order.
  - **Last Updated**: Sorts repositories by the last updated date in descending order.

### 4. Pagination
- Displays a limited number of repositories per page (default is 5).
- Provides **Previous** and **Next** buttons to navigate between pages.
- Displays the current page number and the total number of pages.

### 5. User Profile
- Displays a user profile section with a profile image and username.
- Includes an **Edit profile** button (non-functional, for UI purposes only).

### 6. Repository List
- Displays a list of repositories with the following details:
  - **Name**: The name of the repository, which is a clickable link to the repository's details page.
  - **Stars**: The number of stars the repository has received.
  - **Description**: A brief description of the repository.
  - **Last Updated**: The relative time since the repository was last updated.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/github-repos-viewer.git
## Install the dependencies:
npm install
## Start the development server:
npm run build
npm run dev

## Usage
Open your browser and navigate to http://localhost:3000.
Use the search bar to find specific repositories.
Use the sort dropdown to sort the repositories by stars or last updated date.
Navigate between pages using the Previous and Next buttons.

## Code Overview

State Management
repos: Stores the list of all fetched repositories.
filteredRepos: Stores the list of repositories filtered based on the search term and sort option.
searchTerm: Stores the current search term.
sortOption: Stores the current sort option.
currentPage: Stores the current page number for pagination.

## Components

Home: The main component that contains the user profile section, search and sort functionality, and the repository list with pagination controls.
Utility Functions
fetchRepositories: Fetches the list of repositories from GitHub.
handleSearch: Filters the repositories based on the search term.
handleSort: Sorts the repositories based on the selected sort option.
goToPreviousPage: Decrements the current page number.
goToNextPage: Increments the current page number.
