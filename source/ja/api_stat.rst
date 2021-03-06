jubatus::client::stat
---------------------

..See `IDL definition <https://github.com/jubatus/jubatus/blob/master/src/server/stat.idl>`_ for original and detailed spec.
詳細は `IDL definition <https://github.com/jubatus/jubatus/blob/master/src/server/stat.idl>`_ を参照してください。

typedef
~~~~~~~

.. describe:: jubatus::stat::config_data

.. code-block:: c++

   message config_data {
     int window_size
   }


stat methods
~~~~~~~~~~~~

.. describe:: bool push(0: string name, 1: string key, 2: double val)

属性情報 ``key`` の値 ``val`` を与える。

.. describe:: double sum(0: string name, 1: string key)

属性情報 ``key`` を持つ値の合計値を返す。

.. describe:: double stddev(0: string name, 1: string key)

属性情報 ``key`` を持つ値の標準偏差を返す。

.. describe:: double max(0: string name, 1: string key)

属性情報 ``key`` を持つ値の最大値を返す。

.. describe:: double min(0: string name, 1: string key)

属性情報 ``key`` を持つ値の最小値を返す。

.. describe:: double entropy(0: string name, 1: string key)

属性情報 ``key`` を持つ値のエントロピーを返す。

.. describe:: double moment(0: string name, 1: string key, 2: int n, 3: double c)

属性情報 ``key`` を持つ値の ``c`` を中心とした ``n`` 次のモーメントを返す。
