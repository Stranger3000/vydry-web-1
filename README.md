# Web skautského oddílu Vydry

- `site/` – hotový web (index.html, img, fonts). Nasazuje se právě tato složka.
- `.github/workflows/deploy.yml` – po každé změně ve větvi `main` nahraje `site/` přes FTP do `/www/`.
- FTP údaje jsou v Settings → Secrets and variables → Actions (`FTP_SERVER`, `FTP_USERNAME`, `FTP_PASSWORD`).
- Ruční nasazení: záložka Actions → „Deploy na hosting“ → Run workflow.

Repozitář musí zůstat **soukromý** – složka `site/fonts` obsahuje licencovaná písma, která se nesmí veřejně šířit.
