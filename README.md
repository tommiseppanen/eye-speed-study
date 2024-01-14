# Visual perception study
After reading an article about the [speed of human visual perception](https://www.hs.fi/tiede/art-2000010100592.html) (article references [a white paper](https://www.biorxiv.org/content/10.1101/2023.11.15.567175v1) about the subject), I wanted to test if I could reproduce the same phenomenon with my computer screen.

I prepared a simple DX12 app to test the flicker fusion threshold by rendering black and white frames after each other to computer screen.

## Test results:
### Display #1 (144Hz with 160 Hz OC mode)
- 60 FPS flicker (Windows refresh rate set to 60Hz)
- 144 FPS no-flicker
- 160 FPS no-flicker

### Display #2 (60 Hz)
- 60 FPS flicker

### 144 Hz VRR display with capped FPS:
- 60 FPS flicker
- 120 FPS flicker
- 130 FPS flicker
- 140 FPS flicker

### Native refresh rate 144 Hz but render two frames of each color:
- 77 FPS flicker
