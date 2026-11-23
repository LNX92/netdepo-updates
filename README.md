# netdepo-updates

NetDepo'nun ev sunucusu (Cloudflare hızlı tüneli) her yeniden başladığında yeni bir adres alır.
Sunucu güncel adresi `sunucu.json` dosyasına yazar; el terminali ve masaüstü uygulaması
("Ev sunucusu (adres otomatik)" seçeneği) adresi buradan okur ve adres değişse de kendiliğinden yeniden bağlanır.

```json
{"v": 1, "url": "https://<ad>.trycloudflare.com/", "updated": "2026-11-24T00:00:00Z"}
```

Bu depoda kod yoktur. Dosyayı yalnızca ev sunucusunun bu depoya yazabilen anahtarı (deploy key) değiştirir.
Kaynak: özel LNX92/NetDepo deposu, `server/ev-sunucu/`.
