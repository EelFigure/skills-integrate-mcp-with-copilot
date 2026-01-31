# Pull Request

## Description
Resolves #3: Hard to change activities

This PR moves the hardcoded activities list from the Python code into a dedicated `activities.json` file, making it much easier for teachers to manage activities without fear of breaking the application.

## Changes
- Created `src/activities.json` containing all 9 extracurricular activities
- Updated `src/app.py` to load activities from JSON file using a new `load_activities()` function
- Removed hardcoded activities dictionary from Python code

## Benefits
✅ Teachers can now safely edit activities without touching Python code  
✅ Reduces risk of accidental code breakage  
✅ Easier maintenance and updates  
✅ Better separation of configuration from code  

## Testing
The application loads all activities correctly from the JSON file and the API endpoints function as expected.
