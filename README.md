hi everyonew

Burada normal bir şekilde Flask-App'in çalışabilme için Dockerfile vardır. Fakat uygulamayı build ettiğimizde Image'ın boyutunun 1.01GB olduğunu gördüm. Bu normal bir image için çok yüksek bir büyüklük. 


Buna çözüm için Dockerfile'da mutlti-stage yapıyı kullanmaya karar verdim.

Dockerfile'da multi-stage build, Docker imajının birden fazla aşamasında çalışmasını sağlayan bir tekniktir. Bu yöntem, daha küçük ve güvenli bir çalışma zamanı ortamı oluşturmanıza olanak tanırken, geliştirme aşamasında daha büyük ve daha karmaşık araçlar kullanmanızı sağlar.


Gördüğünüz üzere "akademi" image'i 1.01GB'ken "akademi2023-flask-app" multi-stage'le 266MB 'a kadar düşürebildik.

Şimdi oluşturduğumuz image'i çalıştırıyoruz.
docker run -d -p 5001:5000 2023akademi


2023akademi image'mi onurcanoglu/akademi2023 dockerhub repo'ma pushladım.

