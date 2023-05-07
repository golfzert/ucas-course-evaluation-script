# 国科大评教脚本
```
x=document.getElementsByTagName("input")
select1=["口碑好","时间"]
for (var i=0;i<x.length;i++)
    {
        //console.log(x[i])
        if(x[i].getAttribute("value")=="5" &&
           x[i].getAttribute("type")=="radio")
            x[i].click()
        if(x[i].parentElement.textContent.match("合适")
)
            x[i].click()
        for (let sel of select1) {
            if(x[i].parentElement.textContent.match(sel))
                x[i].click()
            
            
        }
    }
x=document.getElementsByTagName("textarea")
var str1="                               "//自行填入其他文字
for (let xx of x) {
    xx.value=str1
    
}
```
# 使用方法
打开评教页面
f12打开开发者工具
点击源代码标签页,选择代码片段,新建代码片段后拷贝.按ctrl+enter执行
![image](https://user-images.githubusercontent.com/56443668/236660766-ebbf23cb-c3f5-4d29-84ab-2cc948145ead.png)

