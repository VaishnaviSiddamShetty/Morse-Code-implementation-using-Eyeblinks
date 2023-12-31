
# Blink-To-Text
This project focuses on building hybrid application which converts the blinking of eyes to text. It implements [Face Landmark Detection] from Tensorflow.js to capture movement of the eyes, and uses Morse Code to translate short and long blinks to alphabet characters.

## How to start
1. Download the project By cloning the repo to your local and go to the project directory.
2. Note: install node version >=14 to run the project and
3. In the ternmial
4. Run `npm install` in the directory.
5. Run `npm run blink` to start the project.
6. If the browser opens url *0.0.0.0:8080*, change it to *localhost:8080* and reload.

## How to use
1. Wait until the model loads.
2. When you see yourself, click *Start Capturing* button.
3. You have 7 seconds to blink the sequence you want.
4. If the converted letter is wrong, delete it with *Remove Letter*.

## Important files
#### JS
- `blinkPrediction.js` - Tensorflow.js model and prediction logic
- `hybridFunctions.js` - functions for loading camera on browser/mobile
- `morseCodeTable.js` - Morse Code dictionary
- `blinkStore.js` - Pinia store containing state of the app

#### Vue (UI)
- `LoadingPage.vue` - first screen that user sees while loading the model
- `MorseCodePage.vue` - helper screen to see Morse Code table
- `PredictingPage.vue` - main screen where predicting is happening

---

## WebPack

- There is a webpack bundler setup. It compiles and bundles all "front-end" resources. You should work only with files located in `/src` folder. Webpack config located in `script/webpack.config.js`.
- Webpack has specific way of handling static assets (CSS files, images, audios). 

## Documentation & Resources

* [Framework7 Core Documentation](https://framework7.io/docs/)
* [Framework7 Vue Documentation](https://framework7.io/vue/)
* [Vue3 Documentation](https://v3.vuejs.org/guide/introduction.html)
