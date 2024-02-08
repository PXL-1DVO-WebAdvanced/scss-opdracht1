# SCSS: Opdracht 1

## 1. Clone
Door deze opdracht te aanvaarden werd er een GitHub repository voor je aangemaakt. Volg de onderstaande stappen om een lokale clone te maken van deze repository:
- Kopieer de GitHub url
- Open VS Code
- Clone repository

<img src="https://github.com/PXL-1DVO-WebAdvanced/scss-opdracht1/blob/media/images/github.png?raw=true" alt="nmp init" width="250" />
<img src="https://github.com/PXL-1DVO-WebAdvanced/scss-opdracht1/blob/media/images/clone.png?raw=true" alt="nmp init" width="250" />

## 2. Initialiseer project
Voorlopig bevat de repository enkel een readme.md en een .gitignore bestand. Maak een nieuw Node.js project aan met de standaardwaarden door onderstaande commando uit te voeren in de terminal in de root van de projectfolder:

    npm init -y

<img src="https://github.com/PXL-1DVO-WebAdvanced/scss-opdracht1/blob/media/images/npm-init.png?raw=true" alt="nmp init" width="250" />
<img src="https://github.com/PXL-1DVO-WebAdvanced/scss-opdracht1/blob/media/images/package-json.png?raw=true" alt="nmp init" width="250" />

Wijzig de inhoud en verwijder eventuele scripts uit het package.json bestand.

## 3. Installeer sass
Om de scss bestanden te converteren (transpilen) naar gewone css bestanden moeten we het sass package toevoegen aan ons project.
Open hiervoor de terminal in de root van de projectfolder en voer het volgende commando uit:

    npm install sass

## 4. Script
Maak een dev script in het package.json bestand aan dat er voor zorgt dat het main.scss bestand binnende map scss wordt omgezet naar een main.css bestand in de map css. Ook de watch functie moet hierbijgebruikt worden.

    {
        "name": "scss-opdracht1",
        "version": "1.0.0",
        "description": "Mijn eerste scss project.",
        "main": "index.js",
        "scripts": {
            "dev": "sass --watch scss/main.scss:css/main.css"
        },
        "keywords": [],
        "author": "",
        "license": "ISC"
    }

## 5. Folders en bestanden
- Maak in de root folder van het project 2 nieuwe folders aan:
  - css
  - scss
- Maak in de scss-folder een nieuw bestand aan: main.scss
- Maak in de root folder een nieuw bestand aan: index.html

<img src="https://github.com/PXL-1DVO-WebAdvanced/scss-opdracht1/blob/media/images/projectstructure.png?raw=true" alt="project" width="250" />

**index.html:**

    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>SCSS</title>
        <link rel="stylesheet" href="css/main.css">
    </head>
    <body>
        <h1>Hello SASS!</h1>
    </body>
    </html>

## 6. SCSS
In het main.scss bestand schrijf je nu code om de achtergrondkleur van het body element te wijzigen naar een kleur naar keuze:

    body {
        background-color: orange;
    }

## 7. NPM
Voer het dev script uit met onderstaand commando in de terminal en bekijk het resultaat in de browser:
    
    npm run dev

*"dev" is de naam van het script zoals we dit hebben toegevoegd aan het package.json bestand*

## Extensions
<img src="https://github.com/PXL-1DVO-WebAdvanced/scss-opdracht1/blob/media/images/vscode-extensions.png?raw=true" alt="extensions" />