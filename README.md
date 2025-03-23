# Startup Pitch Evaluation AI

## Overview
This project implements an AI-driven system to evaluate startup pitch sections using Hugging Face's language models. The model assesses different sections of a startup pitch and provides scores, feedback, strengths, and weaknesses.

## Features
- Loads pitch data from a JSON file.
- Preprocesses and extracts key sections.
- Uses Hugging Face API for text evaluation and scoring.
- Identifies strengths and weaknesses in the pitch.
- Outputs an overall pitch score with detailed feedback.

## Installation
### Prerequisites
Ensure you have the following installed:
- Python 3.x
- Requests library

### Install Dependencies
```sh
pip install requests
```

## Usage
### Upload Dataset
Run the script and upload a JSON file containing startup pitch data.

### Execute Evaluation
The script automatically:
1. Loads and preprocesses the dataset.
2. Identifies key sections of the pitch.
3. Evaluates sections using Hugging Face API.
4. Calculates an overall pitch score.
5. Provides feedback on strengths and weaknesses.

### Running the Script
```sh
python startup_pitch_evaluation.py
```

## Input Format
The dataset should contain startup pitch details such as:
- Name
- Overview
- Stage
- Industry
- Cheque_range (Investment range)
- Type
- Global_HQ
- Countries

Example JSON Structure:
```json
[
  {
    "Name": "Startup A",
    "Overview": "Innovative AI-powered platform for data analytics.",
    "Stage": "Seed",
    "Industry": "Technology",
    "Cheque_range": "$100K - $500K",
    "Type": "SaaS",
    "Global_HQ": "USA",
    "Countries": "Global"
  }
]
```

## Output
The script returns an overall pitch score along with strengths and weaknesses:

Example Output:
```
Analyzing: Startup A
Pitch Score: 85/100

Strengths:
- Overview is strong: Clear and engaging description.

Weaknesses:
- Stage section needs improvement: Lack of clarity on traction.
```

## Future Improvements
- Fine-tune evaluation with additional AI models.
- Implement a web-based interface for easier pitch assessments.
- Support for multiple pitch formats (PDF, text, etc.).

## License
This project is open-source unlicenced.

## Contributors
- Harika Vaddempudi

## Contact
For any inquiries, reach out at [vaddempudiharika@gmail.com](mailto:vaddempudiharika@gmail.com).

