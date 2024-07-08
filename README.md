# Xkeys (BurpSuite Extension)
<img src="https://raw.githubusercontent.com/vsec7/BurpSuite-Xkeys/master/Screenshot/result.png">

## Description

A Burp Suite Extension to extract interesting strings (keys, secrets, tokens, etc.) from webpages. Then, lists it as information and issues.

Type : Passive Scanner

### Setup

<img src="https://raw.githubusercontent.com/vsec7/BurpSuite-Xkeys/master/Screenshot/install.png">

1. Setup your python environment by providing a <a href="https://www.jython.org/download.html">Jython.jar</a> file in 'Options' under 'Extender' in Burp Suite.
2. Download <a href="https://github.com/vsec7/BurpSuite-Xkeys/archive/master.zip">BurpSuite-Xkeys.zip</a>.
3. In 'Extensions' under 'Extender', select 'Add'.
4. Change the extension type to 'Python'.
5. Provide PATH of file "Xkeys.py". Click 'Next'.

## Usage
- The extension then starts identifying the assets through a passive scan.

## Results
- The extension shows issues boxes and an output extender.
<img src="https://raw.githubusercontent.com/vsec7/BurpSuite-Xkeys/master/Screenshot/log.png">

## The Possible Value Extractions are:
```
{keyword}=<value>
{keyword}= <value>
{keyword} =<value>
{keyword} = <value>
{keyword}'='<value>'
{keyword}'= '<value>'
{keyword}' ='<value>'
{keyword}' = '<value>'
{keyword}"="<value>"
{keyword}"= "<value>"
{keyword}" ="<value>"
{keyword}" = "<value>"
{keyword}":"<value>"
{keyword}": "<value>"
{keyword}" :"<value>"
{keyword}" : "<value>"
{keyword}=<value>&
```

### Requirements
- [Jython 2.7.0](https://www.jython.org/download.html)
- [Burp Suite Pro](https://portswigger.net/burp)

#### Credits:

```
# PortSwigger example-scanner-checks: https://github.com/PortSwigger/example-scanner-checks
# RedHuntLabs BurpSuite-Asset_Discover: https://github.com/redhuntlabs/BurpSuite-Asset_Discover
```

- Sec7or Team
- Surabaya Hacker Link
_eof_
