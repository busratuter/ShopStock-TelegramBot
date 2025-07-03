# 🛍️ Shop Stock Checker Bot (Telegram Mesajı + Bildirim Sesi)

Bu Python kodu ürünlerin stoklarını kontrol edip istediğiniz beden stoğa gelince size telegram mesajı ve bildirim sesi yollar.

## Nasıl Kullanılır?

### 1. Repository'i klonlayın veya zip olarak indirin

### 2. Gerekli paketleri indirin
`pip install -r requirements.txt` terminale yazarak indirebilirsiniz

### 3. Config dosyasına istediğiniz linkleri kurun
 ```json
{
    "urls": [
        {
            "store": "bershka",
            "url": "https://www.bershka.com/tr/saplı-distressed-bowling-çanta-c0p177309999.html?colorId=742"
        },
        {
            "store": "zara",
            "url": "https://www.zara.com/tr/tr/z1975-genis-paca-orta-bel-yan-dikisli-jean-p06164103.html?v1=441123665"
        }
    ],
    "sizes_to_check": [ "XS", "S", "36"],
    "sleep_min_seconds": 180,  
    "sleep_max_seconds": 240
}
```
url kısmına istediğiniz linki, sizes_to_check kısmına istediğiniz bedenleri yazabilirsiniz. İstediğiniz kadar store ve url ekleyebilirsiniz. 

## 4. Botu çalıştırın!
`python main.py` yazmanız yeterli

## 5. Opsiyonel: Telegram Mesaj Botu Kurulumu
+ Telegram'a girin -> BotFather'ı aratıp seçin ve /newbot komutunu kullanın.
+ Botunuza isim verin. İsim verdikten sonra HTTP API ve chat id'nizi size yollayacak.
+ .env isimli bir dosya kurun ve bu iki variable'ı şu formatta yazın:
```env
BOT_API=your_telegram_bot_api_key
CHAT_ID=your_chat_id
``` 

