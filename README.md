* 让左侧的图例栏，不可双击：  
通过判断不等于0，`obj.data.loc.split(' ')[0] !== '0'`，说明不在左侧的图例栏中
```
doubleClick: function (e, obj) {
    if (obj.data.category === "Command" && obj.data.loc.split(' ')[0] !== '0') {
        window.myVue.form.jobType = obj.data.category
    }
}
```