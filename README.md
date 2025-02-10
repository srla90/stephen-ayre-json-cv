# Stephen Ayre - JSON CV

Welcome to my JSON-based CV! This file is designed to showcase my technical expertise in a format that's both unique and highly flexible.

## What Is This?
This JSON file (`stephen_ayre_cv.json`) contains all the structured information about my professional experience, skills, projects, and more. It's designed to:
- Demonstrate my technical abilities in working with structured data formats.
- Be easily parsed, visualized, or extended by technical audiences.

## How to Use
### Option 1: View the JSON Directly
If you're familiar with JSON, you can open the `stephen_ayre_cv.json` file in:
- A code editor like VS Code, Sublime Text, or Notepad++.
- An online JSON viewer such as [JSONViewer](https://jsonviewer.stack.hu/) or [JSON Formatter](https://jsonformatter.curiousconcept.com/).

### Option 2: Render It Programmatically
You can use the file in your own program to render the CV in various formats (e.g., HTML, PDF). Here's an example in Python:

#### Python Script Example:
```python
import json

# Load JSON CV
with open("stephen_ayre_cv.json", "r") as file:
    cv_data = json.load(file)

# Print Summary
print(f"{cv_data['personal_details']['name']} - {cv_data['personal_details']['role']}")
print(f"Contact: {cv_data['personal_details']['contact']['email']} | {cv_data['personal_details']['contact']['phone']}")
print("\nProfessional Summary:")
print(cv_data['professional_summary'])

