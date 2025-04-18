# Hand-Tracking-Piano
🎹 HandTracking Piano Control a virtual piano without ever touching a key — just by moving your fingers in the air! This project uses real-time hand tracking and MIDI synthesis to turn your hands into a playable piano interface.

Features
Touchless Piano: Play chords by simply raising your fingers in front of your webcam.

Chord Mapping: Each finger is mapped to a specific chord in the D major scale.

Real-Time MIDI Playback: Chords are played instantly using your system’s MIDI synthesizer via pygame.midi.

Visual Feedback: A live OpenCV video feed with hand landmarks for interaction clarity.

Sustain Control: Notes automatically fade out after a brief delay for more natural sound.

Multithreaded Playback: Ensures smooth transitions and simultaneous chord handling.

Technologies Used
Python

OpenCV – for video capture and visualization

cvzone (built on MediaPipe) – for hand and finger tracking

pygame.midi – to output MIDI sound

Python threading – for managing note sustain

Installation
Clone the repository:

git clone https://github.com/yourusername/handtracking-piano.git
cd handtracking-piano

Install the dependencies:
pip install opencv-python pygame cvzone
Make sure your system supports MIDI playback (or you have a virtual MIDI synth installed).

Usage
Simply run the script:
python piano.py
Raise a finger to play a chord.

Lower your finger to stop it (with a natural delay).

Both hands are supported — play up to 10 chords!

Press Q to quit.

Notes
Default chords are based on the D major scale.

MIDI Instrument is set to Acoustic Grand Piano (program 0).

You can customize chords or sustain time directly in the script.
