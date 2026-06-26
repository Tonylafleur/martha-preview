# Martha Residence Platform

Plateforme de reservation hoteliere premium pour Martha Travel and Consulting Group - Residence Martha, Yaounde.

## Stack

- React 18 + Vite
- TailwindCSS
- API Node.js / Express
- PostgreSQL
- Docker Compose

## Lancement

```bash
docker compose up --build
```

URLs locales :

- Site : http://localhost:5173
- API : http://localhost:4000/api/health
- PostgreSQL : localhost:5434

## Fonctionnalites incluses

- Accueil mobile-first avec hero immersif, recherche de disponibilites, appartements, avis et FAQ.
- Pages : accueil, appartements, detail, disponibilites, reservation, a propos, contact, FAQ, confidentialite, conditions.
- Tunnel de reservation sans compte obligatoire.
- Options : navette aeroport, blanchisserie, demande speciale.
- Choix de garantie/paiement : sur place, MTN MoMo, Orange Money, carte via passerelles compatibles Cameroun.
- Base PostgreSQL avec hebergements, reservations, paiements, options et calendriers iCal.
- Endpoints API pour disponibilites, reservations, paiement, export iCal.

## Notes d'integration paiement

Le code expose un point d'extension `backend/src/payments.js` pour brancher Monetbil, Campay ou CinetPay. Les appels actuels simulent l'initialisation du paiement pour que le tunnel fonctionne localement sans cles API.
