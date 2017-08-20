# Sincding

[![circleciB]][circleciL]
[![npmVersionB]][npmVersionL]
[![npmDownloadsB]][npmDownloadsL]
[![dependenciesB]][dependenciesL]
[![greenkeeperB]][greenkeeperL]
[![contributionsB]][contributionsL]

[![bithoundB]][bithoundL]
[![codeclimateB]][codeclimateL]
[![coverageB]][coverageL]
[![codeissuesB]][codeissuesL]
[![styleB]][styleL]

**If you aren't familiar with CLI** (command line interface) programs you should check the [video tutorial](https://github.com/open-source-uc/sincding/blob/assets/tutorial.mp4).  
If you are, just keep reading.

You must have [node](https://nodejs.org) installed to use this (version >= 8)

Install with
```bash
npm install -g sincding
```

And then just run
```bash
sincding        # Run full program
sincding sync   # Update files quickly
```

On the first run you will be prompted for credentials
- **username**: Your uc username without @uc
- **password**: Your uc password
- **path**: The absolute path to the folder where you want to download the siding folders and files
- **ignore**: Space separated acronyms of courses you don't want to download. Usefull for those who are assistants. (example: IIC2154 IIC1103)

The credentials are stored in your Home directory on `.sincding/data.json`

Let's see it in action

![demo](https://github.com/open-source-uc/sincding/blob/assets/demo.gif)

***

# Development

Follow this script
```bash
git clone https://github.com/open-source-uc/sincding.git # Clone the repo
cd sincding     # Cd into directory
yarn            # Install dependencies
```

Run tests
```bash
yarn test
```

Run program
```bash
yarn start    # Run from project folder

npm link      # Link it
sincding      # Run from anywhere
```

### Tests

In order for tests to pass you must create a `.env.json` file in `./__tests__` like this
```json
{
  "username": "YOUR_UC_USERNAME",
  "password": "YOUR_UC_PASSWORD"
}
```

Check the [contributing guide](https://github.com/open-source-uc/sincding/blob/dev/CONTRIBUTING.md)

<!-- Badges -->
[circleciL]:https://circleci.com/gh/open-source-uc/sincding
[circleciB]:https://circleci.com/gh/open-source-uc/sincding.svg?style=svg

[npmDownloadsL]:https://www.npmjs.com/package/sincding
[npmDownloadsB]:https://img.shields.io/npm/dt/sincding.svg

[npmVersionL]:https://www.npmjs.com/package/sincding
[npmVersionB]:https://img.shields.io/npm/v/sincding.svg

[dependenciesL]:https://david-dm.org/open-source-uc/sincding
[dependenciesB]:https://david-dm.org/open-source-uc/sincding.svg

[greenkeeperL]:https://account.greenkeeper.io/account/open-source-uc
[greenkeeperB]:https://badges.greenkeeper.io/open-source-uc/sincding.svg

[styleL]:https://github.com/prettier/prettier
[styleB]:https://img.shields.io/badge/code%20style-prettier-brightgreen.svg?style=flat

[bithoundL]:https://www.bithound.io/github/open-source-uc/sincding
[bithoundB]:https://www.bithound.io/github/open-source-uc/sincding/badges/score.svg

[codeclimateL]:https://codeclimate.com/github/open-source-uc/sincding
[codeclimateB]:https://codeclimate.com/github/open-source-uc/sincding/badges/gpa.svg

[coverageL]:https://codeclimate.com/github/open-source-uc/sincding/coverage
[coverageB]:https://codeclimate.com/github/open-source-uc/sincding/badges/coverage.svg

[codeissuesL]:https://codeclimate.com/github/open-source-uc/sincding
[codeissuesB]:https://img.shields.io/codeclimate/issues/github/open-source-uc/sincding.svg

[contributionsL]:https://github.com/open-source-uc/sincding/issues
[contributionsB]:https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat
