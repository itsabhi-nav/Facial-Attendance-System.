Facial Attendance System 

Overview

Welcome to the Facial Attendance System GitHub repository, a robust and user-friendly solution for attendance tracking using facial recognition technology. This system leverages Streamlit for the web interface, Redis for efficient data storage, and the powerful Insightface library for accurate face recognition.

Components

1. home.py

   * Description: The main module for the Streamlit web application.
  
   * Key Features:

      * Sets up the Streamlit app with an intuitive header and loading messages.
      * Loads the face recognition model seamlessly and establishes a connection to a Redis database.
      * Implements functions to retrieve data from Redis, conduct face recognition, and maintain attendance logs.
    
2. face_rec.py

  * Description: Module encompassing functions and classes crucial for facial recognition and user registration.

  * Key Features:

      * Connects to a Redis database to facilitate data storage.
      * Implements face recognition using the Insightface library, employing cosine similarity for accuracy.
      * Introduces a real-time prediction class for live video stream processing.
      * Features a registration form class for adding new users to the system.
    
3. real_time_prediction.py

  * Description: Real-time attendance prediction module.

  * Key Features:

    * Integrates the Streamlit WebRTC component for seamless real-time video streaming.
    * Retrieves up-to-date data from the Redis database.
    * Implements a callback function to process video frames, execute face recognition, and record attendance logs dynamically.

4. registration_form.py

  * Description: Module designed for user registration.

  * Key Features:

    * Presents a user-friendly Streamlit interface for collecting user information and facial features.
    * Manages the storage of facial embeddings locally and subsequently registers the data in the Redis database.
      
5. report.py
   
  * Description: Reporting module for displaying registered data and attendance logs.

  * Key Features:

    * Constructs a Streamlit interface with tabs, enabling users to view registered data and attendance logs effortlessly.
    * Offers the convenience of refreshing and accessing the latest data from the Redis database with just a click.
      
Getting Started

To deploy the Facial Attendance System, follow these straightforward steps:

1. Install the necessary dependencies (streamlit, numpy, pandas, cv2, redis, insightface, streamlit-webrtc).
2. Launch the Streamlit app by executing streamlit run home.py in your terminal.

   
Feel free to explore and tailor the code to suit your specific requirements. Should you encounter any challenges or wish to contribute enhancements, kindly open an issue or submit a pull request.

Let the Facial Attendance System simplify your attendance tracking with precision and ease!
