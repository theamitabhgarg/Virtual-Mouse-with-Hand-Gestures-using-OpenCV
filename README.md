\# Virtual Mouse Using Hand Gestures



A real-time \*\*virtual mouse\*\* built with Python, OpenCV, and MediaPipe that allows you to control the computer mouse using \*\*hand gestures captured through a webcam\*\*.



\## Features



\- Real-time hand tracking using MediaPipe

\- Move the mouse using your index finger

\- Left click using hand gestures

\- Right click using hand gestures

\- Double click using hand gestures

\- Take screenshots using a hand gesture

\- Live webcam-based processing



\## Tech Stack



\- \*\*Python\*\*

\- \*\*OpenCV\*\* – webcam capture and image processing

\- \*\*MediaPipe\*\* – hand landmark detection

\- \*\*PyAutoGUI\*\* – mouse movement and screenshots

\- \*\*Pynput\*\* – mouse click control

\- \*\*NumPy\*\* – angle and distance calculations



\## How It Works



The webcam captures live video frames, which are processed using MediaPipe's hand-tracking model.



MediaPipe detects \*\*21 hand landmarks\*\*, and the application uses the positions of these landmarks to calculate:



\- Finger angles

\- Distance between fingers

\- Hand gesture patterns



These gestures are then mapped to mouse actions such as movement, clicking, double-clicking, and taking screenshots.



```text

Webcam

&#x20;  ↓

OpenCV

&#x20;  ↓

MediaPipe Hand Tracking

&#x20;  ↓

21 Hand Landmarks

&#x20;  ↓

Angles \& Distances

&#x20;  ↓

Gesture Recognition

&#x20;  ↓

Mouse / Screenshot Action

```



\## Gesture Controls



| Gesture | Action |

|---|---|

| Index finger movement | Move mouse |

| Index bent + middle extended | Left click |

| Index extended + middle bent | Right click |

| Index + middle bent | Double click |

| Index + middle bent + thumb close | Screenshot |

| `Q` | Exit |



\## Installation



Clone the repository:



```bash

git clone https://github.com/Deepakdj007/Computer-Vision.git

```



Navigate to the project:



```bash

cd Computer-Vision/live\_mouse\_control\_using\_hand\_gestures

```



Create a virtual environment:



```bash

python -m venv venv

```



Activate it on Windows:



```powershell

.\\venv\\Scripts\\Activate.ps1

```



Install the dependencies:



```bash

pip install -r requirements.txt

```



Run the application:



```bash

python main.py

```



> Make sure your webcam is available and accessible to the application.



\## Project Structure



```text

live\_mouse\_control\_using\_hand\_gestures/

│

├── main.py          # Main application

├── util.py          # Angle and distance calculations

├── requirements.txt # Python dependencies

└── README.md        # Project documentation

```



\## Learning Goals



This project demonstrates practical concepts in:



\- Computer vision

\- Hand landmark detection

\- Gesture recognition

\- Coordinate mapping

\- Geometric calculations

\- Real-time video processing

\- Python automation



\## Future Improvements



\- Mouse scrolling using gestures

\- Drag and drop

\- Cursor smoothing

\- Gesture cooldown/debouncing

\- Volume and brightness control

\- Improved gesture classification

\- Better screen-coordinate mapping



\## Author



This project is developed by Amitabh Garg.

