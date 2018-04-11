# Checkstyle

[Checkstyle](http://checkstyle.sourceforge.net) is a development tool to help programmers write Java code that adheres to a coding standard. It automates the process of checking Java code to spare humans of this boring (but important) task. This makes it ideal for projects that want to enforce a coding standard.

## Visual Code Extension

[Checkstyle for Java](https://marketplace.visualstudio.com/items?itemName=shengchen.vscode-checkstyle)

## Eclipse Checkstyle Plugin

[Eclipse Checkstyle Plugin](checkstyle.org/eclipse-cs)

### Install

* Go to `Help->Eclipse Marketplace...`
* Install [Checkstyle Plug-in by Larz Ködderitzch](http://marketplace.eclipse.org/content/checkstyle-plug)

### Config

* Go to `Windows->Preference->Checkstyle`

```ini
Rebuild project if needed: [prompt]
[x] Warn before losing configured file sets
[x] Include rules names in violations messages
[x] Include rules module id (if available) in violation messages
```

* Click in `New`.

```ini
Type="External Configuration File"
Name="custom checkstyle"
Localization=[path of the custom_checks.xml]
```

* Save this configuration.

* Select "Custom checkstyle", click on "Set as Default" and then `Apply and Close`

### Usage

* Right click on the chosen file
* `Checkstyle->Check Code with Checkstyle`
* See the warnings in the `Problems tab`

### Formatter

* Go to `Windows->Preference->Java->Code Style->Formatter`;
* Click on `Import...`
* Select the [file](eclipse_formatter.xml). It has the format which follow the checkstyle rules.

## Extension for Visual Code

[Checkstyle for Java](https://marketplace.visualstudio.com/items?itemName=shengchen.vscode-checkstyle)
