# Badger Bodger - Development Instructions

## Project Overview
This project creates a web application for generating badges for the Badger device with an RP2350 running Micropython. The website allows users to enter their information, preview how it will appear on the badge, export as a PNG file, and send the data directly to the badge over web serial.

## File Structure
- `app/index.html` - Main entry point for the application

## Implementation Guidelines

### HTML Structure
- Create a responsive single-page layout
- Include form elements for: GitHub handle, Firstname, Surname, Title
- Include a canvas element with dimensions 296x128 pixels
- Add buttons for generating PNG and connecting to the badge via web serial

### CSS Guidelines
- Use a clean, minimal design
- Use Primer CSS for styling
- Ensure mobile responsiveness
- Use CSS variables for consistent theming
- Follow BEM naming convention for classes

### JavaScript Guidelines
- Use vanilla JavaScript (no framework dependencies)
- keep the javascript code and the CSS in the same index.html file
- Handle form validation and real-time canvas preview
- Implement proper error handling for serial communication
- Use async/await for asynchronous operations

### Canvas Implementation
- Default badge background should be white
- Text should be black
- Use appropriate font sizes to ensure readability on the actual device
- Implement live preview that updates as user types

### Web Serial Implementation
- Follow the Web Serial API standard
- Include clear connection/disconnection UI
- Implement proper error handling
- Format data appropriately for the Micropython implementation on the RP2350

## Development Tasks
1. Create the basic HTML structure
2. Add form input with live preview updates
3. Add Web Serial communication with the RP2350
6. Implement the badge canvas preview
4. Implement PNG export functionality
5. Test all functionality
7. Optimize for deployment on GitHub Pages

## Deployment
- The application will be deployed using GitHub Pages
- Ensure all assets are properly linked with relative paths
- Verify the site works correctly when deployed
