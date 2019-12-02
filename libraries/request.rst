=================
Request 请求类
=================


+-------------+----------+
|属性         |值        |
+=============+==========+
|命名空间     |fize\\web |
+-------------+----------+
|类名         |Request   |
+-------------+----------+


:方法:


+-----------------+-------------------------------+
|方法名           |说明                           |
+=================+===============================+
|`__construct()`_ |初始化静态属性                 |
+-----------------+-------------------------------+
|`server()`_      |获取原生 SERVER                |
+-----------------+-------------------------------+
|`get()`_         |获取 GET 参数                  |
+-----------------+-------------------------------+
|`post()`_        |获取 POST 参数                 |
+-----------------+-------------------------------+
|`files()`_       |获取上传文件                   |
+-----------------+-------------------------------+
|`request()`_     |获取 REQUEST 参数              |
+-----------------+-------------------------------+
|`session()`_     |获取 SESSION 参数              |
+-----------------+-------------------------------+
|`env()`_         |获取 ENV 参数                  |
+-----------------+-------------------------------+
|`cookie()`_      |获取 COOKIE 参数               |
+-----------------+-------------------------------+
|`input()`_       |返回原始输入数据               |
+-----------------+-------------------------------+
|`header()`_      |获取请求头                     |
+-----------------+-------------------------------+
|`contentType()`_ |当前请求 HTTP_CONTENT_TYPE     |
+-----------------+-------------------------------+
|`method()`_      |当前的请求类型                 |
+-----------------+-------------------------------+
|`isGet()`_       |是否为 GET 请求                |
+-----------------+-------------------------------+
|`isPost()`_      |是否为 POST 请求               |
+-----------------+-------------------------------+
|`isPut()`_       |是否为 PUT 请求                |
+-----------------+-------------------------------+
|`isDelete()`_    |是否为 DELTE 请求              |
+-----------------+-------------------------------+
|`isHead()`_      |是否为 HEAD 请求               |
+-----------------+-------------------------------+
|`isPatch()`_     |是否为 PATCH 请求              |
+-----------------+-------------------------------+
|`isOptions()`_   |是否为 OPTIONS 请求            |
+-----------------+-------------------------------+
|`isCli()`_       |是否为 cli                     |
+-----------------+-------------------------------+
|`isCgi()`_       |是否为 cgi                     |
+-----------------+-------------------------------+
|`isSsl()`_       |当前是否 ssl                   |
+-----------------+-------------------------------+
|`isJson()`_      |当前是否 JSON 请求             |
+-----------------+-------------------------------+
|`isAjax()`_      |当前是否 Ajax 请求             |
+-----------------+-------------------------------+
|`isPjax()`_      |当前是否 Pjax 请求             |
+-----------------+-------------------------------+
|`isMobile()`_    |检测是否使用手机访问           |
+-----------------+-------------------------------+


方法
======
__construct()
-------------
初始化静态属性

.. code-block:: php

  public function __construct (
      array $config = []
  )


:参数:
  +-------+-------+
  |名称   |说明   |
  +=======+=======+
  |config |配置   |
  +-------+-------+
  
  


server()
--------
获取原生 SERVER

.. code-block:: php

  public static function server (
      string $key = null,
      string $default = null
  ) : mixed


:参数:
  +--------+----------+
  |名称    |说明      |
  +========+==========+
  |key     |键名      |
  +--------+----------+
  |default |默认值    |
  +--------+----------+
  
  


get()
-----
获取 GET 参数

.. code-block:: php

  public static function get (
      string $key = null,
      string $default = null
  ) : mixed


:参数:
  +--------+----------+
  |名称    |说明      |
  +========+==========+
  |key     |键名      |
  +--------+----------+
  |default |默认值    |
  +--------+----------+
  
  


post()
------
获取 POST 参数

.. code-block:: php

  public static function post (
      string $key = null,
      string $default = null
  ) : mixed


:参数:
  +--------+----------+
  |名称    |说明      |
  +========+==========+
  |key     |键名      |
  +--------+----------+
  |default |默认值    |
  +--------+----------+
  
  


files()
-------
获取上传文件

.. code-block:: php

  public static function files (
      string $key = null
  ) : mixed


:参数:
  +-------+-------+
  |名称   |说明   |
  +=======+=======+
  |key    |键名   |
  +-------+-------+
  
  


request()
---------
获取 REQUEST 参数

.. code-block:: php

  public static function request (
      string $key = null
  ) : mixed


:参数:
  +-------+-------+
  |名称   |说明   |
  +=======+=======+
  |key    |键名   |
  +-------+-------+
  
  


session()
---------
获取 SESSION 参数

.. code-block:: php

  public static function session (
      string $key = null,
      string $default = null
  ) : mixed


:参数:
  +--------+----------+
  |名称    |说明      |
  +========+==========+
  |key     |键名      |
  +--------+----------+
  |default |默认值    |
  +--------+----------+
  
  


env()
-----
获取 ENV 参数

.. code-block:: php

  public static function env (
      string $key = null,
      string $default = null
  ) : mixed


:参数:
  +--------+----------+
  |名称    |说明      |
  +========+==========+
  |key     |键名      |
  +--------+----------+
  |default |默认值    |
  +--------+----------+
  
  


cookie()
--------
获取 COOKIE 参数

.. code-block:: php

  public static function cookie (
      string $key = null,
      string $default = null
  ) : mixed


:参数:
  +--------+----------+
  |名称    |说明      |
  +========+==========+
  |key     |键名      |
  +--------+----------+
  |default |默认值    |
  +--------+----------+
  
  


input()
-------
返回原始输入数据

.. code-block:: php

  public static function input () : string


:返回值:
  失败时返回 false


header()
--------
获取请求头

.. code-block:: php

  public static function header (
      string $key = null,
      mixed $default = null
  ) : mixed


:参数:
  +--------+-------------------------------------------+
  |名称    |说明                                       |
  +========+===========================================+
  |key     |键名，不设置则返回请求头数组               |
  +--------+-------------------------------------------+
  |default |默认值                                     |
  +--------+-------------------------------------------+
  
  


contentType()
-------------
当前请求 HTTP_CONTENT_TYPE

.. code-block:: php

  public static function contentType () : string



method()
--------
当前的请求类型

.. code-block:: php

  public static function method () : string



isGet()
-------
是否为 GET 请求

.. code-block:: php

  public static function isGet () : bool



isPost()
--------
是否为 POST 请求

.. code-block:: php

  public static function isPost () : bool



isPut()
-------
是否为 PUT 请求

.. code-block:: php

  public static function isPut () : bool



isDelete()
----------
是否为 DELTE 请求

.. code-block:: php

  public static function isDelete () : bool



isHead()
--------
是否为 HEAD 请求

.. code-block:: php

  public static function isHead () : bool



isPatch()
---------
是否为 PATCH 请求

.. code-block:: php

  public static function isPatch () : bool



isOptions()
-----------
是否为 OPTIONS 请求

.. code-block:: php

  public static function isOptions () : bool



isCli()
-------
是否为 cli

.. code-block:: php

  public static function isCli () : bool



isCgi()
-------
是否为 cgi

.. code-block:: php

  public static function isCgi () : bool



isSsl()
-------
当前是否 ssl

.. code-block:: php

  public static function isSsl () : bool



isJson()
--------
当前是否 JSON 请求

.. code-block:: php

  public static function isJson () : bool



isAjax()
--------
当前是否 Ajax 请求

.. code-block:: php

  public static function isAjax () : bool



isPjax()
--------
当前是否 Pjax 请求

.. code-block:: php

  public static function isPjax () : bool



isMobile()
----------
检测是否使用手机访问

.. code-block:: php

  public static function isMobile () : bool



