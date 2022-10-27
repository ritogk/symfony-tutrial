# symfony cli insatll
curl -1sLf 'https://dl.cloudsmith.io/public/symfony/stable/setup.deb.sh' | sudo -E bash
sudo apt install symfony-cli

# project作成

---

`composer create-project symfony/skeleton:"6.1.*" my_project_directory`

## symfony 起動
symfony server:start -d  
or  
`php -S 127.0.0.1:8000 -t public`  
## symfony server log出力(色付き)
symfony server:log  

## symfony 環境変数出力
symfony var:export

## symfony エンティティからmigration作成
symfony console make:migration

## symfony マイグレーションからDB後進
symfony console doctrine:migrations:migrate

## php
# php モジュール確認
php -m

## pdo_pgsql install
sudo apt-get install php-pgsql