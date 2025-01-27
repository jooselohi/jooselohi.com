## Jooselohi.com

Tämä opas tarjoaa vaiheittaiset ohjeet kotisivujen muutosten julkaisemiseksi Firebase Hosting -palvelun avulla.

### Ennakkovaatimukset

Ennen kuin aloitat, varmista että sinulla on seuraavat asiat:

- Node.js ja npm asennettuna järjestelmääsi.
- Firebase-projekti luotuna Firebase-konsolissa.

### Firebase CLI:n Asentaminen

1. Avaa komentorivi.

2. Asenna Firebase CLI globaalisti suorittamalla seuraava komento:

    ```bash
    npm install -g firebase-tools
    ```

3. Asennuksen jälkeen voit varmistaa, että Firebase CLI on asennettu oikein suorittamalla:

    ```bash
    firebase --version
    ```

### Julkaisuprosessi

1. **Kirjaudu Firebaseen:**

    Suorita seuraava komento ja seuraa ohjeita todentautuaksesi Firebaseen:

    ```bash
    firebase login
    ```

2. **Alusta Firebase:**

    Jos et ole vielä alustanut Firebaseä projektitiedostossasi, voit tehdä sen suorittamalla:

    ```bash
    firebase init
    ```

    Noudata ohjeita valitaksesi Firebase Hostingin, kun sinulta kysytään, mitä ominaisuuksia haluat asentaa.

3. **Julkaista muutokset Firebase Hostingiin:**

    Kun muutoksesi ovat valmiita julkaistavaksi, suorita seuraava komento julkaistaksesi ne:

    ```bash
    firebase deploy --only hosting
    ```

    Tämä komento lähettää /public-kansion sisällön Firebase Hostingiin, tehden muutokset näkyviksi.

4. **Pääsy Julkaistuun Sivustoon:**

    Onnistuneen julkaisun jälkeen Firebase CLI antaa sinulle linkin, jolla voit käydä katsomassa sivustoasi, kun se on nyt julkaistu. Jos olet yhdistänyt oman verkkotunnuksesi projektiin, muutoksen julkaistaan suoraan sinne myös.

Muutoksesi /public-kansiosta on nyt julkaistu ja näkyvissä Firebase Hostingissa.
