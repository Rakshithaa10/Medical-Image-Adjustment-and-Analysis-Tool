# Medical-Image-Adjustment-and-Analysis-Tool
This project reflects the core functionalities, including image adjustments (brightness, contrast) and the capability to work with medical images (e.g., DICOM support). 
This React code creates a Medical Image Analysis Tool application where users can upload images, view them, and adjust their brightness and contrast. Here's a breakdown of its components, logic, and functionality.
Overview

This project is a Medical Image Analysis Tool, a web-based application designed to assist healthcare lab technicians in analyzing medical images. The tool provides an intuitive interface for uploading, viewing, and performing basic adjustments on medical images, such as brightness and contrast. Future expansions include support for DICOM images, commonly used in medical imaging.

Features

Upload Images: Upload PNG images and preview them in a gallery.

Image Viewer: Select an image to view and adjust its properties.

Image Adjustments: Adjust brightness and contrast using sliders.

Gallery: View uploaded images in a thumbnail gallery for easy selection.

Animations: Smooth transitions using animations for better user experience.

Expandability: Placeholder for supporting DICOM file uploads and real-world measurement unit conversions.

Project Structure

The application is built using ReactJS with a focus on modularity, responsiveness, and clean code practices. Below is an outline of the key components and functionality:

1. State Management

State is managed using the useState and useEffect hooks for handling:

Uploaded images.

Selected image for detailed viewing.

Brightness and contrast adjustment values.

2. File Upload

PNG File Upload: Allows users to upload standard image formats like PNG. These files are converted to Base64 strings and stored in state for rendering.

DICOM File Upload: Placeholder functionality for future development to support DICOM files and metadata extraction.

3. Image Adjustments

Image brightness and contrast are dynamically adjusted by applying CSS filters using JavaScript. The adjustments are applied in real-time via the filter property of the selected image.

4. Reusable Components

Reusable components like Card and Button are used to improve modularity and readability of the code. These components enhance the user interface and improve maintainability.

5. Styling

The project uses Tailwind CSS for consistent and responsive styling. Utility-first classes ensure rapid and clean UI development.

6. Animations

Smooth animations are implemented using the Framer Motion library to improve user experience by adding visual appeal to transitions and component loading.

7. Future Enhancements

Full support for DICOM file parsing and display of metadata.

Real-world measurement unit conversions based on pixel resolution.

Advanced image manipulation features like cropping, rotating, and annotation.

Setup and Installation

Follow these steps to set up and run the application on your local machine:

Prerequisites

Node.js (v16 or higher)

npm (v8 or higher) or Yarn

Installation Steps

Clone the repository:

git clone https://github.com/your-repo/medical-image-analysis-tool.git
cd medical-image-analysis-tool

Install dependencies:

npm install

Development Server

Run the application in development mode:

npm start

Opens the application on http://localhost:3000/.

Watches for changes in the source files and reloads automatically.

Building for Production

To build the application for production:

npm run build

Outputs a minified and optimized production build in the build/ directory.

Ready to be deployed to a static hosting service or a web server.

Serving Production Build Locally

To serve the production build locally:

npm install -g serve
serve -s build

Serves the application at http://localhost:5000/ by default.

Code Walkthrough

App.js

The App.js file serves as the entry point for the application and contains:

State Management: Handles image uploads, selected image, and adjustments.

Image Upload Handlers: Functions to process PNG and DICOM files.

Image Adjustments: Dynamically applies brightness and contrast filters to the selected image.

Gallery: Displays uploaded images with the ability to select an image for detailed viewing.

Components

Card

A reusable container for displaying image thumbnails with consistent styling.

Button

A reusable button component for actions like removing selected images.

Dependencies

ReactJS: Frontend framework for building the UI.

Framer Motion: For smooth animations.

Tailwind CSS: Utility-first CSS framework for styling.

License

This project is licensed under the MIT License. See the LICENSE file for details.

