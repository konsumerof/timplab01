# timplab01

1. $ cd timplab01
 С помощью команды $ wget https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz скачал нужный архив
![Снимок экрана от 2022-03-18 14-10-07](https://user-images.githubusercontent.com/90759633/158992772-79b3fbd3-fe79-4255-a9c6-da81870881ca.png)
2. $ tar -xf node-v6.11.5-linux-x64.tar.xz
3. $ cd boost_1_69_0
 $ ls -l | wc -l
Ответ: 19 (количество файлов не включая вложенные директории)
4. $ find . | wc
Ответ: 66829
5. $ find . -name "*.cpp" | wc -l
Ответ: 13774
$ find . -name "*.h" | wc -l // количество заголовочных = 296
=> Ответ: количество незаголовочных и не цппшных = 52759
или $ find . -not -name "*.h" -not -name "*.cpp" | wc -l
6. $ find . -name "any.hpp"
./boost/spirit/home/support/algorithm/any.hpp
./boost/proto/detail/any.hpp
./boost/hana/fwd/any.hpp
./boost/hana/any.hpp
./boost/type_erasure/any.hpp
./boost/any.hpp
./boost/fusion/algorithm/query/any.hpp
./boost/fusion/algorithm/query/detail/any.hpp
./boost/fusion/include/any.hpp
./boost/xpressive/detail/utility/any.hpp
7. $ grep -rl 'boost::asio'
![Снимок экрана от 2022-03-18 17-49-07](https://user-images.githubusercontent.com/90759633/159025494-20acb792-590c-4155-a260-3c619ebc8a3c.png)
8. $ ./bootstrap.sh
$ ./b2
![Снимок экрана от 2022-03-18 18-09-03](https://user-images.githubusercontent.com/90759633/159029151-1038b9c4-f9c3-4af5-8232-9cf3ee0142c6.png)
9. $ mkdir ~/boost-libs
$ cd boost_1_69_0/boost_output/lib 
$ mv *.* ~/boost-libs
10. $ cd boost-libs
$ ls -sh
11. $ ls -S -sh
![Снимок экрана от 2022-03-18 18-18-25](https://user-images.githubusercontent.com/90759633/159030728-e4258e08-04ed-45e3-b354-1e4353eebc3e.png)
