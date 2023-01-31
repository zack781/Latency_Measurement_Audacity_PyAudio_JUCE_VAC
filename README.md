# Audio Latency Measurement

Measuring Audio Latency through Corelink using Audacity, PyAudio, JUCE, and VAC

Audacity
1. Generate a continous waveform (ex. sine)
2. Generate a different continuous waveform that continues the previous waveform (ex. square)

VAC
- Set up 2 Virtual Audio Cables

JUCE
1. Build and run the Juce Audio Plugin Host (APH)
2. Instaintiate a JUCE Corelink audio sender and receiver instance.
3. Set APH audio input to VAC A and its output to VAC B

Play and Record
1. Play the generated waveforms in Audacity
2. Run Latency_Measurer.py to record the audio stream through each VAC

Measurement
- The offset between the 2 recordings is the latency

