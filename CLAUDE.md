# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a single-file HTML application showcasing the Coast to Coast Walk 2025 route across Northern England (St Bees to Robin Hoods Bay). The project is a self-contained webpage with embedded CSS styling and JavaScript functionality.

## File Structure

- `coast_to_coast_website.html` - Complete standalone webpage with inline CSS and JavaScript

## Technology Stack

- **HTML5** - Document structure and semantic markup
- **CSS3** - Styling with modern features (flexbox, grid, gradients, backdrop-filter)
- **Vanilla JavaScript** - Interactive functionality and map integration
- **Leaflet.js** (CDN) - Interactive mapping via OpenStreetMap
- **External CDN Dependencies**:
  - Leaflet CSS: `https://cdnjs.cloudflare.com/ajax/libs/leaflet/1.9.4/leaflet.min.css`
  - Leaflet JS: `https://cdnjs.cloudflare.com/ajax/libs/leaflet/1.9.4/leaflet.min.js`

## Architecture

### Core Components

1. **Hero Section** (`lines 311-329`) - Title, description, and walk statistics
2. **View Toggle** (`lines 331-334`) - Switch between timeline and map views
3. **Interactive Map** (`lines 336-344`) - Leaflet map with route markers and popups
4. **Daily Timeline** (`lines 345-839`) - Detailed itinerary with accommodation info
5. **JavaScript Map Engine** (`lines 848-1181`) - Route coordinates, accommodation data, and map controls

### Data Structure

- **Route Coordinates** (`lines 852-870`) - 17 GPS waypoints defining the walking route
- **Accommodations Array** (`lines 872-1043`) - Detailed lodging information including coordinates, contact details, and daily notes

### Key JavaScript Functions

- `initMap()` - Initialize Leaflet map with route polyline and markers
- `showTimeline()` - Display daily itinerary view
- `showMap()` - Display interactive map view

## Development Notes

- No build process - direct file editing and browser refresh
- Responsive design with mobile breakpoints at 768px
- Modern CSS features may require recent browser versions
- Map requires internet connectivity for OpenStreetMap tiles
- Self-contained with no local dependencies beyond the HTML file

## Testing

Open `coast_to_coast_website.html` directly in a web browser. Test both desktop and mobile views, and verify map functionality with internet connection.