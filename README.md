# Spawn Judgehost DOMJudge

## Install docker

Jangan lupa install docker dan docker-compose dulu wkwkw

## Jumlah judgehost

Untuk mengubah jumlah daemon yang berjalan, cukup copy paste aja setting dari `core0` di `docker-compose.yml`. Ganti angka 0 nya jadi 1, 2, 3, ..., dst. Contoh bisa dilihat pada `core1`. Maks judgehost dalam 1 VM adalah (N - 1) dari jumlah core. Jangan lupa ganti `host-name`-nya ya.

## Login judgehost

Ganti username dan password pada `env/judgehost.env` sesuai portal senior.

## Jalankan judgehost

```sh
docker-compose up -d
```
