golaravel.com/download  
sourcetree
开启php扩展 php_openssl.dll  php_mbstring.dll php_pdo_mysql.dll

server.php 改成Index.php 直接不从public就能访问
伪静态linux 复制到最外层

怎么快怎么来

快速入门http://laravelacademy.org/post/8855.html

// 通过主键获取模型...
$flight = App\Flight::find(1);

// 获取匹配查询条件的第一个模型...
$flight = App\Flight::where('active', 1)->first();
$flights = App\Flight::find([1, 2, 3]);


$count = App\Flight::where('active', 1)->count();
$max = App\Flight::where('active', 1)->max('price');

        $flight = new Flight;

        $flight->name = $request->name;

        $flight->save();

更新
$flight = App\Flight::find(1);
$flight->name = 'New Flight Name';
$flight->save();

批量更新

更新操作还可以同时修改给定查询提供的多个模型实例，在本例中，所有有效且 destination=San Diego 的航班都被标记为延迟：

App\Flight::where('active', 1)
      ->where('destination', 'San Diego')
      ->update(['delayed' => 1]);

      