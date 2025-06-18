<p align="center">
    <img src="https://pbo.tools/assets/images/logo.png" width="512">
</p>

<p align="center">
    <a href="https://github.com/PBO-Tools/DayZ-PBO-Obfuscator/releases/latest">
        <img src="https://img.shields.io/badge/Version-1.8.0-blue.svg?style=flat-square" alt="PBO Tools Version">
    </a>
</p>

PBO Tools is a free and user-friendly obfuscation suite, specially crafted for DayZ and ARMA. It simplifies the PBO obfuscation process, making it accessible to all users, regardless of their experience level.

We offer a professional edition subscription with advanced features such as an enhanced obfuscation model, automated code obfuscation, model binning, and more. This subscription is ideal for users looking for advanced obfuscation capabilities. <br><br>To purchase a subscription, please visit https://pbo.tools.

## Features

- Intuitive and user-friendly interface
- Utilizes an advanced PBO obfuscation model
- Breaks deobfuscation software, enhancing protection
- Automatically adds junk code to the PBO for additional security
- Offers automatic code obfuscation
- Supports model binarizing and obfuscation
- Includes PBO signing upon completion
- Regular updates and continuous improvements for enhanced functionality

## Installation

* Download the most latest version of PBO Tools and save the application to your Desktop. Then, drag a mod from your P Drive onto the exe and follow the on-screen instructions.

## Settings
* PBO Tools can be configured using the Settings.json file found in `\Documents\SIX Software\PBO Tools\Settings.json` 
Below is an overview of the current settings and their functions. Settings marked with ** require an active subscription to PBO Tools Professional Edition, which can be purchased at https://pbo.tools/products.
```
{
  
  "Version": "1.5", //Do not modify this, version control
  "Configuration": { 
    "SelectedGame": "DayZ", //Do not modify this, reserved for future use
    "BinarizeLocation": "Temp", //Temporary location for model binning, requires a valid subscription to PBO Tools Professional Edition **
    "PBOOutputLocation": "P:\\Output\\", //Location where the PBO will be saved, requires a valid subscription to PBO Tools Professional Edition **
    "SigningKeyLocation": "" //Path to your private key for signing, requires a valid subscription to PBO Tools Professional Edition **
  },
  "NotificationSettings": {
    "NotifyOnErrors": true, //Enables a five-beep notification when an error occurs
    "NotifyOnSuccess": true, //Enables a single-beep notification when an action is successful
    "DisplayWarnings": true //Enables display of warnings
  },
  "Updates": {
    "CheckForUpdates": true //Enables automatic check for updates on PBO Tools launch
  },
  "ExclusionLists": {
    "ExcludeFromPBO": [ //List of folders and files to exclude from being added to your PBO
      ".git\\",
      ".vs\\",
      ".vscode\\",
      ".idea\\",
      ".cfg",
      ".h",
      ".hpp",
      ".png",
      ".txt",
      "thumbs.db",
      ".dep",
      ".bak",
      ".log",
      ".pew",
      "source",
      ".tga",
      ".bat",
      ".psd",
      ".cmd",
      ".mcr",
      ".fbx",
      ".max",
      "$VERSION$",
      "$PRODUCT$",
      "$PREFIX$"
    ],
    "ExcludeFromCompression": [ //List of file extensions to exclude from compression
      ".p3d",
      ".wss",
      ".ogg",
      ".jpg",
      ".wav",
      ".fsm",
      ".paa",
      ".bin"
    ]
  },
  "PBOSettings": {
    "BinarizeModels": true, //Enables binarization of MLOD models, requires a valid subscription to PBO Tools Professional Edition **
    "BinarizeConfigs": true, //Enables binarization of configs from config.cpp to config.bin
    "CompressPBO": true, //Enables compression of the PBO
    "JunkFiles": true, //Adds junk files to the obfuscated PBO
    "CrashUnpackers": true, //Intentionally crashes DayZ deobfuscators
    "ScrambleScriptPaths": true, //Scrambles the paths of scripts to obfuscate their location
    "UseWindowsGUIDs": false, //Adds Windows GUIDs to paths (see https://shorturl.at/gBRS5)
    "InvalidFileExtensions": true, //Renames files to have invalid Windows extensions such as NULL, COM, etc.
    "ComplexPaths": true, //Adds long, complex Unicode characters to paths
    "IncludeNonVisibleChars": true, //Includes Unicode paths with invisible characters
    "ObfuscateClasses": true, //Obfuscates class names, requires a valid subscription to PBO Tools Professional Edition **
    "ObfuscateFunctions": true, //Obfuscates functions, requires a valid subscription to PBO Tools Professional Edition **
    "ObfuscateTypes": true, //Obfuscates types, requires a valid subscription to PBO Tools Professional Edition **
    "ObfuscateVariables": true, //Obfuscates variables, requires a valid subscription to PBO Tools Professional Edition **
    "ObfuscateStrings": true, //Obfuscates strings, requires a valid subscription to PBO Tools Professional Edition **
    "EnableTypeDefs": false //Enables defining strings, variables, functions, etc., requires a valid subscription to PBO Tools Professional Edition **
  }
}
```

## Support

* If you encounter any issues, please visit https://discord.pbo.tools and open a ticket and we'll get you sorted.

## Documentation 

* https://docs.pbo.tools
  
## License
* https://pbo.tools/end-user-licence-agreement

## Privacy Policy
* https://pbo.tools/privacy-policy
