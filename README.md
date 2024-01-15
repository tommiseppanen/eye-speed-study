# Visual perception study
After reading an article about the [speed of human visual perception and flicker fusion](https://www.hs.fi/tiede/art-2000010100592.html) (article references [a white paper](https://www.biorxiv.org/content/10.1101/2023.11.15.567175v1) about the subject), I wanted to test if I could reproduce the same phenomenon with my computer screen.

I prepared a simple DX12 app to test the flicker fusion threshold by continuosly rendering black and white frames after each other. Then I tested the application with different refresh rates.
## PC Test results:
### Display #1 (144Hz with 160 Hz OC mode)
Display adjusted from Windows to different refresh rates
- 60 FPS flicker
- 95 FPS flicker
- 144 FPS no-flicker
- 160 FPS no-flicker

### Display #2 (60 Hz)
- 60 FPS flicker

### 144 Hz Variable Refresh Rate (VRR) display with capped FPS:
FPS value verified from the screen's own FPS meter
- 60 FPS flicker
- 120 FPS flicker
- 130 FPS flicker
- 140 FPS flicker

### Native refresh rate (144 Hz) but render two frames of each color:
- 77 FPS flicker

## Web Test results:
I decided to continue the testing with a simple web app since I had a couple of mobile devices with different refresh rates. The web test was also run on a desktop browser to verify results.

### Mobile phone #1 
- 120 Hz no-flicker
- 60 Hz flicker

### Mobile phone #2
- 90 Hz no-flicker

### Desktop browser
- 144 Hz no-flicker
- 95 Hz flicker
- 60 Hz flicker

Based on these tests, the flickering seems to disappear when approaching the maximum update frequency of the displays (except the 60 Hz desktop screen). That makes me think that could it be just due to ghosting/persistence of the screens. However, more testing with faster displays would be needed.
