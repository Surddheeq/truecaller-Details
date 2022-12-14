# truecaller-Details

[![Version](https://img.shields.io/badge/Version-1.0.4-blue)](https://github.com/sumithemmadi/truecaller-on-termux/releases)
[![stars](https://img.shields.io/github/stars/sumithemmadi/truecaller-on-termux)](https://github.com/sumithemmadi/truecaller-on-termux/stargazers)
[![MIT Licence](http://img.shields.io/github/license/sumithemmadi/truecaller-on-termux)](https://github.com/sumithemmadi/truecaller-on-termux/blob/main/LICENSE)
[![issues](https://img.shields.io/github/issues/sumithemmadi/truecaller-on-termux)](https://github.com/sumithemmadi/truecaller-on-termux/issues)

A simple truecaller on termux

<div class="imgs" style="center">
    <img src="https://user-images.githubusercontent.com/50250422/139717425-824b5468-29d4-4514-8b4a-77b119239501.jpg">
</div>

## Before we start
Before we start/ you should do the following things.
1. Make sure that you install [termux-api](https://f-droid.org/packages/com.termux.api/)
2. Now you should give notifications permission to termux-api.
```bash
termux-notification-list
```
3. After running above command in termux,click **Allow**.
3. Then run `termux-notificatin-list` and see a json is showing or not.
If it's not shown try enabling Auto Start for Termux:API and disable all battery optimizations.
https://dontkillmyapp.com/xiaomi
4. Make sure that you install `git` and `make`.

## Installation and Login

First clone this repository.

```bash
git clone https://github.com/surddheeq/truecaller-Details.git
cd truecaller-Details
```

```
make install
```
Then [login](https://github.com/surddheeq/truecaller-Details.git)to your Truecaller account.

After installation you need to restart session or source this file:

```bash
source start-truecallerjs.sh
```

Now you ready to enable and start the `truecallerjs` daemon service:
```bash
sv-enable truecallerjs
sv up truecallerjs
```

```
TYPE : truecallerjs -s (victim number)  [Then Click Enter Bottom]
```
then show you your victim sim details! E.T.C ðŸ˜„
If you need to stop, run `sv down truecallerjs`
> **Note** : If you get any error just close the termux app and reopen it.Then start truecallerjs services.
> **Note** : If it is not working export  the exvironment variable DEFAULT_DIALER_APP="Yor Dialer App Package Name" .
- [click here](https://support.google.com/admob/answer/9972781?hl=en) to know about package name
```bash
export DEFAULT_DIALER_APP="Yor Dialer App Package Name"
```

Example 1: If you use MI Dialer which has a package name `com.android.incalleriu`.
```bash
~$ export DEFAULT_DIALER_APP="com.android.incalleriu"
```

### To uninstall 
```
make uninstall
```

Then stop service with below command

```
sv down truecallerjs
sv-disable truecallerjs
```
## LICENSE

MIT License

Copyright (c) 2022 HOTORO_KING by Abir-rahman 2021

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

DON'T USE THE TOOL ILLEGALLY!!!!
