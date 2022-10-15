
# Dockerize PHP

PHP'yi docker üzerinden çalıştırmak için kullanılır.

# Kurulum
Repository'i bir dizine clonlayın. Dizin içindeki "docker" dizinine geçiş yapın ve 
```bash
  docker-compose up 
```
komutu ile php 8 kurulumu tamamlanır ve container ayağı kalkar. 
[http://127.0.0.1:8080/](http://127.0.0.1:8080/) veya 
[http://localhost:8080/](http://localhost:8080/) veya adresi ile erişim sağlayabilirsiniz.

Not: src altındaki public dizine attığınız her dosya container'a kopyalanır.


# Docker üzerinde çalışan containerları listeleme

```bash
  docker ps
```
komutu ile aşağıda gördüğümüz gibi containerlar listelenecektir. 

Şimdi de PHP container'ının içine girip Word kütüphanesini yükleyelim. 

![Uygulama Ekran Görüntüsü](https://img.onl/G61SY) 

```bash
  docker exec -it cc9a10174be5 bash
```
komutu ile container içine girdik. Burada `composer require phpoffice/phpword` komutu ile phpWord kütüphanesini indirebiliriz.
