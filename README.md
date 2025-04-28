# docker
dev docker

<!-- コンテナ起動 -->
docker-compose up -d
<!-- コンテナ削除 -->
docker-compose down -v
<!-- コンテナの中に入る -->
docker exec -it postgres_container psql -U postgres -d postgres
<!-- volume.参照 -->
docker volume ls
<!-- volume.削除 -->
docker volume rm docker_postgres_data
<!-- docker composeの確認 -->
docker-compose version
<!-- 停止中のコンテナを確認 -->
docker ps -a
<!-- 不要なコンテナを削除 -->
docker rm <コンテナIDまたは名前>
<!-- 不要なイメージを削除 -->
docker rmi <イメージID>

ALTER DATABASE postgres SET timezone TO 'Asia/Tokyo';

<!-- テーブル名取得 -->
SELECT table_name
FROM information_schema.tables
WHERE table_schema = 'public';

select * from users;