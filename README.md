# CSE 476 Final Project

This project uses a reasoning agent that sends each question to the provided model API and collects the final answers. The program loads the test questions from a JSON file, gets responses from the model, and writes the outputs into a new JSON file.

## How to Run
1. Connect to ASU network or use a VPN to connect.
2. Install pip install requests
3. Run using: python generate_answer_template.py

Answers will be written to:
cse_476_final_project_answers.json

## Techniques Used
- Specific domain prompting
- Self-consistency (two model calls for math and logic)
- Output checker with retry on wrong answers

## Files
- agent/api_client.py - model API 
- generate_answer_template.py – agent loop and output generator
- cse_476_final_project_test_data.json – input test data
- cse_476_final_project_answers.json – output answers file
