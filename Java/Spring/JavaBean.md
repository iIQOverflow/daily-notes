# JavaBean
**JavaBean是一个遵循特定写法的Java类**，它通常具有如下特点：
* 这个Java类必须具有一个无参的构造函数
* 属性必须私有化。
* 私有化的属性必须通过public类型的方法暴露给其它程序，并且方法的命名也必须遵守一定的命名规范。
代码示例：
```java
package gacl.javabean.study;

/**
 * @author gacl
 * Person类就是一个最简单的JavaBean
 */
public class Person {

    //------------------Person类封装的私有属性---------------------------------------
    // 姓名 String类型
    private String name;
    // 性别 String类型
    private String sex;
    // 年龄 int类型
    private int age;
    //是否已婚 boolean类型
    private boolean married;
    //---------------------------------------------------------
    
    //------------------Person类的无参数构造方法---------------------------------------
    /**
     * 无参数构造方法
     */
    public Person() {
        
    }
    //---------------------------------------------------------
    
    //------------------Person类对外提供的用于访问私有属性的public方法---------------------------------------
    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public String getSex() {
        return sex;
    }

    public void setSex(String sex) {
        this.sex = sex;
    }

    public int getAge() {
        return age;
    }

    public void setAge(int age) {
        this.age = age;
    }

    public boolean isMarried() {
        return married;
    }

    public void setMarried(boolean married) {
        this.married = married;
    }
    //---------------------------------------------------------
}
```
JavaBean在J2EE开发中，通常用于封装数据，对于遵循以上写法的JavaBean组件，其它程序可以通过反射技术实例化JavaBean对象，并且通过反射那些遵守命名规范的方法，从而获知JavaBean的属性，进而调用其属性保存数据。
## JavaBean的属性
**JavaBean的属性可以是任意类型，并且一个JavaBean可以有多个属性**。每个属性通常都需要具有相应的setter、 getter方法，setter方法称为属性修改器，getter方法称为属性访问器。
* 属性修改器必须以小写的set前缀开始，后跟属性名，且属性名的第一个字母要改为大写，例如，name属性的修改器名称为setName，password属性的修改器名称为setPassword。 

* 属性访问器通常以小写的get前缀开始，后跟属性名，且属性名的第一个字母也要改为大写，例如，name属性的访问器名称为getName，password属性的访问器名称为getPassword。 
* 一个JavaBean的某个属性也可以只有set方法或get方法，这样的属性通常也称之为只写、只读属性。
## 参考
[javaweb学习总结(二十)——JavaBean总结](https://www.cnblogs.com/xdp-gacl/p/3871730.html)