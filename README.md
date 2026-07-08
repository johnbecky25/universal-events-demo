# Universal Events Platform — Client Demo

  Interactive mockup for client pitches. No backend needed — pure static site.

  ## 🚀 Deploy on VPS (one-time setup)

  ```bash
  # 1. Clone the repo into nginx web root
  git clone https://github.com/johnbecky25/universal-events-demo.git /var/www/universal-events-demo

  # 2. Add nginx site (see nginx.conf in this repo)
  cp /var/www/universal-events-demo/nginx.conf /etc/nginx/sites-available/universal-events-demo
  ln -s /etc/nginx/sites-available/universal-events-demo /etc/nginx/sites-enabled/
  nginx -t && systemctl reload nginx
  ```

  ## 🔄 Update after changes (on VPS)

  ```bash
  cd /var/www/universal-events-demo && git pull
  ```

  That's it — no build step, no npm, no Node.js needed on the server.

  ## 📱 Demo screens

  | Path | What it shows |
  |------|--------------|
  | `/` | Pitch landing page — links to all modules |
  | `/preview/backstage-portal/OrganizerDashboard` | Full organizer dashboard (Registrations, Agenda, Speakers, Exhibitors, Design …) |
  | `/preview/backstage-portal/EventWebsite` | Public event website & registration |
  | `/preview/backstage-portal/CheckIn` | Gate check-in & badge printing |
  | `/preview/backstage-portal/NetworkingApp` | Attendee networking app |

  ## 📄 License
  Private demo — not for redistribution.
  