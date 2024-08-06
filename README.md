# Human Facial Emotion Recognition (HFER)

## Introduction
HFER is a Python project that leverages a convolutional neural network to detect emotions from human faces which are extracted from images uploaded by a user. This streamlit front-end allows a user to upload an image and get an annotated image back with detected faces outlined. The emotions of these faces are then returned and displayed in tabular form.

## Usage

[Check out the website here](https://hfer-farid-nathan.streamlit.app)
### Local usage
1. Clone the repo.  
   **For those using the cloud-deployed API, skip to step 4.**
2. Follow the instructions in the [hfer](https://github.com/facial-emotion-recognition-service/hfer) repo's README to install and run the backend.
3. Change the URL on [line 9 of  `hfer_front/streamlit_fe.py`](https://github.com/facial-emotion-recognition-service/hfer_front/blob/1b5caf049802bfdb87bf5f439ad67a9f5420cc22/hfer_front/streamlit_fe.py#L9) to match the URL of your backend uvicorn server.
    ``` python
    # Example
    URL ="http://127.0.0.1:8000"
    ```

4. From the `hfer_front` directory run:
   ``` bash
   streamlit run hfer_front/streamlit_fe.py
   ```

## API
For more information on API usage please [visit the GitHub repository for the HFER backend](https://github.com/facial-emotion-recognition-service/hfer).


## Contributors
HFER was developed by two friends, [Farid](https://github.com/artificialfintelligence) and [Nathan](https://github.com/nihonlanguageprocessing), with significant input and guidance from a third friend: [Or](https://github.com/orbartal).
