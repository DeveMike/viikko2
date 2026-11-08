# Viikko 2 – kävijälaskuri

http://195.148.21.19/viikko2/

Flask + Gunicorn Nginxin takana cPoudan Ubuntu-koneella. Jokainen lataus ajaa
`UPDATE laskuri SET kaynnit = kaynnit + 1 WHERE id = 1` MariaDB:ssä, joten luku
säilyy rebootin yli.

- `app.py` – sovellus
- `templates/index.html` – sivu
- `deploy/` – systemd-palvelu ja Nginx-konfiguraatio
