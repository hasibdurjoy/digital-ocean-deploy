Machine Create

1. sudo apt update
2. sudo apt upgrade
3. curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
4. source ~/.bashrc
5. nvm install 20
6. sudo apt install nginx
7. create swap memory:
   1. sudo fallocate -l 1G /swapfile
   2. sudo chmod 600 /swapfile
   3. sudo mkswap /swapfile
   4. sudo swapon /swapfile
   5. echo '/swapfile none swap sw 0 0'
8. sudo apt install htop
9. npm i -g pm2 yarn
10. sudo ufw enable
11. sudo ufw allow ssh
12. sudo ufw allow http
13. sudo ufw allow https
14. mkdir frontend
15. cd frontend
16. add github actions
17. export RUNNER_ALLOW_RUNASROOT="1"
18. sudo ./svc.sh install
19. sudo ./svc.sh start
20. cd (name)
21. pm2 start npm --name nextjs-app -- run start -- -p 3000
22. cd ~
23. cd /etc/nginx
24. ls
25. sudo nano nginx.conf
26. sudo systemctl reload nginx
