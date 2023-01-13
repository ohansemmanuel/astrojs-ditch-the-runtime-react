# Astro: ditch the runtime (React)

An astro clone of a [React starter project](https://create-react-app.dev) for educational purposes.

<br />

## Aim 🎯

To make a **simple** comparison between a similar Astro and React project and consider the runtime implication.

Results upon building the same project:

| Library   | file        | loc(lines of code) | size      |     |
| --------- | ----------- | ------------------ | --------- | --- |
| Astro     | index.html  | 44                 | 1kb       |     |
| React     | index.html  | 23                 | 744b      |     |
| **Astro** | **main.js** | **0**              | **0kb**   |     |
| **React** | **main.js** | **9,360**          | **318kb** |     |
| Astro     | main.css    | 43                 | 872b      |     |
| React     | main.css    | 56                 | 1kb       |     |

<br />

## Conclusion 🥂

The effect of asset optimisation in both libraries is arguably negligible. The major difference is the amount of Javascript shipped to the client.

**Astro ships none by default.**

**React ships over 9000+ lines of Javascript** for the same trivial application, with the React runtime overhead being the major culprit.

<br />

## Run the project 🛖

```bash
  git clone https://github.com/ohansemmanuel/astrojs-ditch-the-runtime-react.git
  cd astrojs-ditch-the-runtime-react
  npm install
  npm run start
```
