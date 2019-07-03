**1.1.3**

* index.js: Reworked method "getI18nFile"; removed unnecessary variable in methods "writeBootStr" and "rmBootStr"; make use of "const" and "let"
* package.json: Updated version number to 1.1.3; changed to up-to-date versions of npm modules "fs-extra", "v-conf", "onoff" and "sleep"


**1.1.2**

* index.js: Code linted according to JavaScript Semi-Standard Style (https://github.com/Flet/semistandard)
* package.json: Updated version number to 1.1.2


**1.1.1**

* index.js: Change in method "writeBootStr" in order to avoid unnecessary write operations on /boot/config.txt
* i18n/strings_en.json: Fixed typo
* i18n/strings_de.json: Minor textual changes
* package.json: Updated version number to 1.1.1


**1.1.0**

* index.js: Added modal showing up if a reboot is required; added localization support for modals, toast messages etc.
* UIConfig.json: Adjustments for extended localization support
* i18n/strings_xx.json: Added strings for toast messages and "reboot required" user modal
* package.json: Updated version number to 1.1.0


**1.0.1**

* index.js: Corrected sleep time from microseconds (usleep) to milliseconds (msleep) in method "onVolumioShutdown"
* package.json: Updated version number to 1.0.1


**1.0.0**

* Initial commit
