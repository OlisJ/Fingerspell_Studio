# Fingerspell Studio

Learn and practice the American Sign Language (ASL) fingerspelling alphabet in the browser.

- **Learn**: every letter A–Z on a 3D hand you can turn and view from any side, with step-by-step instructions and color-coded fingers. J and Z show their movement path.
- **Practice**: your camera checks your handshape live. The coach looks at each finger, tells you what to adjust, and guides you if your hand is too far, out of frame or poorly lit. Modes: A to Z, random, or spell a word.
- **Spell**: type any word or name and watch the hand fingerspell it at slow, normal or fast speed, with loop and step controls.
- Progress tracking, light and dark mode, and right- or left-hand display.

## Privacy

Hand tracking runs entirely in the browser with [MediaPipe Hand Landmarker](https://ai.google.dev/edge/mediapipe/solutions/vision/hand_landmarker). Video never leaves your device. Progress is stored only in your browser's local storage.


## How recognition works

MediaPipe returns 21 hand landmarks per frame. The page turns them into joint angles, fingertip distances, thumb position and pointing direction, then scores each letter with a set of per-finger rules. The same rules drive the coach's checklist, so every tip maps to a specific finger. If the coach misses a sign you make correctly, **Save my version** stores your own example of that letter.

Built with [three.js](https://threejs.org/) and [MediaPipe Tasks Vision](https://www.npmjs.com/package/@mediapipe/tasks-vision).
