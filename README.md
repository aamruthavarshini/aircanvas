AirCanvas is a computer vision–based drawing application that allows users to draw on a virtual canvas using hand gestures, without physically touching the screen. The application uses a webcam to capture real-time video and tracks finger movements to convert them into digital strokes. This project demonstrates practical use of computer vision techniques and real-time gesture recognition.

The main features of AirCanvas include real-time hand and finger tracking, the ability to draw using the index finger, multiple drawing colors, an eraser mode controlled through gestures, and a live webcam feed overlaid with a drawing canvas. The system is designed to be smooth, responsive, and intuitive, making it suitable for interactive and educational use cases.

The project is implemented using Python 3.11 along with popular libraries such as OpenCV for image processing, MediaPipe for accurate hand landmark detection, and NumPy for efficient numerical operations. These technologies together enable fast and reliable detection of hand movements and seamless drawing performance.

The project structure is kept simple and organized. It includes a main Python file that contains the application logic, a requirements file listing all dependencies, a README file for documentation, and a gitignore file to exclude virtual environments and cache files from version control. This structure makes the project easy to understand, run, and maintain.

To set up the project, the repository is first cloned from GitHub and a virtual environment is created to isolate dependencies. After activating the environment, all required libraries are installed using the requirements file. Once the setup is complete, the application can be launched by running the main Python script, which opens the webcam and starts the hand-tracking process.

Internally, the application works by capturing live video from the webcam and passing each frame to MediaPipe’s hand detection model. The model identifies hand landmarks, particularly the index finger tip, and tracks its movement across frames. These coordinates are then mapped onto a virtual canvas where drawing strokes are rendered in real time.

User interaction is handled entirely through hand gestures. Raising the index finger allows the user to draw, while specific combinations of fingers switch between drawing, selection, and eraser modes. The application can be exited safely by pressing the designated quit key. Gesture behavior may vary slightly depending on the implementation.

Future improvements for AirCanvas include adding the ability to save drawings as image files, implementing undo and redo functionality using gestures, supporting multiple hands, introducing a graphical toolbar overlay, and exploring mobile or touchless kiosk versions of the application.

