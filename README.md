# WASM-Canvas

HTML Canvas with logic written in C language, compiled with emscripten into a WebAssembly module.

Demo project from "Getting started with WebAssembly & Emscripten" course on Udemy (https://www.udemy.com/course/webassembly-emscripten/) made to ilustrate the benefits of using WebAssembly & Emscripten where there is a lot of computation to be done on the client side of a website.

## Running the project on your machine

1. CMD: npm install
2. CMD: yarn start
3. HUMAN: Open Google Chrome and navigate to http:\\localhost:2222

## Compiling the wasm module on your machine
1. HUMAN: Install emscripten on your machine (https://emscripten.org/docs/getting_started/downloads.html)
2. CMD: emcc lib\canvas.c -s WASM=1 -s "EXPORTED_FUNCTIONS=['_main', '_getCircles']" -o public\canvas.js
