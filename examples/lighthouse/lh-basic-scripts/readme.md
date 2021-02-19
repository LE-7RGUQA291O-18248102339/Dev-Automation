# lighthouse basic examples: Scripting

---

Go to the [GitHub Playbook-Automation published page](https://section508coordinators.github.io/Dev-Automation/)

---

## lighthouse: programmatic usage

The scripts (JavaScript) in this project are meant to provide relatively simple examples, on which you can build, of how to use the pa11y  accessibility engine for accessibility testing using various configurations and rulesets - to include Deque's axe-core and SQIZ Lab's HTML CodeSniffer.  

## Automated tools and rulesets

#### Ruleset assessments and recommended rules

This tool allows the user to pick and choose the individual, underlying rules for testing. Not all automated tool rulesets on the market perfectly align with the pass/fail success criteria as expressed by the DHS standard. However upon analysis, DHS OAST has identified specific rules, for specific vendor accessibility ruleset libraries, that provide value in identifying accessibility to the DHS Standard.

Those analyses of vendor accessibility rulesets and the OAST ruleset recommendations reside in [rulesets folder](/rulesets) on this site.

---

## Technology requirements

These examples use the following technology stack:

- Chrome
- Nodejs 12+
- Git (Bash window)
- google lighthouse

## Setup

Perform the following steps to setup your environment to run the examples

2. Install Chrome desktop
2. Install Git 
2. Install Node
2. Install lighthouse: `npm install -g lighthouse`
2. Reboot

---

## Usage/Syntax

In a Git Bash window, run: `node <script_name>`

---

### Example scripts


The scripts will present different scenarios based on their internal configurations as follows:

- <u>*Script 1*</u>:`01_lighthouse_BasicScript.js`: This script will:

  - Runs only the audit (test) for 'accessibility' against one URL and all audits (rules)
  - launches a visual instance of Chrome briefly while testing the page then closes 
  - Writes an HTML report to your local machine file system.

- <u>*Script 2*</u>:`02_lighthouse_BasicScript.js`: This script will:

  - Runs only the audit (test) for 'accessibility' against one URL and all audits (rules)
  - launches a headless instance of Chrome and sends no results to command window

- <u>*Script 3*</u>:`03_lighthouse_BasicScript.js`: This script will:

  - Runs only the audit (test) for 'accessibility' against a single URL

  - Only tests against preferred audits (rules) favorable to TTv5

  - launches a headless instance of Chrome and sends no results to command window

---

# More Information

For more information on google lighthouse scripting, go here

- Programmatic usage (scripting): https://github.com/GoogleChrome/lighthouse/blob/master/docs/readme.md#using-programmatically
- Programmatic use: https://github.com/GoogleChrome/lighthouse/blob/HEAD/docs/readme.md#using-programmatically
- Lighthouse configuration: https://github.com/GoogleChrome/lighthouse/blob/HEAD/docs/

---

02/19/2021 | 10:33a
