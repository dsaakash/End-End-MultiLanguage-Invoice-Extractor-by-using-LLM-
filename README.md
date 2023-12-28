
# Multilange Invoice Extractor by using gemini pro 

This project involves creating a web application using Streamlit, a popular framework for building data applications. The core functionality of the application is to process and interpret images, specifically invoices, using a combination of Google's generative AI and OpenAI models.

Key components of the application:

1. **Environment Setup**: The project begins by loading environment variables from a `.env` file using the `load_dotenv` function. This is a common practice for managing sensitive information like API keys.

2. **Importing Libraries and Configuring the AI Model**: Essential libraries such as `streamlit` for the web app interface, `os` for operating system interactions, and `PIL` for image processing are imported. The Google generative AI model, specifically the 'gemini-pro-vision' model, is configured using an API key obtained from the environment variables.

3. **Functions**:
   - `get_gemini_response`: This function integrates the 'gemini-pro-vision' model to generate responses based on a combination of text input, an image, and a prompt.
   - `input_image_setup`: It handles the image upload process, ensuring that uploaded files are properly read and formatted for processing.

4. **Streamlit Application Setup**: The Streamlit app is initialized with a specific page configuration and user interface elements. These elements include a header, text input for prompts, an image uploader, and a submit button.

5. **Processing User Input**: When a user uploads an image and inputs a prompt, the application uses the `get_gemini_response` function to process this information. It leverages the AI model to analyze the uploaded invoice image and generate a relevant response based on the prompt.

6. **Displaying Results**: The app displays the uploaded image and the AI-generated response to the user. This interaction allows users to extract and interpret information from invoice images using AI.

Overall, this project showcases the integration of advanced AI models with a user-friendly web interface, enabling users to extract insights from images with ease.


## Documentation

[Creating API from makersuite](https://makersuite.google.com/app/apikey)


## Environment Variables

A virtual environment in the context of Python programming is a self-contained directory that houses a specific version of Python and several additional packages. This environment operates independently of the system-wide Python installation and other virtual environments. The primary purpose of a virtual environment is to manage dependencies and versions for a specific project without affecting other projects or the global Python setup.

Key Aspects of Virtual Environments:

1. **Isolation**: Each virtual environment is isolated from others, ensuring that dependencies and packages used in one project do not conflict with those in another. This isolation is crucial in a scenario where different projects require different versions of the same package.

2. **Project-specific Dependencies**: By using a virtual environment, you can install and manage packages that are required for a particular project without impacting the global Python environment on your system. This means that each project can have its own dependencies, regardless of what is installed globally.

3. **Consistent Development Environment**: Virtual environments help maintain consistency across development, testing, and production stages. They ensure that the software runs in an environment with the exact version of the language and libraries that it was developed and tested with.

4. **Simplified Project Management**: Virtual environments make it easier to manage project dependencies, which is especially beneficial in larger projects or when working in a team. They allow different team members to work with the same setup and avoid the "it works on my machine" problem.

5. **Ease of Setup**: Setting up a virtual environment is straightforward. Tools like `venv` (included in Python 3) and `virtualenv` (a separate package for Python 2 and 3) provide simple commands to create and manage these environments.

6. **Portability**: A project with a virtual environment can be easily transferred between computers without worrying about the installed Python versions and packages on those systems. This makes sharing and collaborative development much more manageable.

In summary, virtual environments are a vital tool in Python development, offering an efficient way to manage project-specific dependencies and ensuring a consistent and isolated development environment.


## Features

- **Environment Variable Management**: Automatically loads environment variables from a `.env` file, ensuring secure and convenient handling of sensitive information like API keys.
  
- **Integrated AI Models**: Incorporates Google's 'gemini-pro-vision' generative AI model and OpenAI capabilities, offering advanced image processing and content generation directly within the application.

- **Streamlit Web Interface**: Utilizes Streamlit for creating an intuitive and interactive web application interface, making it user-friendly and accessible.

- **Image Upload and Processing**: Features an image upload functionality that supports common formats like JPG and PNG, along with an image processing system to prepare the uploaded images for AI analysis.

- **AI-Driven Analysis and Response**: Employs AI models to analyze uploaded images (specifically invoices) and generate contextual responses based on user prompts, enhancing the application's utility in information extraction.

- **Real-Time Response Display**: Showcases AI-generated responses in real-time, providing immediate insights and interpretations of the uploaded images.

- **Error Handling**: Includes a robust error handling mechanism, particularly for file uploads, ensuring a smooth user experience.

- **User Input Accommodation**: Offers text input fields for users to provide specific prompts, enhancing the customizability and relevance of AI responses.

- **Interactive Visualization**: Displays uploaded images within the web interface, offering users a visual confirmation of the files being analyzed.

- **Flexible API Key Configuration**: Allows for flexible configuration of API keys through environment variables, facilitating easy integration with different AI services.

These features combine to make the application a powerful tool for image-based data extraction and interpretation, leveraging cutting-edge AI technology within a user-friendly web interface.

## Installation Instructions for the AI-Driven Image Analysis Web Application

### Prerequisites
Before proceeding with the installation, ensure you have the following:
- Python (preferably Python 3.6 or later)
- `pip` (Python package manager)
- Access to terminal or command prompt
- A text editor or IDE of your choice
- An internet connection for downloading necessary packages

### Step-by-Step Installation Guide

1. **Clone or Download the Project Repository**
   - If the project is hosted on a platform like GitHub, clone the repository using Git, or download the project files to your local machine.

2. **Set Up a Virtual Environment (Optional but Recommended)**
   - Open your terminal or command prompt.
   - Navigate to the project directory.
   - Create a virtual environment:
     ```
     python3 -m venv venv
     ```
   - Activate the virtual environment:
     - On Windows:
       ```
       .\venv\Scripts\activate
       ```
     - On macOS or Linux:
       ```
       source venv/bin/activate
       ```

3. **Install Required Packages**
   - While the virtual environment is active, install the required packages using `pip`:
     ```
     pip install -r requirements.txt
     ```
   - This command will install Streamlit, Pillow, and other dependencies listed in `requirements.txt`.

4. **Setting Up Environment Variables**
   - Create a `.env` file in the root directory of the project.
   - Add your `GOOGLE_API_KEY` to the `.env` file:
     ```
     GOOGLE_API_KEY=your_api_key_here
     ```

5. **Running the Streamlit Application**
   - With the dependencies installed and environment variables set, run the Streamlit application:
     ```
     streamlit run your_app_script.py
     ```
   - Replace `your_app_script.py` with the name of the main Python script of the application (if different).

6. **Accessing the Web Application**
   - Streamlit will start a local server and provide you with a URL (typically `http://localhost:8501`).
   - Open this URL in a web browser to interact with the application.

7. **Using the Application**
   - Follow the on-screen instructions to upload images, enter prompts, and receive AI-driven analysis and responses.

### Troubleshooting
If you encounter issues:
- Ensure all dependencies are correctly installed.
- Verify that the `.env` file is correctly set up with the necessary API keys.
- Check for any error messages in the terminal for clues about what might be going wrong.

### Additional Notes
- Keep your API keys confidential and never commit them to a public repository.
- Update the project dependencies periodically to maintain compatibility and security.
## License

[MIT](https://choosealicense.com/licenses/mit/)


## Support

For support, email savantaakash322@gmail.com 


## Screenshots

![Screenshot](https://github.com/dsaakash/End-End-MultiLanguage-Invoice-Extractor-by-using-LLM-/blob/aefdee3dab29d701ed7b70cc230e8048decf8c62/Screenshots/Screenshot2_Invoice_Extractor.png)


## Demo

https://github.com/dsaakash/End-End-MultiLanguage-Invoice-Extractor-by-using-LLM-/blob/6eb8eb0877292d4a2a86a506c0eed6b5469341cc/Screenshots/invoice_extractor.png

