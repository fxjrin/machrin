# **Machrin**

## Table of Contents
- [About](#about)
- [Installation](#installation)
- [Features](#features)
- [Example-usage](#example-usage)
- [Help](#help)
- [Authors](#authors)

## About

Machrin is a system specifically designed to help its users with a variety of useful features designed specifically for the Growtopia community.

## Installation

```sh
npm install machrin
```

## Features

- server(), Fetches data from the Growtopia website.
- render(), Fetch rendering details for a specific world in Growtopia.

## Example-usage

### server()

```js
const { server } = require("machrin");

server().then(console.log);

    /*
    Example output :

    {
        date: 'July 15th',
        time: '07:15:06',
        player: 56789,
        wotd: 'MACHRIN',
        url: 'https://www.growtopiagame.com/worlds/machrin.png'
    }
    */
```

### render()

```js
const { render } = require("machrin");

render("machrin").then(console.log);

    /*
    Example output if successful :

    {
        world: 'MACHRIN',
        url: 'https://s3.amazonaws.com/world.growtopiagame.com/machrin.png',
        date: '07/15/2006',
        time: '07:15:06'
    }

    Example output if unsuccessful :

    {
        world: 'MACHRIN has never been rendered before',
        url: null,
        date: null,
        time: null
    }
    */
```

## Help

If you have questions, encounter issues, or need assistance with Machrin,
join our community on [Discord](https://discord.gg/2Csp257rYB) for quick assistance, friendly discussions,
and updates about Machrin.

## Authors

- [@fxjrin](https://www.github.com/fxjrin)
