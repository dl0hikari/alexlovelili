#创建流程

1. 创建配置文件config.py
2. 程序包的构造文件 app/\__init__.py
3. 创建蓝本（在蓝本中实现程序功能）
4. 注册蓝本（在程序包的构造文件中注册）
5. 蓝本中的错误处理程序, 蓝本中定义的程序路由
6. 编写models.py forms.py文件
7. 启动脚本（manage.py）
8. 创建mysql数据库（python file.py db init）
    ps: window 目前使用 pymysql
    ```
    $ pip install pymysql
    ```
    ```py
    # ...
    SQLALCHEMY_DATABASE_URI = 'mysql+pymysql://username:password@localhost:port/database'
    ```
    ```
    >>> db.create_all()
    ```

    linux 网上查资料需要安装 python-mysqldb 没有亲自证实
9. 新建base.html文件并重新编写代码