- Clone repository
  git clone https://github.com/ferdhika31/Heroku-Wordpress.git

- Buat Aplikasi Heroku
cd wordpress && heroku create nama-aplikasi

- Install Plugin ClearDB
heroku addons:add cleardb:ignite

- Install Plugin New Relic
heroku addons:add newrelic:stark

- Install Plugin SendGrid
heroku addons:add sendgrid:starter

- Deploy aplikasi ke Heroku
git push heroku master

- Buka aplikasi heroku ke browser :
heroku open