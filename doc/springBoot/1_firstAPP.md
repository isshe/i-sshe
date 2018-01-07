
# 第一个Spring boot程序

## 1.创建spring boot项目

###1.1 步骤
* 打开IntelliJ IDEA
* File->New->project->Spring Initializr
* 填写相关的信息即可(例如这里创建的项目为：isshetest；groupID为：com.isshe)

## 2. 修改源码
* 打开`src/main/java/com/isshe/IsshetestApplication.java`
* 在`@SpringBootApplication`后面添加`@RestController`
* 在`class`里面添加
```
@RequestMapping("/")
public String index(){
    return "Hello World."
}
```
* 保存，运行
* 在浏览器打开`localhost:8080`即可看到输出

