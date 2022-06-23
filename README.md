INSTALL TAILWINDS

npm install -D tailwindcss
npx tailwindcss init

->Création fichier 'tailwind.config.js'
    changer contenu par:

    module.exports = {
    content: ["./src/**/*.{html,js}"],
    theme: {
    extend: {},
    },
    plugins: [],
    }

->Créer un dossier src avec fichier input.css

->CLI building process ajouter dans terminla:
                npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch





INSTALL SCSS dans nouveau terminal

                npm install

                npm init

->Créer un dossier sass avec fichier main.scss
    dans main.scss 
    ajouter:
                @tailwind base;
                @tailwind components;
                @tailwind utilities;

->Changer script dans package.json:
                sass --watch ./sass/main.scss:./src/input.css   

->Lancer SASS
                npm run sass       