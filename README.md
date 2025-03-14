~$ cd coachtech/laravel
~/coachtech/laravel$ git clone git@github.com:coachtech-material/laravel-docker-template.git
~/coachtech/laravel$ mv laravel-docker-template kudamono
~/coachtech/laravel$ cd kudamono
~/coachtech/laravel/kudamono$ git remote set-url origin git@github.com:sakaki839/kudamono.git
~/coachtech/laravel/kudamono$ git remote -v
~/coachtech/laravel/kudamono$ git add .
~/coachtech/laravel/kudamono$ git commit -m "kudamono"
~/coachtech/laravel/kudamono$  git push origin main
~/coachtech/laravel/kudamono$  docker-compose up -d --build
~/coachtech/laravel/kudamono$ code .
~/coachtech/laravel/kudamono$  docker-compose exec php bash
root@1f85ba5f4343:/var/www# composer install
root@1f85ba5f4343:/var/www# cp .env.example .env
root@1f85ba5f4343:/var/www#  exit

root@8be88fd1ca20:/var/www#  php artisan make:controller ContactController


