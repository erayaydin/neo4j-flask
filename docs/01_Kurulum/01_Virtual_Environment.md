Flask ile Neo4j kullanımına başlamadan önce, Python geliştirme ortamımızı hazırlayacağız. Bu geliştirme ortamımızda **Virtual Environment** ile kullandığımız paketlerin birbirine karışmamasını sağlayacağız. Örneğin bir projenizde py2neo paketinin **1.6.4** sürümünü kullanırken bir başka projenizde **2.0.0** sürümünü kullanabileceksiniz.

## Kurulum

`virtualenv` kurulumu için `pip` kullanacağız. Şu komutla `virtualenv` kurulumunu gerçekleştirelim.

~~~
pip install virtualenv
~~~

## Kullanım

Öncelikle boş bir virtualenv klasörü oluşturalım.

~~~
virtualenv neo4j-flask
~~~

Boş bir sanal ortam oluşturduk, fakat henüz bunu aktif etmedik. Bu yüzden içerisindeki paketlere erişimimiz yok. Şu komutla da virtualenv'i aktif edelim.

~~~
source neo4j-flask/bin/active
~~~

Windows kullanıcıları bu komutu çalıştıramayacaktır. Bu yüzden aşağıdaki komutu kullanabilirler.

~~~
cd neo4j-flask/Script
activate
~~~

Aktifleştirdikten sonra terminalinizde (projeadi) şeklinde bir prompt belirecektir. Bu şekilde virtualenvi aktifleştirdiğinizi anlayabilirsiniz.

## Paketler

Virtualenv'de bulunan paketleri görüntülemek için şu komutu kullanabilirsiniz.

~~~
~$ pip freeze
docutils==0.11
Jinja2==2.7.2
MarkupSafe==0.19
Pygments==1.6
Sphinx==1.2.2
~~~
