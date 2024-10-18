# docker
dev docker

<!-- コンテナの中に入る -->
docker exec -it postgres_container psql -U postgres -d postgres
<!-- volume.参照 -->
docker volume ls
<!-- volume.削除 -->
docker volume rm docker_postgres_data
<!-- コンテナ起動 -->
docker-compose up -d
<!-- コンテナ削除 -->
docker-compose down -v

ALTER DATABASE postgres SET timezone TO 'Asia/Tokyo';
ALTER DATABASE postgres SET timezone TO 'Asia/Tokyo';