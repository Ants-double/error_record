# servlet

## 主要流程

### 来源

![servlet](E:\my_github\error_record\image\web\servlet.png)

### 解答

Servlet的生命周期一般可以用三个方法来表示：

1. init()：仅执行一次，负责在装载Servlet时初始化Servlet对象
2. service() ：核心方法，一般HttpServlet中会有get,post两种处理方式。在调用doGet和doPost方法时会构造servletRequest和servletResponse请求和响应对象作为参数。
3. destory()：在停止并且卸载Servlet时执行，负责释放资源

初始化阶段：Servlet启动，会读取配置文件中的信息，构造指定的Servlet对象，创建ServletConfig对象，将ServletConfig作为参数来调用init()方法。所以选ACD。B是在调用service方法时才构造的

