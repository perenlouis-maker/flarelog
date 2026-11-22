# FlareLog

Symptom-Tagebuch (Neurodermitis u. a.) als Web-App. Login per E-Mail und Passwort (Supabase), Daten in Supabase-Postgres mit Row-Level-Security, Hosting über GitHub Pages.

- `index.html` – die komplette App (eine Datei)
- Supabase-Projekt: Tabellen `settings`, `entries`, Freigabeliste `private.allowed_emails`
- Chat: Supabase Edge Function `chat`

Der Schlüssel in `index.html` ist der öffentliche (publishable) Key; der Schutz der Daten kommt von den RLS-Regeln.
