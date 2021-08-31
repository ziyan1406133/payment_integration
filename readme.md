Aplikasi sudah dihost ke cloud platform Heroku. Gunakan postman collection dan environment terlampir.
> "heroku_payment_gateway_test.postman_environment" untuk menggunakan server remote
> "localhost-5000.postman_environment" untuk menggunakan server lokal

### Local Server

Untuk menggunakan server lokal, install terlebih dahulu modul-modul yang diperlukan
> pip install -r requirements.txt
Restore database "postgre_backup_db"
Jalankan server dengan command 
> flask run

### Akses database remote

Host        : ec2-18-235-45-217.compute-1.amazonaws.com
Database    : ded6sc2rb2b630
User        : hgfcicgedydrjq
Port        : 5432
Password    : 7ab96ad474cdb4e78fe0c70d0ab5fe00134ebac928500c4e0c65346d3d2622af
URI         : postgres://hgfcicgedydrjq:7ab96ad474cdb4e78fe0c70d0ab5fe00134ebac928500c4e0c65346d3d2622af@ec2-18-235-45-217.compute-1.amazonaws.com:5432/ded6sc2rb2b630
Heroku CLI  : heroku pg:psql postgresql-infinite-85028 --app z-payment-gateway-test