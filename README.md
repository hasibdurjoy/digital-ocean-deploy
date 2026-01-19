Machine Create

one time setup
-----------------------
1) sudo apt update
2) sudo apt upgrade
3) curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
4) source ~/.bashrc
5) nvm install 20
6) sudo apt install nginx
7) create swap memory:   
     1) sudo fallocate -l 1G /swapfile
     2) sudo chmod 600 /swapfile
     3) sudo mkswap /swapfile
     4) sudo swapon /swapfile
     5) echo '/swapfile none swap sw 0 0'
8) sudo apt install htop
9) npm i -g pm2 yarn
10) sudo ufw enable
11) sudo ufw allow ssh
12) sudo ufw allow http
13) sudo ufw allow https
14) sudo apt install certbot python3-certbot-nginx
15) cd /etc/nginx
16) ls
17) sudo nano nginx.conf
18) comment  includes /etc/nginx/sites-enable/*

** Do Same For all repository
--------------------------------------
1) mkdir frontend
2) cd frontend
3) add github actions  (add command no 2, 4 then add option 4 then add command 5) -> Linux
4) export RUNNER_ALLOW_RUNASROOT="1"
5) sudo ./svc.sh install
6) sudo ./svc.sh start
7) push code from vs code
8) cd _work/project-name/project-name
9) 
        1) react vite->    pm2 serve dist/ --name="store-admin" 5000 --spa 
        2) next->            pm2 start npm --name frontend-or-admin -- run start -- -p 3000
        3) node->           pm2 start ./dist/index.js --name "backend" -p 5000

10) cd ~
11) cd /etc/nginx
12) cd conf.d
13) sudo nano frontend.conf   (then paste reverse proxy and edit domain)
14) sudo systemctl reload nginx
15) sudo certbot --nginx -d domain.com

** Manual Deploy
--------------------------------------
1) cd /etc/nginx  cd conf.d

Sudo nano file-name.conf

Paste domain proxy code and update domain and ports

Reload nginx

Certbot for ssl

