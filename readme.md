

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


添加git 
ssh-keygen
vim ~/.ssh/id_rsa.pub  


插入更新
        $flight = new Flight;

        $flight->name = $request->name;

        $flight->save();

查询一遍自动更新模型时间
$flight = App\Flight::find(1);
$flight->name = 'New Flight Name';
$flight->save();


//=========后台登陆模板引入
1.改server.php为index.php .hitacss 复制到根目录

2修改database.php 中添加            'password' => env('DB_PASSWORD', ''),
 修改.env DB_PREFIX=blog_
 创建新方法pubf回车

 后台   1.登陆

 创建AdminController控制器
 
 ===========================2018.7.30
 golaravel.com/download  
sourcetree
开启php扩展 php_openssl.dll  php_mbstring.dll php_pdo_mysql.dll

server.php 改成Index.php 直接不从public就能访问
伪静态linux 复制到最外层

怎么快怎么来

 ===========================2018.7.31

 LoginController

namespace App\Http\Controllers\Admin;

use Illuminate\Http\Request;

class LoginController extends CommonController
{
    public function login()
    {
    	return view('admin/login');
    }
}

CommonController

namespace App\Http\Controllers\Admin;

use Illuminate\Http\Request;
use App\Http\Controllers\Controller;

class CommonController extends Controller
{
    //
}

陈华地址,用哔哩哔哩18621744021 wang  引入验证码类
http://php.wysls.com/forum-2-3.html