# Image -> Speech via LLM
# Image-to-Story Converter

This Streamlit application leverages the power of AI to transform images into captivating narratives, complete with audio narration. It utilizes a combination of image captioning, language generation, and text-to-speech models to create a unique storytelling experience.

## Features

*   **Image Captioning:** Extracts textual descriptions from uploaded images using the Salesforce BLIP model.
*   **Story Generation:**  Weaves engaging short stories based on the image captions using the OpenAI GPT-3.5-turbo model.
*   **Text-to-Speech:**  Converts the generated stories into natural-sounding audio using the ESPnet model from Hugging Face.
*   **Interactive Interface:** Provides a user-friendly Streamlit interface for uploading images and experiencing the generated stories and audio.
*   **Progress Bar:**  Offers visual feedback during the image processing and story generation stages.

## Setup

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/your-username/your-repository.git](https://github.com/your-username/your-repository.git) 
    cd your-repository
    ```

2.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt 
    ```

3.  **Obtain API Keys:**
    *   Get an OpenAI API key from [https://platform.openai.com/account/api-keys](https://platform.openai.com/account/api-keys).
    *   Get a Hugging Face API token from your Hugging Face profile settings.

4.  **Set Environment Variables:**
    *   Create a `.env` file in your project's root directory.
    *   Add the following lines to the `.env` file, replacing the placeholders with your actual keys:
        ```
        OPENAI_API_KEY=your_openai_api_key
        HUGGINGFACE_API_TOKEN=your_huggingface_api_token
        ```

## Usage

1.  **Run the App:**
    ```bash
    streamlit run app.py 
    ```

2.  **Upload an Image:**
    *   Use the file uploader to select an image (JPG format) from your computer.

3.  **Generate Story & Audio:**
    *   Click the "Please choose a file to upload" button.
    *   The app will process the image, generate a caption, create a short story, and convert it to audio.

4.  **View & Listen:**
    *   Expand the "Generated Image scenario" and "Generated short story" sections to view the generated text.
    *   Use the audio player to listen to the narrated story.

## Important Notes

*   Ensure you have valid OpenAI and Hugging Face API keys and have set them up correctly in your `.env` file.
*   The app currently supports only JPG image uploads.
*   The generated story is limited to a maximum of 50 words.
*   The audio is saved as a FLAC file (`generated_audio.flac`).

## Contributing

Contributions are welcome! If you have any ideas for improvements or bug fixes, please open an issue or submit a pull request.

## License

This project is licensed under the MIT License.
