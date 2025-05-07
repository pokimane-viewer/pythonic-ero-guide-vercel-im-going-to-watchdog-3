# pythonic-ero-guide-vercel-im-going-to-watchdog-3

![GqXQZ8qXsAAuvbc](https://github.com/user-attachments/assets/055260ff-657a-4900-aea0-04cccfe66b8b)

![GqXQZ8lWwAATd4S](https://github.com/user-attachments/assets/8eab6c79-41b1-492a-ac42-86e4b6ce6590)

![GqXQZ8fWQAAmaTn](https://github.com/user-attachments/assets/7f2a2397-0dd6-4eec-be51-b501cf0107cd)

![GqXQqP2XYAAEp7O](https://github.com/user-attachments/assets/1afd340e-fd57-422f-9913-d5fd95763169)

you disgusting americans think you're that good that people need you at all? 白骑士抽搐定义

![GqXQZ8fWQAAmaTn](https://github.com/user-attachments/assets/9238e4a4-a693-480b-991a-e3274a8ea1fb)

![GqXQZ8lWwAATd4S](https://github.com/user-attachments/assets/1b700619-6772-48b6-a8e8-cfa1774a78d6)

![GqXQZ8qXsAAuvbc](https://github.com/user-attachments/assets/2206ef95-e494-4e4d-803c-9aa6805980aa)

# nginx conf file

/etc/nginx/sites-available/WHATEVER_THE_FUCK

# CHANGE THIS FLASK TO 3000; the SAME NGIX CONF; CHANGE EROSOLAR.ONLINE to whatever the fuck

server { server_name erosolar.online www.erosolar.online;

location / {
    proxy_pass http://127.0.0.1:3000;
    proxy_http_version 1.1;
    proxy_set_header Host $host;
    proxy_set_header X-Real-IP $remote_addr;
    proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
}

location /xcode {
    proxy_pass http://127.0.0.1:5000;
    proxy_http_version 1.1;
    proxy_set_header Host $host;
    proxy_set_header X-Real-IP $remote_addr;
    proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
}

listen 443 ssl; # managed by Certbot
ssl_certificate /etc/letsencrypt/live/erosolar.online/fullchain.pem; # managed by Certbot
ssl_certificate_key /etc/letsencrypt/live/erosolar.online/privkey.pem; # managed by Certbot
include /etc/letsencrypt/options-ssl-nginx.conf; # managed by Certbot
ssl_dhparam /etc/letsencrypt/ssl-dhparams.pem; # managed by Certbot
} server { if ($host = www.erosolar.online) { return 301 https://$host$request_uri; } # managed by Certbot

if ($host = erosolar.online) {
    return 301 https://$host$request_uri;
} # managed by Certbot


listen 80;
server_name erosolar.online www.erosolar.online;
return 404; # managed by Certbot
}
